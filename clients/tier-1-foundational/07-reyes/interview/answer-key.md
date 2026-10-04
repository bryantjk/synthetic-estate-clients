# Extraction Answer Key — Tomás Reyes

## Extraction Answer Key

### People & Relationships

- **Tomás "Tom" Reyes** — Principal. Age 29, born November 22, 1996. UX designer at a healthcare tech startup (3 years). Resides in East Village, San Diego, CA (renting, shared with Ash). Single. Motivated by father's death without an estate plan.
- **Ash Taylor** — Partner (nonbinary, they/them pronouns). Age 28. Product manager at a tech company. Lives with Tomás. Not married. Unmarried partner with no default legal standing. Primary DPOA agent. Knows password manager master password.
- **Gloria Reyes** — Mother. Age 57. Lives in National City, CA. Primary beneficiary. Primary trustee. Successor DPOA agent. 401(k) beneficiary (current, aligned with wishes).
- **Isabella Reyes** — Sister. Age 26. Lives in San Diego. Teacher. Secondary beneficiary. Successor trustee.
- **Father (deceased)** — Unnamed in conversation. Died 2019, heart attack, age 58. No estate plan. The difficult aftermath is Tomás's primary motivation for planning. Had accounts his wife couldn't access.

### Assets

- **401(k):** ~$62,000 through employer. Beneficiary: Gloria (current, correct, aligned with wishes).
- **Savings:** ~$28,000 in high-yield savings at Ally Bank.
- **Stock Options:** ~$45,000 vested options at startup (speculative value — company hasn't gone public).
- **Cryptocurrency:** ~$12,000 in Bitcoin and Ethereum on Coinbase. No traditional beneficiary designation mechanism. Access via password manager (Ash knows master password).
- **Vehicle:** 2018 Honda Civic.
- **Digital Assets — App:** UX research tool in development. Not generating revenue. Owned personally (verified against employment agreement IP clause). Has potential future value.
- **Digital Assets — Art:** Generative art portfolio, some pieces sold as NFTs. Hobby with some monetary value.
- **Personal Property:** Computer equipment, standard household items.
- **Real Estate:** None (rents).
- **Total Net Worth:** ~$150,000 (excluding speculative stock options and digital assets).

### Distribution Plan

- Primary: Everything to Gloria (mother).
- Secondary: Everything to Isabella (sister), if Gloria has predeceased.
- Tertiary: Everything to Ash (partner), if both Gloria and Isabella have predeceased.
- No specific bequests. No charitable giving. Digital assets follow the same distribution chain.

### Fiduciary Designations

- **Trustee:** Gloria. Successor: Isabella. Second successor: Ash. (Note: Tomás's reasoning — mom handles the "distribute his stuff" role.)
- **DPOA Agent:** Ash. Successor: Gloria. (Note: Different from trustee chain. Ash is DPOA agent because they're local, know the finances, and lack default legal standing as unmarried partner. Tomás's reasoning — Ash handles the "day-to-day emergency" role.)
- **DPOA Type:** Immediate. Chosen because Ash has no spousal presumption — immediate authority removes legal barriers for an unmarried partner.

### Prior Legal Context

- No prior estate planning documents.
- No prior marriages.
- Father died in 2019 without any estate plan — resulted in a year-long process to sort out accounts. One bank refused to speak with Gloria because she wasn't on the account. This experience is the primary motivation.
- 401(k) beneficiary lists Gloria — aligned with current wishes, no change needed.

### Special Provisions

- **Digital assets provision:** Trust should specifically authorize trustee and DPOA agent to access digital accounts, crypto wallets, and online assets. Password manager credentials to be stored in sealed envelope with trust documents.
- **Employment agreement:** Verifies app IP belongs to Tomás personally. Should be stored with estate planning documents.
- **Body disposition:** Cremation. No elaborate funeral. "Whatever is easiest and cheapest for my family."
- **Charitable giving:** None at this time.
- **Pet provisions:** None (no pets).

---

## Conversational Challenges for Capture Engine

- **Nonbinary pronouns throughout.** Ash uses they/them pronouns, introduced at minute 4. Every reference to Ash throughout the transcript uses they/them. The extraction must use correct pronouns in the profile and never misgender Ash. This is a critical inclusivity test.
- **Preferred name vs. legal name.** Tomás introduces himself as "Tom" immediately. The system should capture both the legal name (Tomás Reyes) and the preferred name (Tom) and use them appropriately.
- **Ash's last name given at the very end.** Tomás says "Ash" throughout the entire conversation. "Ash Taylor" only appears in the last minute when Tomás provides the full name unprompted. System must retroactively associate all prior "Ash" references with "Ash Taylor."
- **Different fiduciary chains with explicit reasoning.** Trustee: Gloria → Isabella → Ash. DPOA: Ash → Gloria. Tomás explains the logic clearly ("day-to-day emergency" vs. "distribute his stuff"). System must keep these distinct and capture the reasoning.
- **Digital assets described informally.** Tomás describes crypto, an app, and digital art in casual language. The system must recognize these as distinct asset categories: cryptocurrency (financial asset), intellectual property (the app), and digital art/NFTs (creative asset with monetary value).
- **Stock options described with uncertainty.** Tomás says they're "worth about $45,000 at the current valuation, but honestly who knows." System should capture both the value and the uncertainty — these are speculative assets.
- **Father's death is emotional context with planning significance.** The details about the father's lack of planning (banks refusing to talk to Gloria, year-long process) explain Tomás's urgency and his specific concern about legal authority. System should capture both the factual details and the motivational context.
- **Unmarried partner authority is a key planning concern.** Tomás repeatedly emphasizes that Ash has "zero standing" legally. The choice of immediate DPOA is tied to this concern. System must capture the relationship status and its legal implications.
- **401(k) beneficiary is already correct.** Unlike Bobby Fitzgerald's situation where beneficiaries needed changing, Tomás's 401(k) correctly lists Gloria and aligns with his wishes. System must note this as "confirmed correct, no change needed."
- **Crypto access path is informal.** Ash knows the password manager master password, but there's no formal documentation. The plan calls for a sealed envelope with credentials. System should capture both the current informal arrangement and the planned formalization.
