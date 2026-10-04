# Extraction Answer Key — Marcus & Andre Williams-Park

## Extraction Answer Key

### People & Relationships

- **Marcus Williams** — Co-principal. Age 44, born October 15, 1981. Architect at Gensler (8 years). Identifies as gay.
- **Andre Park** — Co-principal. Age 47, born April 2, 1979. Owns restaurant "The Porch" in Hillcrest (sole proprietorship, 9 years). Identifies as gay. Estranged from biological family 13+ years.
- **Married:** 2017. Together since 2011 (Andre corrects Marcus who says 2012). Reside in Mission Hills, San Diego, CA.
- **Helen Williams** — Marcus's mother. Age 72. Lives in San Diego. Father deceased (~10 years ago). Receives $25,000 if living. Treats Andre like a son.
- **Denise Williams** — Marcus's sister. Age 40. Lives in Sacramento. Receives 40% of trust remainder. Second successor trustee. Marcus's successor DPOA agent. Backup pet caretaker.
- **Lisa Nakamura** — Andre's best friend / chosen family. Age 49. Lives in San Diego. Andre's emergency contact for everything. Receives $50,000 specific bequest. Successor trustee. Andre's successor DPOA agent. Primary pet caretaker.
- **Miguel Reyes** — Andre's sous chef at The Porch. 12 years at the restaurant (started as dishwasher). "Like a younger brother." Receives the restaurant and its assets. Lives in San Diego.
- **Andre's biological family** — Parents, brother. Estranged 13+ years. Did not accept Andre's coming out. No contact. To be explicitly excluded in trust language. No formal waiver of inheritance rights has occurred.
- **Bowie** — Dog, age 5. Rescue.
- **Prince** — Dog, age 4. Rescue.

### Assets

- **Townhouse:** Mission Hills, ~$950K, mortgage ~$320K. Joint title.
- **The Porch (restaurant):** Sole proprietorship. Andre owns all equipment, inventory, brand. Leased space. Estimated value ~$180K. No operating agreement. No formal succession plan. Business accounts all in Andre's name.
- **Marcus's 401(k):** ~$390,000 at Gensler. Beneficiary believed to be Andre (set up after marriage).
- **Andre's SEP IRA:** ~$85,000. **FLAG:** Beneficiary might be Lisa (set up before marriage). Needs verification.
- **Joint Savings:** ~$60,000 at local credit union.
- **Marcus's Brokerage:** ~$150,000 at Vanguard (individual account).
- **Vehicles:** 2021 Jeep Wrangler (Andre's), 2019 Toyota Tacoma (Marcus's).

### Distribution Plan

- Everything to surviving spouse first.
- After both have passed:
  - The Porch restaurant and all assets to Miguel Reyes. If Miguel declines, sell and add proceeds to trust remainder.
  - $30,000 pet trust for Bowie, Prince, and future pets.
  - $50,000 to Lisa Nakamura.
  - $25,000 to Helen Williams (if living).
  - Remainder: 60% to charities (25% San Diego LGBT Community Center, 25% Trevor Project, 10% local LGBTQ youth scholarship fund), 40% to Denise Williams.

### Fiduciary Designations

- **Trustee:** Surviving spouse. Successor: Lisa Nakamura. Second successor: Denise Williams.
- **Marcus's DPOA Agent:** Andre. Successor: Denise.
- **Andre's DPOA Agent:** Marcus. Successor: Lisa.
- **DPOA Type:** Immediate for both. Andre's specific concern: preventing any window for biological family intervention during incapacity.

### Prior Legal Context

- **FLAG:** Basic wills from 2013, drafted by a law school friend. Outdated. Left everything to each other. Need to be revoked.
- Andre's biological family has not formally waived inheritance rights. Trust should include explicit exclusion language.
- **FLAG:** Andre's SEP IRA beneficiary may be Lisa (pre-marriage designation). Needs verification and likely update to Andre or the trust.
- Restaurant has no operating agreement or formal succession plan — business continuity risk during incapacity or death.

### Special Provisions

- **Pet trust:** $30,000 for Bowie, Prince, and future pets. Lisa primary caretaker, Denise backup.
- **Restaurant succession:** The Porch to Miguel Reyes, free and clear. If declined, sell and add to remainder. Attorney suggested separately exploring LLC formation and operating agreement for business continuity (not part of estate plan but related).
- **Biological family exclusion:** Andre wants explicit trust language intentionally omitting unnamed biological family members. Not a formal disinheritance — a clear statement of intentional omission.
- **Advance healthcare directives:** Both want to prepare these. Andre specifically wants no life-sustaining treatment if no reasonable chance of recovery. Marcus agrees.
- **Body disposition:** Both want cremation. Andre prefers Balboa Park (rose garden). Marcus prefers Torrey Pines. Both stated as soft preferences, not definitive.
- **Charitable giving:** 60% of remainder to three organizations. Significant giving relative to estate size.

---

## Conversational Challenges for Capture Engine

- **Together since date corrected by Andre.** Marcus says 2012, Andre corrects to 2011. System should capture 2011 and should ideally note the correction as a data quality signal.
- **Chosen family concept.** Lisa Nakamura fills a traditional family role (emergency contact, fiduciary, caretaker) without any legal or biological relationship. System must recognize her significance from context rather than from a family label.
- **Biological family described through estrangement.** Andre's parents and brother are mentioned only as people who are excluded. No names, no ages, no locations. System must capture the estrangement, the duration (13+ years), and the explicit exclusion intent.
- **Restaurant valuation is uncertain.** Andre says "maybe $180,000" and notes it's hard to value a restaurant. System should capture both the estimate and the uncertainty.
- **Restaurant succession has conditions.** Miguel gets the restaurant — but only if he wants it. If he declines, sell and add to remainder. System must capture both the primary intent and the fallback.
- **Pet trust covers future pets.** Not just Bowie and Prince — "and any future dogs we might have." System must capture this broader scope.
- **Advance healthcare directive raised by Andre at the end.** This is a separate document type, not part of the trust. System should capture the wish but categorize it correctly.
- **Multiple charity allocations with specific percentages.** 25%, 25%, 10% to three different organizations. System must keep these distinct and correctly allocated.
- **SEP IRA beneficiary uncertainty.** Andre says "might be Lisa." System should flag as unknown/needs verification, not assume.
- **2013 wills dismissed as "garbage."** System should capture their existence and the need to revoke them, regardless of quality assessment.
