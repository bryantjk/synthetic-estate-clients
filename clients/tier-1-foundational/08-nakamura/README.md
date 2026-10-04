---
client: Patricia and George Nakamura
number: 8
tier: 1
jurisdiction: California, United States
shape: Married couple nearing retirement, charitable legacy
net_worth: $3.3M
---

# 08. Patricia and George Nakamura

**Married couple nearing retirement, charitable legacy.** Tax-aware giving (IRA to charity, Roth to family), a partner acknowledged outside the documents, different disposition wishes per spouse, outdated wills, a CPA's vocabulary.

## Why this client exists

Tests sophisticated tax planning awareness (IRA to charity, Roth to family), the desire to acknowledge a non-legally-connected partner (Sam) in a limited way, different body disposition wishes for each spouse, outdated wills that need revocation, and IRA beneficiary designations that conflict with the new plan. George's CPA background means the conversation may include more technical financial language that the capture engine needs to handle. Also tests the situation where a client wants to express something (feelings about Sam) outside the legal document.

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
