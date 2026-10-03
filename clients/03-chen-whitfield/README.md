---
client: Sandra and Diane Chen-Whitfield
number: 3
jurisdiction: California, United States
shape: Married lesbian couple, blended family, complex distributions
net_worth: $2.3M
---

# 03. Sandra and Diane Chen-Whitfield

**Married lesbian couple, blended family, complex distributions.** A non-biological parent, unequal shares with stated reasons, charitable giving with tax motives, a beneficiary-designation conflict, prior documents to revoke, an immediate DPOA.

## Why this client exists

Rich testing scenario. LGBTQIA+ couple with a blended family, asymmetric parent-child relationships, unequal distributions with clear reasoning, charitable giving with tax optimization, pet provisions, prior legal documents that need to be revoked, and a beneficiary designation conflict (the Fidelity account). The system must handle the non-biological parental relationship correctly and capture the emotional dynamics that drive the distribution decisions. Also tests immediate DPOA selection.

## What is here

| File | What it is | Authority |
|---|---|---|
| `profile.md` | who they are: demographics, family, assets, goals, prior legal context | the starting point; the transcript may add to it and may contradict what the client half-remembers |
| `interview/transcript.md` | the simulated attorney interview, with the designer's notes on what it tests at the top | **the authority for everything the client said** |
| `interview/transcript-dialogue-only.md` | the same interview with the notes removed, for feeding to a system under test | derived from `transcript.md` |
| `interview/answer-key.md` | what a correct reading of the transcript must find: people, assets, the plan, fiduciaries, prior documents, open items, and the traps set on purpose | derived from the transcript; every line traces to it |
| `interview/answer-key.json` | the same, structured, for automated scoring | derived from `answer-key.md` |
| `intake.md` | what the client returned on the follow-up form after the interview. Values not said in the interview are tagged `[SYNTH]` | transcript plus intake is the complete data set a finished plan should reflect |
| `documents/` | the papers a real client would bring (deeds, statements, designation forms, prior instruments). **Empty to start**; its README says what belongs | to be created |

Everything is invented. Addresses, account numbers and institutions are fabricated and should not match any real person or account.
