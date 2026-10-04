# Supplemental Intake: Tomás Reyes

**Profile 7 / Reyes**
**Source:** Online intake form returned by client after initial interview, plus follow-up email confirming the health-care agent, the 401(k) designation and the stock-option paperwork.
**Use:** Ground-truth answer key for evaluating generated estate-planning documents. Combined with `interview/transcript-dialogue-only.md` and `interview/answer-key.md`, this represents the complete data set the documents should reflect.

> **Convention.** Values that appear in the transcript are repeated here for one-stop reference. Values that did **not** appear in the transcript and were synthesized for testing are tagged `[SYNTH]` so they can be edited or replaced. `profile` means the value comes from the client profile the voice agent plays (`profile.md`, Profile 7); `inferred` means it follows from the transcript without being said. Phone numbers use the (619) 555-XXXX reservation. Addresses and account details are fabricated and should not match real persons or institutions. Ash Taylor is nonbinary and uses they/them pronouns; every reference below does the same, and so must every document.

---

## 1. Principal

| Field | Value | Source |
|---|---|---|
| Full legal name | Tomás Reyes (no middle name) | transcript; "no middle name" [SYNTH] |
| Preferred name | Tom | transcript |
| Date of birth | November 22, 1996 (age 29) | profile |
| Place of birth | National City, California | [SYNTH] |
| SSN | 612-58-2267 | [SYNTH] |
| Marital status | Single, never married; unmarried partner (Ash Taylor), not a registered domestic partnership | transcript; registration status [SYNTH] |
| Citizenship | U.S. citizen | [SYNTH] |
| Domicile | California | inferred |
| Residence address | 875 Tenth Avenue, Unit 1406, San Diego, CA 92101 | [SYNTH] (East Village, renting, is correct per transcript) |
| Mailing address | same as residence | [SYNTH] |
| Mobile phone | (619) 555-7318 | [SYNTH] |
| Email | tom.reyes.ux@gmail.com | [SYNTH] |
| Employer | Tidepath Health, Inc. (healthcare-technology startup, privately held) | employer type transcript; name [SYNTH] |
| Occupation / title | UX Designer | transcript |
| Years with employer | about 3 | transcript |

## 2. Family

### Children

None. No children, living or deceased. *(transcript)*

### Partner

| Field | Ash Taylor | Source |
|---|---|---|
| Relationship | Partner, unmarried; together about three years; lives with the principal | transcript |
| Pronouns | they/them | transcript |
| Full legal name | Ash Taylor (no middle name; "Ash" is the legal first name, not a short form) | name transcript; the rest [SYNTH] |
| DOB | July 30, 1998 (age 28) | age transcript; date [SYNTH] |
| Address | same as principal | transcript |
| Phone | (619) 555-7319 | [SYNTH] |
| Email | ash.taylor.pm@outlook.com | [SYNTH] |
| Occupation | Product manager at a larger technology company | transcript |
| Role in plan | Primary DPOA agent; primary AHCD agent; HIPAA designee; second successor trustee; third-tier residuary beneficiary | transcript (DPOA, trustee, residue); AHCD profile + [SYNTH] follow-up; HIPAA [SYNTH] |
| Notes | Knows the password-manager master password. Has no default legal standing as an unmarried partner, which is why the principal chose them as immediate DPOA agent. Not close to their own family ("their story to tell"). | transcript |

### Other family

| Person | Gloria Reyes (mother) | Isabella Reyes (sister) |
|---|---|---|
| Role in plan | Primary residuary beneficiary; primary trustee; executor; successor DPOA agent; successor AHCD agent; HIPAA designee; current 401(k) beneficiary | Secondary residuary beneficiary; successor trustee; successor executor; HIPAA designee |
| Full legal name | Gloria Reyes (no middle name on file) | [SYNTH] | Isabella Reyes (no middle name on file) | [SYNTH] |
| DOB | April 8, 1969 (age 57) | age transcript; date [SYNTH] | February 14, 2000 (age 26) | age transcript; date [SYNTH] |
| Address | 2319 E. 16th Street, National City, CA 91950 | city transcript; street [SYNTH] | 4912 Mt. Etna Drive, Apt 3, San Diego, CA 92117 | city transcript; street [SYNTH] |
| Phone | (619) 555-4402 | [SYNTH] | (619) 555-6185 | [SYNTH] |
| Email | gloria.reyes.nc@gmail.com | [SYNTH] | isabella.reyes.teach@gmail.com | [SYNTH] |
| Notes | Widowed 2019; "doesn't have a lot of savings," which is why she is first in line. Loves Ash. | Teacher; close to the principal. |

Deceased family: **father, Rafael Reyes** [SYNTH name], born January 16, 1961 [SYNTH], died March 2019 [SYNTH month] of a sudden heart attack at age 58 *(year, cause and age: transcript)*. Died with no will or trust; administration took over a year and one bank refused to speak with Gloria because her name was not on the account. He is not a beneficiary or fiduciary and must not be recorded as a living person.

No stepchildren, no half-siblings, no other family material to the plan. [SYNTH]

## 3. Assets

| Asset | Institution / Detail | Approx. value | Ownership | Disposition |
|---|---|---|---|---|
| Retirement (401(k)) | Tidepath Health 401(k) plan, recordkeeper Vanguard [SYNTH], account ending 2208 [SYNTH] | $62,000 | Sole | **Beneficiary confirmed correct, no change needed:** primary beneficiary Gloria Reyes (confirmed by client per follow-up). No contingent beneficiary listed [SYNTH]. |
| High-yield savings | Ally Bank, account ending 6631 [SYNTH] | $28,000 | Sole | Retitle to trust (or pour over) |
| Checking | Ally Bank, account ending 6604 [SYNTH] | ~$4,500 [SYNTH] | Sole | Retitle to trust (or pour over) |
| Vested stock options | Tidepath Health, Inc., 2023 Equity Incentive Plan [SYNTH]; ~18,000 vested ISOs [SYNTH] | ~$45,000 at current (409A) valuation; **speculative**, company is private and has not gone public | Sole | Passes under the pour-over will to the trust. Per the plan document the client forwarded, options are not transferable during life, and the estate may exercise vested options for 12 months after death [SYNTH]. |
| Cryptocurrency | Coinbase account: Bitcoin (~$8,000) and Ethereum (~$4,000) [SYNTH split] | ~$12,000, fluctuates | Sole | No beneficiary designation mechanism. Follows the residuary chain; reached through the digital-assets provision and the credentials envelope. |
| Side-project app | UX research tool, in development, pre-revenue; source code in a private GitHub repository; not incorporated, no LLC [SYNTH] | undetermined; potential value | Sole, personally owned (built on own time and equipment; employment agreement's IP clause covers only company time and resources) | Follows the residuary chain. Employment agreement to be stored with the trust documents. |
| Digital art / NFTs | Generative-art portfolio; some pieces sold as NFTs; unsold and retained NFTs held in a self-custody MetaMask wallet [SYNTH] | ~$2,500 [SYNTH] | Sole | Follows the residuary chain. |
| Vehicle | 2018 Honda Civic, VIN 2HGFC2F59JH000731 [SYNTH], owned outright, no loan [SYNTH] | ~$15,000 [SYNTH] | Sole | Pour over to trust |
| Personal property | Computer equipment, furniture, standard household items | ~$6,000 [SYNTH] | Sole | Follows the residuary chain |

No real estate (rents). No business entity. No life insurance beyond a $50,000 employer group-term benefit [SYNTH], beneficiary Gloria Reyes [SYNTH]. No safe-deposit box. No pets. No charitable pledges.

Total approximate gross estate: **~$175,000** including the options at current valuation; **~$130,000** excluding the options and the IP, against the answer key's "~$150,000" (both are approximate).

## 4. Liabilities

| Item | Detail | Balance |
|---|---|---|
| Credit card | Chase Freedom [SYNTH] | ~$1,200 [SYNTH], paid in full monthly |
| Auto loan | None; Civic owned outright | none [SYNTH] |
| Student loans | None | none [SYNTH] |
| Lease | Apartment lease in both names (principal and Ash Taylor) | month-to-month obligation [SYNTH] |

## 5. Fiduciary designations

| Role | Primary | Successor / Backup |
|---|---|---|
| Trustee (during incapacity / after death) | Gloria Reyes | Isabella Reyes, then Ash Taylor |
| Executor of will | Gloria Reyes | Isabella Reyes, then Ash Taylor | [SYNTH alignment with trustee] |
| Guardian of minor children | none (no children) | none |
| DPOA agent (financial) | Ash Taylor | Gloria Reyes |
| AHCD agent (health care) | Ash Taylor | profile; confirmed [SYNTH] follow-up | Gloria Reyes | [SYNTH] |
| HIPAA-authorized recipients | Ash Taylor; Gloria Reyes; Isabella Reyes | [SYNTH] (Ash per profile) | none |

DPOA type: **Immediate**, effective on signing, not on incapacity. *(transcript)* The principal's reason, in his words: the day-to-day emergency role is Ash's; the "distribute his stuff" role is his mother's. The two chains are deliberately different.

## 6. Distribution plan

1. **Specific bequests:** None. *(transcript)*
2. **Residuary:** The whole remaining trust estate, including the digital assets, the app and the art, passes **outright to Gloria Reyes**. *(transcript)*
3. **First alternate:** If Gloria Reyes does not survive the principal, the whole residue passes **outright to Isabella Reyes**. *(transcript)*
4. **Second alternate:** If neither Gloria nor Isabella survives the principal, the whole residue passes **outright to Ash Taylor**. *(transcript)*
5. **No continuing trust** for any taker; every beneficiary is an adult. *(inferred)*
6. **If none of the three survives:** to the principal's heirs at law under California intestacy rules. [SYNTH; interview did not cover]
7. **401(k):** passes by beneficiary designation to Gloria Reyes, outside the trust, which aligns with the plan. *(transcript)*

## 7. Health-care directive preferences

- **Agent:** Ash Taylor, with Gloria Reyes as alternate. [SYNTH follow-up confirming the profile; the interview covered only the financial power, but the principal said "if I'm in the hospital, they can't make decisions for me" and that Ash should have the authority.]
- **End-of-life care:** Principal does **not** want life-sustaining treatment continued if he is in an irreversible coma, persistent vegetative state, or terminal condition with no reasonable expectation of recovery. Comfort care and pain management to be maintained. [SYNTH; interview did not cover]
- **Artificial nutrition / hydration:** Discontinue once curative treatment is withdrawn. [SYNTH]
- **Anatomical gifts:** Yes, consents to organ and tissue donation for transplantation or therapy. [SYNTH]
- **Primary physician designation:** None designated. [SYNTH]

## 8. Final disposition

- **Method:** Cremation. *(transcript)*
- **Service:** No elaborate funeral; "whatever is easiest and cheapest for my family." *(transcript)*
- **Authority over remains:** Ash Taylor, as health-care agent, in consultation with Gloria Reyes. [SYNTH; follows from naming Ash as AHCD agent, but please confirm]
- **Disposition of cremated remains:** No specific instructions. [SYNTH]

## 9. Charitable giving

None at this time. *(transcript)*

## 10. Digital assets

- **Password manager:** 1Password [SYNTH product]; everything is in it (Coinbase, GitHub, the NFT wallet). Ash Taylor knows the master password. *(transcript, except the product name)*
- **Credentials envelope:** Principal will prepare a sealed envelope with the master password and access instructions, stored with the trust documents. *(transcript)*
- **Cryptocurrency:** Coinbase (Bitcoin and Ethereum); two-factor authentication through an authenticator app on his phone, recovery codes in the password manager [SYNTH].
- **Code:** GitHub account, private repository for the app. *(transcript; "private" [SYNTH])*
- **NFTs:** self-custody wallet; seed phrase in the password manager [SYNTH].
- **Email:** Gmail (personal) [SYNTH]; work email handled by employer, not part of the estate.
- **Social media:** Instagram, LinkedIn [SYNTH].
- **Authority:** Trustee and DPOA agent are both granted access to all digital assets, accounts, wallets and electronic communications under the California RUFADAA (Probate Code §§ 870 to 884). *(transcript for both roles; statute [SYNTH inference, standard clause])*
- **Employment agreement:** copy to be kept in the same folder as the trust documents, to evidence personal ownership of the app. *(transcript)*

## 11. Prior legal context

- No prior wills, trusts, or codicils. *(transcript)*
- No prior marriages. *(profile)*
- No domestic-partnership registration. [SYNTH]
- No active litigation, judgments, or liens against the principal. [SYNTH]
- Father died intestate in 2019; the year-long administration is the principal's motivation. *(transcript)*

## 12. Document deliverables for this matter

The completed package should include:

1. **Revocable Living Trust** ("The Tomás Reyes Revocable Living Trust dated [execution date]" [SYNTH name]): Tomás as initial trustee, Gloria as successor, Isabella as second successor, Ash as third; residue outright to Gloria, then Isabella, then Ash; digital-assets provision.
2. **Certification of Trust**: short-form summary suitable for delivery to financial institutions (Ally, Coinbase).
3. **Pour-Over Will**: Tomás as testator, Gloria as executor, Isabella then Ash as alternates; no guardian nomination (no children).
4. **Distribution / Personal Property Memorandum**: no current specific items; available for future tangible-property memos.
5. **Immediate Durable Power of Attorney** (financial): Ash primary, Gloria successor; express digital-assets authority.
6. **Advance Health-Care Directive**: Ash primary, Gloria alternate; preferences in §7 above.
7. **HIPAA Authorization**: designees in §5 above.

Note: single grantor, so only one set of documents is required. Ash is a partner, not a spouse and not a principal.

---

## Editor checklist

Before this file is treated as ground truth for an attorney-agent run, please review and adjust the following items, all of which were synthesized:

- [ ] All `[SYNTH]` addresses, phones, emails, DOBs, account numbers, VIN and SSNs.
- [ ] Legal names recorded with **no middle names** (Tomás, Gloria, Isabella, Ash). Kept that way on purpose so the package key's name patterns ("Tomás Reyes", "Gloria Reyes", "Ash Taylor") still match; adding a middle name will change what the documents print.
- [ ] **AHCD agent (§5, §7):** Ash primary is from the profile, not the transcript, which covered only the financial power. Resolved here as a follow-up confirmation [SYNTH]; the package key already expects Ash.
- [ ] **AHCD alternate (§5):** Gloria, mirroring the DPOA chain [SYNTH].
- [ ] **HIPAA designees (§5):** Ash, Gloria and Isabella [SYNTH]; the interview named none.
- [ ] **Executor chain (§5):** Gloria, then Isabella, then Ash, aligned with the trustee chain [SYNTH]. The package key expects Gloria as personal representative.
- [ ] **Authority over remains (§8):** given to Ash as health-care agent [SYNTH]. A real choice between the partner and the mother; the interview only said "cremation, keep it simple."
- [ ] **Ultimate taker (§6.6):** heirs at law if Gloria, Isabella and Ash all fail to survive [SYNTH].
- [ ] **401(k) contingent beneficiary (§3):** none listed [SYNTH]. Whether to advise adding Isabella is the attorney's call; the primary designation is confirmed correct and needs no change.
- [ ] **Stock-option terms (§3):** ISO count, non-transferability and the 12-month post-death exercise window [SYNTH].
- [ ] AHCD end-of-life and anatomical-gift preferences (§7): inferred, not interviewed.
- [ ] Trust name (§12): "The Tomás Reyes Revocable Living Trust" [SYNTH]; the interview gave no name.
- [ ] Group-term life insurance of $50,000 naming Gloria (§3) [SYNTH]; delete if the test should hold only the transcript's assets.
- [ ] Father's name and date of death (§2) [SYNTH].
- [ ] **Profile vs transcript:** the profile calls Ash Tomás's "girlfriend"; the transcript says "partner" and they/them throughout. This file follows the transcript. The profile's "Orientation" line is not recorded here; it is not an intake fact.
- [ ] **Attorney decisions:** none. the originating project's typed answer key (not included here) has an empty `DECISIONS`, and `docs/plans/client_decisions_proposal.md` proposes none for Reyes; nothing in this file stands in for one.
