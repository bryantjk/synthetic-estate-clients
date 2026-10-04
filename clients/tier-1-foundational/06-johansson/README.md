---
client: Linda Johansson
number: 6
tier: 1
jurisdiction: California, United States
shape: Widowed grandmother, multi-generational planning
net_worth: $2.8M
---

# 06. Linda Johansson

**Widowed grandmother, multi-generational planning.** A discretionary trust for a child with substance-use issues without punitive language, restatement versus revocation, a property that fell out of the trust, IRA designations to align.

## Why this client exists

Tests a complex emotional scenario: a parent wanting to protect a child with substance use issues without being punitive. The discretionary trust for Peter is a nuanced provision. The system must capture Linda's strong feelings about not including sobriety testing language while still creating a structure that protects Peter. Also tests trust restatement vs. revocation, a property that fell out of the trust, IRA beneficiary designation alignment, and multi-generational distributions with specific bequests.

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
