# Judge rubric

Judge each bullet separately. Every criterion is PASS or FAIL with one line of reason. A bullet passes only if every criterion passes. Be strict: the labelled samples below show how strict.

## Criteria

- **R1 One point.** A reader remembers exactly one thing after reading it once. Two achievements, or an achievement plus unrelated background, is FAIL.
- **R2 Clause test.** Every clause carries one of: what was built · for whom / to do what · one technical mechanism · the result. A clause that carries none, or that a reader can't attach to one of these, is FAIL.
- **R3 Register grammar.** Opens with a verb and no subject: past tense for finished work, present participle for ongoing work ("Leading redesign of…"), optionally after one adverb ("Independently instructing"); or a noun-phrase status such as "First design hire for an edtech startup;". Coordinated verbs ("Designed and implemented") are fine. Further verbs may be chained by commas or participles when each names a technical act on the same artifact ("Built X…, fixed Y", "resolving Z"). A relative clause is allowed only when it modifies the artifact and states what it does ("a system that locks the player into its momentum"); a relative clause that introduces a before-state, a comparison or a new subject ("setup that took…", "the version that let…") is FAIL. No narrative connector (until, despite, after, then; "while" when it sequences a story). "while integrating X" as a simultaneous technical act on the same artifact is fine. No metaphorical verb (becomes, turns into, unlocks). After a semicolon: a verbless noun phrase or a second verb-led clause ("; grew DAU across 350,000+ users"); a clause with its own subject is FAIL, except after a dash or colon when the subject is a component of the artifact and the clause (or a short chain of such clauses) explains its mechanism ("— each lane reduces a 16-bit comparison to a 5-bit count", "X: model maps the request to parameters, script computes the plan": PASS). An appositive renaming the artifact just built ("Built /eval, a chat command for…") is PASS; it is not the banned mid-bullet noun phrase. The implied subject of every verb is the candidate; a verb whose implied subject is the artifact or its users ("; asked before a human") is FAIL. A verbless noun phrase attached mid-bullet by a comma ("…threads, answers as exact steps…") is FAIL. More than one absolute phrase ("with the model mapping…, a script computing…") is FAIL.
- **R4 Stance.** Describes a thing and its measured effect. Any effort, persuasion, resistance, feeling or struggle is FAIL. Difficulty, if present, is carried by a scale number, a constraint noun phrase, a from→to, or a mechanism.
- **R5 Readability.** A smart reader outside the project understands every noun on first pass. The reader has the section header (company, role title, e.g. "AI Product Intern, Internal SRE Agent") and the bullets above it, so "the agent" is glossed by the header; a pronoun whose antecedent is only in a previous bullet ("its planner") is weak but not a FAIL on its own. Industry-standard technology names (React, Cinemachine, DOM, MCP) are fine. Project-internal layer names, codenames, shorthand ("65–81s", "params"), or a phrase that needs decoding is FAIL.
- **R6 Ending.** The bullet ends on a mechanism, a concrete specific, or a gain. No number is required. An old failure as the ending ("stalled", "never launched") is FAIL. A from→to that ends on the gain is PASS.
- **R7 Facts.** Every number and status is in the facts file with the same scope. Invented, rounded, converted or upgraded (merged→deployed, read→used) is FAIL. A number the user supplied with a sound derivation is PASS. A design target or projection is PASS only if the source labels it so and the bullet keeps the label ("estimated", "targeting").
- **R8 Voice.** The user's verbs and nouns where they exist in the facts; no word from the banned list (spearheaded, leveraged, orchestrated, championed, utilized, facilitated, pioneered, revolutionized, catalyzed, empowered, drove, synergy, robust, seamless, frictionless, cutting-edge, innovative, pivotal, impactful, passionate, results-driven, proven track record, best practices, end-to-end as filler, successfully, significantly, greatly); no "stronger synonym" swapped in.
- **R9 Length.** At most two lines in the target layout; the target brief gives characters per line (default 84, so about 170 characters). A third line (up to about 250) is PASS only when every clause is a technical specific (component, number with unit, named mechanism); otherwise FAIL. A fourth line is FAIL.
- **R10 Section rhythm** (judge once for the whole set). Strongest bullet first; no two consecutive bullets open with the same verb; skeletons vary (at most two bullets end on a "; result" tail); no bullet duplicates another's point or lands on the same gain specific as its neighbour.
- **R11 Difficulty legible** (judge once for the whole set). From the bullets alone, a target-industry reader can tell what was hard, without being told it was hard. A bullet that states a design decision with no consequence (no from→to, no adoption or outcome specific) counts against this.

## Output format

```
Bullet 1: PASS | FAIL
  R1 PASS – …
  R2 FAIL – …
  …
Bullet 2: …
Set: R10 PASS|FAIL – … ; R11 PASS|FAIL – …
Overall: PASS | FAIL
```
