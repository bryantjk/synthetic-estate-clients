# Synthetic estate-planning clients

Nine invented clients, each with a profile, a simulated attorney interview, an answer key for what the interview contains, and the follow-up intake form the client returned afterwards. Built to test systems that read estate-planning conversations and produce estate plans; usable by anyone working on the same problem.

Clients are grouped into four wealth tiers under `clients/`. The nine so far are all tier 1, the foundational tier where no estate has a tax problem. Tiers 2 to 4 are empty and open to contributors; see [Wealth tiers](#wealth-tiers).

Everything here is fabricated. No client, family member, address, employer or account is real.

## The nine (tier 1)

| # | Client | Shape | Built to test | Net worth |
|---|---|---|---|---|
| 01 | [Maria Elena Vega](clients/tier-1-foundational/01-vega/) | Single mother, straightforward plan | Guardianship, minor beneficiaries with age conditions, the guardian/trustee distinction, and excluding an absent parent without naming him as disinherited. | $730K |
| 02 | [James and Priya Okonkwo](clients/tier-1-foundational/02-okonkwo/) | Married couple, young family, standard plan | The standard couple: joint planning with two sets of agents, a pet trust, keeping each spouse's family on the right side, Nigerian and Indian naming conventions. | $2.4M |
| 03 | [Sandra and Diane Chen-Whitfield](clients/tier-1-foundational/03-chen-whitfield/) | Married lesbian couple, blended family, complex distributions | A non-biological parent, unequal shares with stated reasons, charitable giving with tax motives, a beneficiary-designation conflict, prior documents to revoke, an immediate DPOA. | $2.3M |
| 04 | [Robert "Bobby" Fitzgerald](clients/tier-1-foundational/04-fitzgerald/) | Recently divorced man, prior trust complications | An unrevoked prior trust of uncertain status, beneficiary designations that contradict current wishes, a fuzzily remembered QDRO, a deliberately excluded sibling. | $1.7M |
| 05 | [Marcus and Andre Williams-Park](clients/tier-1-foundational/05-williams-park/) | Married gay couple, no children, charitable focus | Chosen family, estrangement from blood relatives with legal consequences, a small business succession, heavy charitable giving, a domestic partnership followed by marriage. | $1.5M |
| 06 | [Linda Johansson](clients/tier-1-foundational/06-johansson/) | Widowed grandmother, multi-generational planning | A discretionary trust for a child with substance-use issues without punitive language, restatement versus revocation, a property that fell out of the trust, IRA designations to align. | $2.8M |
| 07 | [Tomás Reyes](clients/tier-1-foundational/07-reyes/) | Single young professional, simple plan, first-time client | The simplest end of the range: a nonbinary partner, cryptocurrency and app IP, an agent who is not the primary beneficiary, urgency from a parent who died without a plan. | $150K |
| 08 | [Patricia and George Nakamura](clients/tier-1-foundational/08-nakamura/) | Married couple nearing retirement, charitable legacy | Tax-aware giving (IRA to charity, Roth to family), a partner acknowledged outside the documents, different disposition wishes per spouse, outdated wills, a CPA's vocabulary. | $3.3M |
| 09 | [Raymond "Ray" Delacroix](clients/tier-1-foundational/09-delacroix/) | Older single gay man, limited support network, professional fiduciary | No viable personal fiduciary: a professional fiduciary to be named, a trust protector over them, compensation and replacement terms, a named collection as a bequest, institutions as backup fiduciaries. | $1.3M |

`COVERAGE.md` shows the same set by dimension, and lists what the nine do **not** cover.

## Wealth tiers

The tier a client sits in decides what the planning is about, and therefore what the client tests. The tiers are drawn by what changes in the planning, with net worth as the rough guide. The boundaries are relative to the federal estate tax exemption ($15M per person in 2026, indexed), not fixed dollars.

| Tier | Folder | Rough range | What defines it | Clients |
|---|---|---|---|---|
| 1 | [`clients/tier-1-foundational/`](clients/tier-1-foundational/) | Up to about $3.5M | No tax exposure. The plan is the core document set; the hard parts are people. | 01 to 09 |
| 2 | [`clients/tier-2-affluent/`](clients/tier-2-affluent/) | About $3.5M up to the exemption | Still non-taxable, but no longer comfortably. Multiple properties, a closely held business, concentrated stock, large retirement accounts. | none yet |
| 3 | [`clients/tier-3-taxable/`](clients/tier-3-taxable/) | The exemption up to about $50M | Federal estate tax is a real cost. Planning is tax-driven and the attorney works alongside a CPA and advisor. | none yet |
| 4 | [`clients/tier-4-ultra-high-net-worth/`](clients/tier-4-ultra-high-net-worth/) | Above about $50M | Family office or on the way to one. Multi-generational governance, several jurisdictions, often international family or assets. | none yet |

Each tier folder's README describes the tier in full: what defines it, what the planning turns on, what a client there tests that the tier below does not, and which gaps it would most usefully fill first. `clients/README.md` has the placement rule for borderline cases. Numbering runs across the whole set, so the next client is 10 whichever tier it joins.

## How a client is organised

```
clients/tier-1-foundational/02-okonkwo/
  README.md                          who they are, why they exist, what is here
  profile.md                         demographics, family, assets, goals, prior legal context
  interview/
    transcript.md                    the simulated interview, with the designer's notes at the top   <- the authority
    transcript-dialogue-only.md      the same, notes removed, for feeding to a system
    answer-key.md                    what a correct reading must find, and the traps set on purpose
    answer-key.json                  the same, structured, for scoring
  intake.md                          what the client returned on the follow-up form ([SYNTH] marks invented values)
  documents/                         the papers a real client brings: empty to start, README says what belongs
  recordings/                        where an interview was spoken aloud and captured (01 only, so far)
```

**Which file is the authority.** The transcript is the record of what the client said. The profile is where the client started, and the interview may add to it or contradict what the client half-remembers. The answer key is derived from the transcript and every line traces to it. The intake is what the client supplied afterwards; **transcript plus intake is the complete data set a finished plan should reflect.**

## How to use it

- **To test extraction** (reading a conversation into structured facts): feed `interview/transcript-dialogue-only.md` to the system and score against `interview/answer-key.json`. The answer key's last section lists the traps each transcript sets on purpose.
- **To test drafting** (producing documents from the facts): the facts are `intake.md` plus the transcript; the document set the client wants is section 12 of `intake.md`.
- **To rehearse a live interview**: `profile.md` is enough to play the client. Where a `recordings/` folder exists, the interview has been spoken once and need not be again.
- **To test document reading**: nothing yet. Each `documents/` folder is empty and its README says what should go there.

## Jurisdiction

**All nine clients are California residents interviewed by a California attorney, and the plans they expect are California plans**: a revocable living trust with a pour-over will, a durable power of attorney, an advance health-care directive, a HIPAA authorization, and California community-property questions throughout. The family facts, the assets and the wishes are portable; the intake's document list and the answer key's plan expectations are not, and a system under test in another state should be scored on the facts rather than on the California deliverables.

Every client's `README.md` carries `jurisdiction:` in its front matter. A client from another state is welcome; say in the profile what differs and why it matters there.

## Coverage and gaps

`COVERAGE.md`. The short version: no special-needs beneficiary, no non-citizen spouse, no second marriage with children on both sides, no taxable estate, no business with partners, no capacity question, nobody over 85, no out-of-state property, no client who speaks through an interpreter, and no documents at all yet. Several of those gaps are what appears when wealth moves up a tier, so tiers 2 to 4 would absorb most of the list; each tier README names the gaps it should fill first.

## Adding a client

`CONTRIBUTING.md`: which tier folder the client goes in, the layers in order, the derivation rule, the `[SYNTH]` tag, and the rules that keep the set usable. `docs/transcript-design-notes.md` is how the interviews are written to be realistically messy. `docs/profiles-overview.md` is the original overview the nine were designed from.

## Provenance and licence

Written for an AI-assisted estate planning platform between March and September 2026, and separated into this repository on 2026-10-03 so that other estate-planning practitioners can use and extend it. **Licence: [MIT](LICENSE).** Use it, change it, and redistribute it for any purpose, commercial or otherwise. The only condition is that copies carry the copyright and licence notice.
