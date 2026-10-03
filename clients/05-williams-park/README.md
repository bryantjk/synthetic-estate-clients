---
client: Marcus and Andre Williams-Park
number: 5
jurisdiction: California, United States
shape: Married gay couple, no children, charitable focus
net_worth: $1.5M
---

# 05. Marcus and Andre Williams-Park

**Married gay couple, no children, charitable focus.** Chosen family, estrangement from blood relatives with legal consequences, a small business succession, heavy charitable giving, a domestic partnership followed by marriage.

## Why this client exists

Tests chosen family dynamics (Lisa's role), estrangement with legal implications, a small business succession concern, significant charitable giving, and the interplay between a domestic partnership and subsequent marriage. The biological family concern is an important capture point --- the system should flag that Andre may want explicit language addressing the exclusion of his biological relatives, even though he didn't use the word "disinherit." Also tests immediate DPOA and the concept of future pets in the pet trust.

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
