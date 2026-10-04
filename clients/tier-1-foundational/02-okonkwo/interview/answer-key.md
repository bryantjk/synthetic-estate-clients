# Extraction Answer Key — James & Priya Okonkwo

## Extraction Answer Key

### Initial Knowledge
  --------------- -------------------------------------------------------
  James Okonkwo (Husband)           Software engineer at Qualcomm. 

  Priya (Wife)           Age 39 / born August 22, 1986. Pediatrician in private practice. 

  Married         2015

  Residence       Own a home in Carmel Valley, San Diego, CA

  Orientation     Heterosexual
  --------------- -------------------------------------------------------

### Interview Notes

This is the "standard" married couple scenario — two working professionals with young children, a house, retirement accounts, and a dog. The plan is relatively straightforward: everything to the surviving spouse, then to the kids in trust. The primary complexity is in guardianship designations and the pet trust. This transcript tests whether the system handles a clean, uncomplicated scenario accurately without inventing complexity that isn't there.

Both spouses participate. Priya tends to lead on decisions while James defers but occasionally adds specifics. The conversation about guardianship reveals family dynamics across both sides — each spouse's family is in a different city, creating logistical considerations. Cross-cultural naming conventions (Nigerian and Indian names) test the system's ability to handle non-Western name patterns.


### People & Relationships

- **James Okonkwo** — Co-principal. Age 41, born March 3, 1985. Software engineer at Qualcomm (8+ years). Resides in Carmel Valley, San Diego, CA.
- **Priya Okonkwo** — Co-principal. Age 39, born August 22, 1986. Pediatrician in private practice (sole proprietorship, Carmel Valley). 
- **Married:** 2015. 
- **Zara Okonkwo** — Daughter. Age 8.
- **Kiran Okonkwo** — Son. Age 5.
- **James's parents** — Both living, in their 70s (father 76, mother 73), in Atlanta, GA.
- **Adaeze (Ada) Okonkwo** — James's sister. Age 38. Lives in Atlanta. Not married, no children. Backup guardian. Successor trustee. James's successor DPOA agent. Backup pet caretaker. Kids call her "Auntie Ada."
- **Priya's parents** — Both living, late 60s (father 69, mother 67), in San Jose, CA.
- **Ravi** — Priya's brother. Age 43. Lives in San Jose. Wife: Meena. Has two children (ages similar to Zara and Kiran). Primary guardian (with Meena). Primary trustee. Priya's successor DPOA agent. Family takes Biscuit.
- **Meena** — Ravi's wife. No last name given. Primary guardian (with Ravi).
- **Biscuit** — Dog (golden retriever). Age 3. $15,000 pet trust. Ravi's family primary caretaker, Adaeze backup.

### Assets

- **Primary Residence:** Carmel Valley house, purchased 2019, ~$1.2M value, ~$650K mortgage. Joint title.
- **James's 401(k):** ~$420,000 at Qualcomm. Beneficiary believed to be Priya (needs verification).
- **Priya's SEP IRA:** ~$310,000. Beneficiary believed to be James (needs verification).
- **Joint Savings:** ~$95,000 at Wells Fargo.
- **Joint Brokerage:** ~$180,000 at Schwab.
- **529 Plans:** ~$35,000 each for Zara and Kiran. Successor beneficiary designations need verification.
- **Life Insurance:** James: $1M term policy. Priya: $750K term policy. Both through Northwestern Mutual. Beneficiaries believed to be each other (needs verification).
- **Vehicles:** 2022 Tesla Model Y, 2020 BMW X3.
- **Priya's Practice:** Sole proprietorship pediatric practice. No tangible assets (equipment leased). Would wind down if Priya passed. Not an estate planning asset.

### Distribution Plan

- Everything to surviving spouse outright, no conditions.
- If both have passed: everything in trust for Zara and Kiran equally.
- Trustee discretion for health, education, and support until age 28.
- Full outright distribution at age 28.
- $15,000 pet trust for Biscuit.
- No charitable giving.
- No specific personal property bequests.

### Fiduciary Designations

- **Guardian:** Ravi and Meena. Backup: Adaeze.
- **Trustee:** Surviving spouse. Successor: Ravi. Second successor: Adaeze.
- **James's DPOA Agent:** Priya. Successor: Adaeze.
- **Priya's DPOA Agent:** James. Successor: Ravi.
- **DPOA Type:** Springing for both.

### Prior Legal Context

- No prior estate planning documents.
- No prior marriages for either spouse.
- Priya's medical practice is a sole proprietorship with no significant tangible assets (equipment leased). Not a succession concern.

### Special Provisions

- **Pet trust:** $15,000 for Biscuit. Ravi's family primary caretaker, Adaeze backup.
- **Body disposition:** No strong preferences. Open to either cremation or burial. Defer to families' wishes at the time.
- **Charitable giving:** None at this time.

### Items Requiring Follow-Up

- **FLAG:** Beneficiaries on both life insurance policies need verification (believed to be each other).
- **FLAG:** Beneficiaries on James's 401(k) and Priya's SEP IRA need verification (believed to be each other with kids as contingent).
- **FLAG:** Successor beneficiary designations on both 529 plans need verification — may default to account owner's estate.

---

## Conversational Challenges for Capture Engine

- **Name variant: Adaeze vs. Ada.** James calls his sister "Ada," Priya provides the full name "Adaeze." The children call her "Auntie Ada." System must recognize all three as the same person.
- **Cross-cultural names.** Nigerian (Okonkwo, Adaeze, Zara, Kiran) and Indian (Priya, Ravi, Meena) names. System must handle these without confusion or mislabeling.
- **Straightforward scenario — system should not over-complicate.** Unlike the complex profiles, this is a clean, standard plan. The system should extract it accurately without inventing complexity (e.g., should not flag unequal distribution concerns when the plan is simply "equal to both kids").
- **Both spouses contribute information about different family members.** James provides his family details, Priya provides hers. System must correctly associate each person with the right spouse's side.
- **"We think" beneficiary uncertainty.** Priya says she's "pretty sure" about beneficiaries but can't confirm. System should flag all six accounts as needing verification rather than assuming.
- **Specific age for distribution (28).** Priya emphasizes "specifically twenty-eight" with a personal reason. System should capture the number precisely — not default to 25 or 30.
- **529 plans raised at the very end by James.** An afterthought that reveals a potential issue (successor beneficiary designations). System must capture this late addition.
- **Priya's practice is NOT an asset to plan for.** She explicitly says it would "just wind down." System should note the practice exists but should not treat it as a distributable asset.
- **Dog mentioned via jacket hair.** Biscuit is first mentioned through a visual cue (golden retriever hair). In a real audio scenario this contextual detail might not be captured, but the name and details that follow should be.
