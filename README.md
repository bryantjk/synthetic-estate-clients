# Synthetic estate-planning clients

Nine invented clients, each with a profile, a simulated attorney interview, an answer key for what the interview contains, and the follow-up intake form the client returned afterwards. Built to test systems that read estate-planning conversations and produce estate plans; usable by anyone working on the same problem.

Everything here is fabricated. No client, family member, address, employer or account is real.

## The nine

| # | Client | Shape | Built to test | Net worth |
|---|---|---|---|---|
| 01 | [Maria Elena Vega](clients/01-vega/) | Single mother, straightforward plan | Guardianship, minor beneficiaries with age conditions, the guardian/trustee distinction, and excluding an absent parent without naming him as disinherited. | $730K |
| 02 | [James and Priya Okonkwo](clients/02-okonkwo/) | Married couple, young family, standard plan | The standard couple: joint planning with two sets of agents, a pet trust, keeping each spouse's family on the right side, Nigerian and Indian naming conventions. | $2.4M |
| 03 | [Sandra and Diane Chen-Whitfield](clients/03-chen-whitfield/) | Married lesbian couple, blended family, complex distributions | A non-biological parent, unequal shares with stated reasons, charitable giving with tax motives, a beneficiary-designation conflict, prior documents to revoke, an immediate DPOA. | $2.3M |
| 04 | [Robert "Bobby" Fitzgerald](clients/04-fitzgerald/) | Recently divorced man, prior trust complications | An unrevoked prior trust of uncertain status, beneficiary designations that contradict current wishes, a fuzzily remembered QDRO, a deliberately excluded sibling. | $1.7M |
| 05 | [Marcus and Andre Williams-Park](clients/05-williams-park/) | Married gay couple, no children, charitable focus | Chosen family, estrangement from blood relatives with legal consequences, a small business succession, heavy charitable giving, a domestic partnership followed by marriage. | $1.5M |
| 06 | [Linda Johansson](clients/06-johansson/) | Widowed grandmother, multi-generational planning | A discretionary trust for a child with substance-use issues without punitive language, restatement versus revocation, a property that fell out of the trust, IRA designations to align. | $2.8M |
| 07 | [Tomás Reyes](clients/07-reyes/) | Single young professional, simple plan, first-time client | The simplest end of the range: a nonbinary partner, cryptocurrency and app IP, an agent who is not the primary beneficiary, urgency from a parent who died without a plan. | $150K |
| 08 | [Patricia and George Nakamura](clients/08-nakamura/) | Married couple nearing retirement, charitable legacy | Tax-aware giving (IRA to charity, Roth to family), a partner acknowledged outside the documents, different disposition wishes per spouse, outdated wills, a CPA's vocabulary. | $3.3M |
| 09 | [Raymond "Ray" Delacroix](clients/09-delacroix/) | Older single gay man, limited support network, professional fiduciary | No viable personal fiduciary: a professional fiduciary to be named, a trust protector over them, compensation and replacement terms, a named collection as a bequest, institutions as backup fiduciaries. | $1.3M |

`COVERAGE.md` shows the same set by dimension, and lists what the nine do **not** cover.

## How a client is organised

```
clients/02-okonkwo/
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

`COVERAGE.md`. The short version: no special-needs beneficiary, no non-citizen spouse, no second marriage with children on both sides, no taxable estate, no business with partners, no capacity question, nobody over 85, no out-of-state property, no client who speaks through an interpreter, and no documents at all yet.

## Adding a client

`CONTRIBUTING.md`: the layers in order, the derivation rule, the `[SYNTH]` tag, and the rules that keep the set usable. `docs/transcript-design-notes.md` is how the interviews are written to be realistically messy. `docs/profiles-overview.md` is the original overview the nine were designed from.

## Provenance and licence

Written for an AI-assisted estate planning platform between March and September 2026 by the team at Lexploration, and separated into this repository on 2026-10-03 so that other estate-planning practitioners can use and extend it. **Licence: not yet chosen.** Until one is, treat the set as shared with the contributing attorneys for their own development and testing, and ask before publishing it further.
