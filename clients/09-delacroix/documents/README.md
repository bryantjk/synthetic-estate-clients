# Client documents

**Empty to start.** This folder is the place for the papers a real client brings to the first meeting, so that a system under test can be asked to read documents as well as a conversation. Nothing here exists yet; the facts these documents would carry are already in `../intake.md`, and any document added must agree with it.

## What belongs here

- deeds and the latest property tax bill for each parcel in `intake.md`
- account statements (a first page is enough) for each account
- beneficiary designation forms, including the outdated ones the client mentions in the interview
- prior wills, trusts, powers of attorney and directives the interview says exist
- business documents (operating agreement, buy-sell) where the client owns a business
- life insurance policy declarations
- a marriage certificate, divorce judgment or QDRO where the interview turns on one

## Rules

1. **Fabricated, and visibly so.** Use the 555 phone exchange, the account numbers in `intake.md`, and institution names that are either the ones already in `intake.md` or plainly invented. Never a real person's name, a real address, or a real account format that could be mistaken for a live one.
2. **Consistent with `intake.md`.** A document that contradicts the intake is a defect unless the contradiction is the point, in which case say so in a note beside it and in `intake.md`.
3. **One file per document**, named `<what>_<whose>.<ext>` in lower case, for example `deed_carmel_valley_home.pdf`, `beneficiary_form_fidelity_401k_james.pdf`, `prior_will_2009_george.pdf`.
4. **Say how it was made.** A short `MANIFEST.md` here listing each file, what it shows, and whether it was drawn by hand, generated from a template, or produced by a tool, so a contributor from another firm can reproduce or extend it.
5. **Jurisdiction.** Documents follow the client's state (see the front matter of `../README.md`). A deed form from another state is a different test and should be labelled as one.
