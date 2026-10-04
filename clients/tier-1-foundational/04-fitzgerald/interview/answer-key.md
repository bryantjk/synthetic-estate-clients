# Extraction Answer Key — transcript_04_fitzgerald

# Extraction Answer Key
The following is a summary of key data points that the capture engine
should extract from this transcript, organized by data model category.
This serves as the ground-truth for measuring capture accuracy.

## People & Relationships
-   **Robert "Bobby" Fitzgerald** --- Principal. Age 61, retired
    commercial pilot (United Airlines). Resides in La Jolla, San Diego,
    CA (renting). Divorced January 2025.

-   **Catherine Fitzgerald (now Catherine Moore)** --- Ex-wife.
    Remarried. Amicable relationship. 30+ year marriage. Still listed as
    beneficiary on IRA and Merrill Lynch accounts.

-   **Patrick Fitzgerald** --- Son. Age 32. Lives in Denver, CO. Married
    to Julia. No children. Plays guitar (relevant to specific bequest).
    Successor trustee.

-   **Julia** --- Patrick's wife. No last name given in conversation.

-   **Erin Fitzgerald** --- Daughter. Age 29. Lives in San Diego. In
    relationship with David (boyfriend). Works in project management.
    Primary trustee, executor, and DPOA agent. Pet caretaker for Murphy.

-   **David** --- Erin's boyfriend. No last name given. Long-term
    relationship.

-   **Colleen Byrne** --- Sister. Age 58. Lives in Boston, MA. Very
    close relationship (weekly calls). Married to Brian. Has two
    daughters Amy and Bridget. Successor DPOA agent. Backup pet
    caretaker for Murphy.

-   **Brian** --- Colleen's husband. Bobby mentions being closer to
    Brian than to Thomas.

-   **Amy and Bridget** --- Colleen's daughters (Bobby's nieces).
    Adults. Ages approximate ("twenty-something"). Each receives
    \$10,000 specific bequest.

-   **Thomas Fitzgerald** --- Brother. Age 55. Lives in San Diego.
    Strained relationship due to family business dispute. Excluded from
    plan. Not a formal disinheritance; Bobby is clear it's not punitive
    and Thomas has his own resources.

-   **Murphy** --- Dog (Irish Setter). Age 8. \$40,000 pet trust. Erin
    primary caretaker, Colleen backup.

## Assets
-   **Traditional IRA:** \~\$890,000. Rolled over from airline 401(k).
    Beneficiary likely still Catherine (needs verification).

-   **Roth IRA:** \~\$210,000. Beneficiary unknown (possibly Catherine,
    possibly kids --- Bobby unsure).

-   **Airline Pension:** \~\$6,800/month. Catherine receives a survivor
    benefit via QDRO (details uncertain, paperwork unclear).

-   **Savings:** \$75,000 at Bank of America.

-   **Brokerage:** \~\$340,000 at Merrill Lynch (individual account,
    received in divorce). Beneficiary likely still Catherine.

-   **Whole Life Insurance:** \$250,000 face value, \~\$85,000 cash
    value. Beneficiaries correctly listed as Patrick and Erin equally.

-   **Vehicle:** 2022 Ford F-150.

-   **Guitar Collection:** 15--16 vintage instruments including a 1963
    Fender Stratocaster and 1970s-era Gibsons. Estimated value
    \~\$60,000+. Specifically bequeathed to Patrick.

-   **Real Estate:** None. Renting in La Jolla. Del Mar house sold in
    divorce.

## Distribution Plan
-   Guitar collection to Patrick (specific bequest)

-   \$40,000 to pet trust for Murphy

-   \$10,000 each to Amy and Bridget (Colleen's daughters)

-   \$20,000 to Air Line Pilots Association charitable foundation

-   Remainder split 50/50 between Patrick and Erin, outright (no trust,
    no age conditions)

## Fiduciary Designations
-   **Trustee:** Erin. Successor: Patrick.

-   **DPOA Agent:** Erin. Successor: Colleen. (Note: different from
    trustee succession.)

-   **DPOA Type:** Springing (effective upon incapacity only).

## Prior Legal Context (FLAGS)
-   **FLAG:** Joint revocable living trust created \~2005 with
    Catherine. Broad asset assignment language. May not have been
    formally revoked in divorce.

-   **FLAG:** IRA and Merrill Lynch beneficiary designations almost
    certainly still list Catherine. Conflicts with intended distribution
    plan.

-   **FLAG:** Roth IRA beneficiary unknown. Needs verification.

-   **FLAG:** QDRO related to airline pension --- Bobby unclear on
    details, may not have paperwork. Survivor benefit assigned to
    Catherine in divorce.

-   **FLAG:** Divorce judgment may not specifically address revocation
    of the 2005 trust.

## Special Provisions
-   **Pet trust:** \$40,000 for Murphy. Erin primary caretaker, Colleen
    backup.

-   **Charitable bequest:** \$20,000 to ALPA charitable foundation.

-   **Body disposition:** Cremation. Ashes scattered at sea off San
    Diego coast.

-   **Legacy letter:** Bobby wants to write a personal letter to his
    children to be kept with the trust documents.

## Conversational Challenges for Capture Engine
The following elements in this transcript are designed to test specific
capture engine capabilities:

-   **Murphy mentioned casually in small talk (minute 4)** before the
    pet trust discussion (minute 23). System must connect these
    references.

-   **Guitar collection mentioned during assets (minute 17)** with
    distribution intent revealed later (minute 25). System must link
    asset to bequest.

-   **Thomas introduced reluctantly with emotional context.** System
    must capture both the exclusion and the reasoning (not punitive,
    distant relationship, Thomas has his own resources).

-   **Bobby is vague about the QDRO.** Uses phrases like "I think," "my
    attorney mentioned something," "I don't fully understand." System
    should assign low confidence to QDRO details.

-   **Bobby is unsure about Roth IRA beneficiary.** Says "might be
    Catherine, might be the kids." System should flag as unknown, not
    guess.

-   **Nieces' ages are vague.** Bobby says "twenty-something" for both.
    System should capture the imprecision rather than inventing specific
    ages.

-   **Different successor chains for different roles.** Trustee: Erin →
    Patrick. DPOA: Erin → Colleen. System must not conflate these.

-   **Tangent about flying and the ocean (minute 28).** Contains the
    body disposition wish (ashes at sea) embedded in a personal story.
    System must extract the actionable detail from the tangent.

-   **Legacy letter request comes at the very end, almost as an
    afterthought.** System must capture late-stage additions that the
    client raises after the attorney has summarized.

-   **Life insurance is confirmed correct; system must distinguish**
    between accounts where beneficiaries need to be changed vs. accounts
    where they're already correct.

-   **Prior trust details are vague and uncertain.** Year is approximate
    ("I want to say 2005?"), terms are recalled imprecisely. System
    should flag the prior trust as a high-priority issue requiring
    document review.
