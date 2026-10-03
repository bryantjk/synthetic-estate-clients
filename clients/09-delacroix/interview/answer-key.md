# Extraction Answer Key — Raymond "Ray" Delacroix

## Extraction Answer Key

### People & Relationships

- **Raymond "Ray" Delacroix** — Principal. Age 74, born March 17, 1952. Retired librarian (San Diego Public Library, 35 years). Single (never married). Resides in Bankers Hill, San Diego, CA. Partner Walter passed 2018.
- **Walter Hartman** — Deceased partner. Together 28 years. Died 2018 (stomach cancer). Amateur painter. Estranged from his own family. Never married Ray. No estate plan — his death without legal protections is Ray's primary motivation. Surname "Hartman" surfaces in the named collection bequest.
- **Gerald Delacroix** — Brother. Age 78. Lives in memory care facility in Baton Rouge, LA. Advanced dementia. Cannot serve in any fiduciary capacity.
- **Paul Delacroix** — Nephew (Gerald's son). Age 50. Lives in Houston, TX. Cordial but not close (Christmas cards, occasional calls). Receives $10,000.
- **Marie Delacroix-Tran** — Niece (Gerald's daughter). Age 47. Lives in Baton Rouge, LA. Same relationship level as Paul. Receives $10,000.
- **Evelyn Marsh** — Closest friend. Age 71. Former library colleague. Weekly lunch (Tuesdays). Has health issues (hip replacement, early macular degeneration). Explicitly declined trustee/agent role. Potential trust protector (light-touch supervisory role). Receives $10,000.
- **Joseph Kim** — Neighbor. Age 45. Checks on Ray regularly, helps with household tasks. Explicitly declined legal responsibility. Will take Cleo if Ray passes. Receives $5,000.
- **Professional Fiduciary** — To be named. Will serve as trustee, executor, financial DPOA agent, and healthcare DPOA agent. Trust includes compensation provisions and replacement mechanism.
- **Cleo** — Cat, age 9. $15,000 pet trust. Joseph primary caretaker, San Diego Humane Society backup.

### Assets

- **Condo:** Bankers Hill, ~$580K, owned free and clear. In Ray's name individually (not in any trust). Needs to be titled into the new trust.
- **Traditional IRA:** ~$420,000 (rollover from CalPERS-adjacent plan). **FLAG:** Beneficiary almost certainly still lists Walter (deceased). Never updated. No contingent beneficiary. Would go to estate and through probate if not updated. Urgent.
- **CalPERS Pension:** ~$4,100/month.
- **Social Security:** ~$2,800/month.
- **Savings:** ~$95,000 at San Diego County Credit Union. No POD designation.
- **Brokerage:** ~$185,000 at Schwab. No TOD designation.
- **Life Insurance:** None (employer policy lapsed at retirement).
- **Vehicle:** 2019 Toyota Camry.
- **Personal Property — Books:** Rare first editions, ~$15,000 value. Bequeathed to San Diego Public Library as "Delacroix-Hartman Collection" (named collection).
- **Personal Property — Art:** Walter's paintings (oils, watercolors). Modest market value. Bequeathed to San Diego Public Library for display in central branch.

### Distribution Plan

- Walter's artwork to San Diego Public Library (for display at central branch).
- Rare book collection to San Diego Public Library as the "Delacroix-Hartman Collection."
- $15,000 pet trust for Cleo.
- $10,000 each to Paul Delacroix, Marie Delacroix-Tran, and Evelyn Marsh.
- $5,000 to Joseph Kim.
- Remainder: 50% San Diego LGBT Community Center, 30% San Diego Public Library Foundation, 20% Walter Hartman AIDS Memorial Fund (at San Diego Foundation).

### Fiduciary Designations

- **Trustee:** Professional fiduciary (to be named). Trust includes compensation provisions and replacement mechanism.
- **Trust Protector:** Evelyn Marsh. Backup: Executive director of San Diego LGBT Community Center (institutional capacity). Light-touch supervisory role — can remove/replace professional fiduciary.
- **Executor:** Professional fiduciary (same person as trustee).
- **DPOA Agent (financial and healthcare):** Professional fiduciary (same person). Springing.
- **DPOA Type:** Springing.

### Prior Legal Context

- **No prior estate planning documents whatsoever.** No trust, no will, no powers of attorney. First time.
- Walter died in 2018 with no estate plan. Ray had to petition for conservatorship — costly, months-long, traumatic. Walter's estranged brother contested Ray's involvement in medical decisions. This experience is the central motivation for Ray's planning.
- **FLAG:** IRA beneficiary almost certainly lists Walter (deceased, never updated). No contingent beneficiary. Would go to estate/probate. Urgent update needed.
- **FLAG:** Credit union savings has no POD designation.
- **FLAG:** Schwab brokerage has no TOD designation.
- **FLAG:** Condo has no transfer-on-death deed (will be titled into trust).

### Special Provisions

- **Professional fiduciary:** "To be named" placeholder. Serves in all fiduciary roles (trustee, executor, DPOA agent). Trust includes reasonable compensation provisions and replacement process.
- **Trust protector:** Evelyn Marsh with institutional backup. Supervisory role only — authority to remove and replace professional fiduciary if they fail in their duties.
- **Named collection bequest:** Rare books to SDPL as "Delacroix-Hartman Collection" — Ray's surname combined with Walter's surname. Library's head of special collections has been informally consulted.
- **Pet trust:** $15,000 for Cleo. Joseph Kim primary caretaker, San Diego Humane Society backup.
- **Body disposition:** Cremation. Primary: ashes scattered at Balboa Park botanical garden (meaningful location with Walter). Alternative: interment at Greenwood Memorial Park (if scattering not permitted).
- **Charitable giving:** Majority of estate goes to three charities. The AIDS memorial fund is specifically in Walter's name.

---

## Conversational Challenges for Capture Engine

- **Walter's surname revealed late.** Ray refers to "Walter" throughout. "Hartman" only appears when Ray mentions the "Delacroix-Hartman Collection" at minute 21. System must retroactively associate the surname with all prior Walter references.
- **Professional fiduciary is a placeholder.** The system must handle "to be named" — this is not a person who exists yet in the data model. It's a role to be filled.
- **Trust protector is an unfamiliar concept.** The system needs to capture this as a distinct role separate from trustee — supervisory authority, not management authority.
- **Institutional backup for trust protector.** The backup is not a person but a position ("executive director of the San Diego LGBT Community Center"). System must capture this as an institutional/positional designation.
- **Multiple missing or outdated beneficiary designations.** IRA (probably Walter, deceased), savings (no POD), brokerage (no TOD). Each has a different status — the IRA is urgent, the others need designations created.
- **Walter's death story is emotional context with legal significance.** The conservatorship fight, the estranged family intervention, the months of legal proceedings — these explain Ray's urgency and his specific fear of probate and legal limbo.
- **Evelyn explicitly declined fiduciary role.** She quoted herself saying she "can barely manage my own affairs." But trust protector is a lighter role she might accept. System must capture both the declination and the potential willingness for the lighter role.
- **Joseph explicitly declined legal responsibility.** Quoted as saying he won't "sign anything." But he will take the cat. System must capture the boundary — he's a caretaker, not a fiduciary.
- **Named collection request is conditional.** Ray wants the books maintained under a specific name, but acknowledges the library needs to agree. He's already had a preliminary conversation. System should capture the wish, the condition, and the preliminary contact.
- **Two body disposition options with priority.** Balboa Park is the preference, Greenwood is the fallback. System must capture the hierarchy, not just list both as equal options.
