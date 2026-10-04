# Adding a client

## Where the client goes

Clients live under `clients/` in a folder per wealth tier: `tier-1-foundational/`, `tier-2-affluent/`, `tier-3-taxable/`, `tier-4-ultra-high-net-worth/`. `clients/README.md` defines the tiers and each tier folder's README says what a client there looks like and what it should test. Choose the tier by the planning problems the client brings, not by net worth alone; a borderline case goes where its problems belong, and the profile's "Testing Value" paragraph should say why.

The client's folder is `NN-surname/` inside the tier folder. `NN` continues the numbering across the whole set, not per tier: 01 to 09 are taken, so the next client is 10 whichever tier it joins. `COVERAGE.md` refers to clients by number and the numbers must stay unique.

## The layers

A client is a set of layered files, each derived from the one before it. Build them in this order and keep the derivation honest: anything in a later layer that does not trace to an earlier one is tagged `[SYNTH]` so it can be changed.

1. **The profile** (`profile.md`). Who they are: demographics, family, assets, planning goals, prior legal context, and a closing paragraph headed "Testing Value" that says what this client exists to exercise. Start from `COVERAGE.md` and the tier README: a new client should add a shape the set lacks.
2. **The interview** (`interview/transcript.md`). A simulated attorney interview of 35 to 45 minutes. Read `docs/transcript-design-notes.md` first: the transcripts are deliberately messy (tangents, self-corrections, one person called by three names, important facts dropped mid-digression), because a clean transcript tests nothing. Open the file with notes on what this conversation is built to test, then the dialogue under a `## Transcript` heading with bracketed timestamps.
3. **The dialogue-only transcript** (`interview/transcript-dialogue-only.md`). The same interview with the designer's notes removed, for feeding to a system under test. Derive it; do not edit it by hand.
4. **The answer key** (`interview/answer-key.md`, and `answer-key.json` for scoring). What a correct reading of the transcript must find, under the headings the existing keys use: People and Relationships, Assets, Distribution Plan, Fiduciary Designations, Prior Legal Context, Special Provisions, Items Requiring Follow-Up, and the Conversational Challenges set on purpose. Every line traces to the transcript.
5. **The supplemental intake** (`intake.md`). What the client returned on the follow-up form: full legal names, dates of birth, every asset with its account detail, liabilities, fiduciaries, the distribution plan, health-care wishes, final disposition, charitable giving, digital assets, prior legal context, and the document set. Use the twelve section headings the existing intakes use. Tag every value the interview never said `[SYNTH]`.
6. **Documents** (`documents/`). Optional, and nobody has done it yet. See the folder's README.
7. **A recording** (`recordings/`). Optional: if the interview is ever spoken aloud and captured, keep the audio and the utterance-level transcript so it never has to be re-spoken.

Then add the client's row to the tier folder's README, to the repository `README.md` and to the tables in `COVERAGE.md`, and a `README.md` in the client's folder in the shape of the existing ones (front matter with `client`, `number`, `tier`, `jurisdiction`, `shape`, `net_worth`). If the client is the first in its tier, change that tier's "no clients yet" to the count and update the tier table in the repository `README.md`.

## Rules that keep the set usable

- **Nobody real.** Invented names, addresses, employers, account numbers (the 555 exchange for phones). Never a real person, never a real client's facts however disguised.
- **Jurisdiction is explicit.** Every client's front matter says their state. The interview, the intake's document list and the answer key's plan expectations follow that state's law. A client from a new state is welcome and should say what differs.
- **The transcript is the authority** for what the client said. The profile is where they started; the intake is what they later supplied; the answer key is derived.
- **Changing a layer means changing what derives from it.** Edit the transcript and the answer keys and the dialogue-only copy change with it.
