# The five judges

Each judge is a fresh agent with no conversation history. It receives: `rubric.md`, the facts file, the target brief, and the candidate bullets. Nothing else. Each judge applies the whole rubric but is told which criteria it owns and must be hardest on.

| Judge | Persona | Owns | Hardest question |
|---|---|---|---|
| J1 | Recruiter doing a six-second scan | R1, R10 | After one read, what is the one thing I remember from each bullet? If I can't say it in five words, FAIL. |
| J2 | Hiring manager for the target role (from the target brief) | R11, R4 | Can I tell what was hard from the facts alone? Does any bullet tell me about the person instead of the work? Would I recognise which famous product or person it imitates? (If yes, FAIL R11.) |
| J3 | Smart reader outside the project and the industry | R5, R2 | Which nouns can't I picture? Which clause can't I attach to anything? |
| J4 | Fact checker | R7, R8 | Each number and status: where in the facts file, same scope? Any banned word? Any word replacing the user's own? |
| J5 | Register editor | R3, R6, R9 | Is this a bullet or a sentence? Does it end on a gain? Character count. |

## Calibration

Before judging a candidate, every judge is run on the labelled samples in `samples.md` (shown to judges unlabelled and shuffled). A judge is calibrated when it passes the positive and fails every negative on the criterion the label names. A judge that passes a negative is miscalibrated: tighten the rubric wording, rerun. Candidate runs don't count until all five calibrate.

## Pass condition for the skill

One writer round in which all five judges pass all bullets and the set criteria, then a second round with a fresh writer that passes again. Two consecutive clean rounds.
