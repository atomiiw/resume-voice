# Judge rubric

Judge each bullet separately. Every criterion is PASS or FAIL with one line of reason. A bullet passes only if every criterion passes. Be strict: the labelled samples below show how strict.

## Criteria

- **R1 One point.** A reader remembers exactly one thing after reading it once. Two achievements, or an achievement plus unrelated background, is FAIL.
- **R2 Clause test.** Every clause carries one of: what was built · for whom / to do what · one technical mechanism · the result. A clause that carries none, or that a reader can't attach to one of these, is FAIL.
- **R3 Register grammar.** Opens with a past-tense verb and no subject (or a noun-phrase status such as "First design hire for an edtech startup;"). Further verbs may be chained by commas or participles when each names a technical act on the same artifact ("Built X…, fixed Y", "resolving Z"). A relative clause is allowed only when it modifies the artifact and states what it does ("a system that locks the player into its momentum"); a relative clause that introduces a before-state, a comparison or a new subject ("setup that took…", "the version that let…") is FAIL. No narrative connector (until, despite, after, then, while). No metaphorical verb (becomes, turns into, unlocks). After a semicolon: a verbless noun phrase or a second verb-led clause ("; grew DAU across 350,000+ users"); a clause with its own subject is FAIL. The implied subject of every verb is the candidate; a verb whose implied subject is the artifact or its users ("; asked before a human") is FAIL. A verbless noun phrase attached mid-bullet by a comma ("…threads, answers as exact steps…") is FAIL. More than one absolute phrase ("with the model mapping…, a script computing…") is FAIL.
- **R4 Stance.** Describes a thing and its measured effect. Any effort, persuasion, resistance, feeling or struggle is FAIL. Difficulty, if present, is carried by a scale number, a constraint noun phrase, a from→to, or a mechanism.
- **R5 Readability.** A smart reader outside the project understands every noun on first pass. The reader has the section header (company, role title, e.g. "AI Product Intern, Internal SRE Agent") and the bullets above it, so "the agent" is glossed by the header; a pronoun whose antecedent is only in a previous bullet ("its planner") is weak but not a FAIL on its own. Industry-standard technology names (React, Cinemachine, DOM, MCP) are fine. Project-internal layer names, codenames, shorthand ("65–81s", "params"), or a phrase that needs decoding is FAIL.
- **R6 Ending.** The bullet ends on a mechanism, a concrete specific, or a gain. No number is required. An old failure as the ending ("stalled", "never launched") is FAIL. A from→to that ends on the gain is PASS.
- **R7 Facts.** Every number and status is in the facts file with the same scope. Invented, rounded, converted or upgraded (merged→deployed, read→used) is FAIL. A number the user supplied with a sound derivation is PASS.
- **R8 Voice.** The user's verbs and nouns where they exist in the facts; no word from the banned list (spearheaded, leveraged, orchestrated, championed, utilized, facilitated, pioneered, revolutionized, catalyzed, empowered, drove, synergy, robust, seamless, frictionless, cutting-edge, innovative, pivotal, impactful, passionate, results-driven, proven track record, best practices, end-to-end as filler, successfully, significantly, greatly); no "stronger synonym" swapped in.
- **R9 Length.** At most about 170 characters. Over 185 is FAIL.
- **R10 Section rhythm** (judge once for the whole set). Strongest bullet first; no two consecutive bullets open with the same verb; skeletons vary (at most two bullets end on a "; result" tail); no bullet duplicates another's point.
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
