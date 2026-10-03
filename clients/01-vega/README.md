---
client: Maria Elena Vega
number: 1
jurisdiction: California, United States
shape: Single mother, straightforward plan
net_worth: $730K
---

# 01. Maria Elena Vega

**Single mother, straightforward plan.** Guardianship, minor beneficiaries with age conditions, the guardian/trustee distinction, and excluding an absent parent without naming him as disinherited.

## Why this client exists

Straightforward single-parent scenario. Tests the system's ability to handle guardianship designations, minor beneficiaries with age-based conditions, and the distinction between guardian and trustee roles. The absent father adds a nuance --- the system should capture the client's explicit wish to exclude someone without that person being a formal "disinherited" party.

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
| `recordings/` | one scripted run of this interview, spoken aloud: the mixed room audio and the utterance-level transcript as captured |

Everything is invented. Addresses, account numbers and institutions are fabricated and should not match any real person or account.
