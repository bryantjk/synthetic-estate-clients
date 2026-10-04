---
client: Robert "Bobby" Fitzgerald
number: 4
tier: 1
jurisdiction: California, United States
shape: Recently divorced man, prior trust complications
net_worth: $1.7M
---

# 04. Robert "Bobby" Fitzgerald

**Recently divorced man, prior trust complications.** An unrevoked prior trust of uncertain status, beneficiary designations that contradict current wishes, a fuzzily remembered QDRO, a deliberately excluded sibling.

## Why this client exists

Directly mirrors the complexity of Client 1 from the real client examples. Prior trust with uncertain status, beneficiary designations that conflict with current wishes, a divorce where the trust wasn't clearly addressed, fuzzy recollection of legal details (QDRO), a deliberately excluded sibling with nuanced reasoning, and a strained family relationship. The capture engine needs to flag multiple potential legal issues: the unrevoked prior trust, the outdated beneficiary designations, and the unresolved QDRO situation.

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
