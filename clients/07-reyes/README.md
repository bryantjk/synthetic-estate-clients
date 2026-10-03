---
client: Tomás Reyes
number: 7
jurisdiction: California, United States
shape: Single young professional, simple plan, first-time client
net_worth: $150K
---

# 07. Tomás Reyes

**Single young professional, simple plan, first-time client.** The simplest end of the range: a nonbinary partner, cryptocurrency and app IP, an agent who is not the primary beneficiary, urgency from a parent who died without a plan.

## Why this client exists

Tests the youngest and simplest end of the client spectrum, but with meaningful nuances. The unmarried partner with nonbinary identity tests the system's pronoun and relationship handling. Digital assets (crypto, app IP) are an increasingly common concern. The emotional motivation (father's death without a plan) is context the system should capture as it informs the urgency and priorities. Also tests the scenario where the DPOA agent is different from the primary beneficiary --- Ash is the agent but Gloria is the primary beneficiary.

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
