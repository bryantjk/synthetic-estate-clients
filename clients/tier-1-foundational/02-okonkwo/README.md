---
client: James and Priya Okonkwo
number: 2
tier: 1
jurisdiction: California, United States
shape: Married couple, young family, standard plan
net_worth: $2.4M
---

# 02. James and Priya Okonkwo

**Married couple, young family, standard plan.** The standard couple: joint planning with two sets of agents, a pet trust, keeping each spouse's family on the right side, Nigerian and Indian naming conventions.

## Why this client exists

The classic married-with-kids scenario. Tests the system's handling of joint planning (two DPOAs, two sets of agent designations), a pet trust, and cross-cultural family naming conventions. The system needs to correctly associate each spouse with their respective family members and agent designations without confusing who belongs to which side.

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
