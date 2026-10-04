---
client: Raymond "Ray" Delacroix
number: 9
tier: 1
jurisdiction: California, United States
shape: Older single gay man, limited support network, professional fiduciary
net_worth: $1.3M
---

# 09. Raymond "Ray" Delacroix

**Older single gay man, limited support network, professional fiduciary.** No viable personal fiduciary: a professional fiduciary to be named, a trust protector over them, compensation and replacement terms, a named collection as a bequest, institutions as backup fiduciaries.

## Why this client exists

This profile tests a critical scenario: a client with no viable personal candidates for fiduciary roles. The capture engine must recognize that the professional fiduciary is not yet selected (a "to be named" placeholder), handle the trust protector concept (which adds a supervisory layer over the professional fiduciary), and capture the specific compensation and replacement provisions that are unique to professional fiduciary arrangements. The emotional backstory about Walter is important context the system should capture, as it explains the urgency and specific concerns driving the plan. Also tests multiple beneficiary designations that are either missing or outdated, the concept of a named collection as a bequest, and institutional beneficiaries serving in backup fiduciary roles.

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
