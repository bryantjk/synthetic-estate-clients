# Transcript Design Notes

These notes describe the design principles used to construct the simulated client interview transcripts. They were originally embedded in the Fitzgerald transcript (Profile 4) and apply when creating simulated conversations for any client profile.

---

## Overview

Each simulated interview is designed to test the capture engine's ability to extract structured information from natural conversation. The transcripts deliberately include realistic conversational artifacts: tangents, self-corrections, informal references, information delivered out of order, vague recollections, emotional digressions, and casual mentions of legally significant details. Stage directions in brackets indicate non-verbal context.

## Conversational Flow Design

The conversation mirrors the attorney's natural interview style. It opens with genuine small talk and rapport building --- the attorney mentions their own mother, the client talks about retirement and his dog. A disclaimer about sensitive topics (death, incapacity) is delivered early and naturally, with an explicit invitation to pause if needed. This warmth and personal disclosure is deliberate: it establishes trust and makes the client more likely to open up about emotionally charged topics later, such as the strained relationship with his brother.

The interview then flows through loosely defined phases --- family and relationships, prior planning history, assets, goals and concerns, distribution wishes, fiduciary designations --- but does not follow a rigid script. Topics bleed into each other naturally. The attorney circles back to earlier topics when new information warrants it (returning to the prior trust issue in minute 33 after initially discussing it in minute 9). The conversation wraps with a summary, homework assignments, and space for the client to raise anything that was missed.

## Deliberate Messiness

Real client conversations are not clean or orderly. Clients mention things out of sequence, go on tangents, refer to the same person by different terms at different points, and drop important details casually in the middle of unrelated topics. The transcripts deliberately incorporate these patterns as specific tests for the capture engine:

**Cross-reference test (pet):** Murphy (the dog) is first mentioned in casual small talk at approximately minute 4, in the context of Bobby joking about Erin visiting too often. The pet trust discussion doesn't happen until minute 23. The capture engine must recognize that the dog mentioned during rapport building is the same animal being planned for later, and must connect the early contextual information (breed, age, personality) with the later planning details (funding amount, caretaker designation).

**Cross-reference test (asset-to-bequest):** The guitar collection surfaces during the asset inventory discussion at approximately minute 17, where Bobby describes the instruments and their value. However, the distribution intent --- that the collection should go to Patrick specifically --- doesn't emerge until the distribution conversation at minute 25. The system must link the asset identified in one phase of the conversation with the bequest instruction given in a later phase.

**Embedded detail in tangent:** Bobby's wish for disposition of his remains is embedded inside a tangent about his flying career and love of the ocean at minute 28. He moves from reminiscing about being a pilot, to a joke his ex-wife used to make, to stating that he wants cremation and ashes scattered at sea --- all in a stream of consciousness that the attorney gently allows to play out. The capture engine must extract the actionable legal detail (cremation, ashes at sea off San Diego) from what is otherwise a personal, emotional digression.

**Late-stage additions:** The legacy letter request comes at the very end of the conversation, after the attorney has already delivered a comprehensive summary of the plan. This is a common pattern in real interviews --- clients think of additional things once they feel the pressure of the formal interview is over and the conversation is winding down. The system must capture late-stage additions and not treat the attorney's summary as the definitive close of information gathering.

## Realistic Client Vagueness

Clients are not precise narrators of their own legal and financial situations. They use hedging language, approximate numbers, and express uncertainty about things they signed years ago. The transcripts model that vagueness in several specific ways, each of which should produce lower confidence scores from the capture engine:

- **Approximate dates:** The client says "this was back in, I want to say 2005?" The question mark in tone signals uncertainty. The capture engine should record the approximate date but flag it as low confidence.
- **Unresolved legal status:** The client does not know whether a prior trust was formally revoked during the divorce. Phrases like "I'm not sure," "I don't specifically remember anyone saying the trust is dissolved," and "whatever the term is. Revoked?" signal a critically important legal issue that the system should flag as requiring document review.
- **Vague awareness of legal instruments:** The client has only a vague awareness of a QDRO, saying "my attorney mentioned something about that," "I think that was part of the deal," and "I don't fully understand how that works." The capture engine should assign low confidence and flag the need for the actual document.
- **Unknown beneficiaries:** The client is uncertain about beneficiary designations, saying "it might be Catherine, it might be the kids." The system should capture this as unknown rather than guessing.
- **Imprecise ages:** Ages given as "twenty-something" should be captured faithfully rather than inventing specific numbers.

## Distinct Successor Chains

A subtle but important test is that a client may name different successor chains for different fiduciary roles. For example, trustee succession might be Erin followed by Patrick, while DPOA succession is Erin followed by Colleen. The reasoning is organic --- for the DPOA, the client wants someone who would be immediately responsive in a crisis, whereas for the longer-term trustee role, the client prefers their children.

This is a critical test because many systems would assume the same succession order applies across all fiduciary roles. The system must maintain separate succession chains for each distinct role and must not conflate them.

## Emotional Context as Planning Context

Emotional content is not merely atmospheric --- it carries planning significance. A strained relationship includes both the emotional reality ("we're just distant") and the practical reasoning for exclusion ("he's doing fine financially," "he got more than his share"). The capture engine should extract both the exclusion decision and the reasoning behind it, because the reasoning informs how the exclusion is handled in the document --- as a natural omission rather than a punitive disinheritance.

Similarly, relational data points (e.g., being closer to a brother-in-law than a sibling) provide context about family dynamics that could be relevant in future planning conversations.

## Beneficiary Designation Complexity

Transcripts may include multiple accounts with different beneficiary statuses. The capture engine must distinguish between them accurately:

- **Confirmed correct:** "I'm sure about that." Mark as high confidence, no change needed.
- **Almost certainly outdated:** "I never changed them after the divorce." Flag as conflict with intended distribution.
- **Genuinely unknown:** "I honestly don't remember." Capture as unknown requiring verification --- do not conflate with accounts where the client has a guess.
- **Governed by separate instrument:** Pension with QDRO is a settled legal arrangement, not something to be changed but something to be documented.

## Principles for Creating Additional Transcripts

When generating simulated conversations for other client profiles:

1. **Start with rapport.** Allow 3--5 minutes of small talk that establishes the client's personality and may contain early, casual mentions of people, pets, or concerns that become formally relevant later.

2. **Let information emerge out of order.** Clients do not present their situations in the categories the system expects. A mention of a sibling might come up during a discussion of assets. A distribution wish might surface during the family overview. The system must assemble a coherent picture from scattered inputs.

3. **Include self-corrections and contradictions.** A client might say they have two retirement accounts and then mention a third one ten minutes later. Or give a dollar amount and then revise it. These test the system's ability to update its model when new information supersedes old information.

4. **Vary confidence signals.** Some information should be stated with certainty. Other information should be hedged. Some should be explicitly unknown. The capture engine's confidence scoring should reflect these differences.

5. **Include emotional context that carries planning significance.** Strained relationships, special closeness to certain family members, fear of specific outcomes, and experiences that motivate the planning are not just atmospheric detail --- they inform the plan's structure and priorities.

6. **Allow tangents and let the attorney redirect naturally.** Real clients tell stories, reminisce, and go off topic. The attorney should gently bring the conversation back without being abrupt. Legally significant information sometimes emerges from within these tangents.

7. **End with space for afterthoughts.** Real clients often add important items after the attorney has summarized. The final minutes should include at least one additional detail or request that the client raises unprompted.
