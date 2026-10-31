# Labelled samples

Used to calibrate judges and to show how strict the rubric is.


### Positive (PASS on all criteria)

> Built /eval, a chat command for on-call engineers to regression-test their custom skills before publishing; 60 users on launch day.

User's own. Verb, artifact, appositive with for-whom and to-do-what, semicolon, number. (The "60 users" scope was later corrected in the facts; judge the shape here, not the number.)

### More positives (PASS on all criteria; user's own previous resume and a reference resume the user rates highly)

> Built a moving platform system that locks the player into its momentum, fixed jitter from overlapping movement and angled landings.

> Built a camera zone system that collapsed a multi-file Cinemachine setup into one prefab, designed editor visualization, fixed breakage from hidden settings.

> Diagnosed that Gemini content-filter rejects 50%+ of valid requests, built auto-retry with randomized prompt variation.

> Built evaluation tooling for a neural signal decomposition model, resolving permutation and sign ambiguity in learned variables for consistent comparison.

> Avoided API key by injecting questions through ChatGPT's own input, kept invisible by reverse-engineering ChatGPT's React/ProseMirror frontend.

> First design hire for an edtech startup; grew DAU and session duration across 350,000+ users by implementing gamified features (Ranks, Avatar System, Friends system).

> Built and documented design systems (50+ variables, 40+ tokens) for product handoffs to support scalability and ensure design consistency.

Note what they share: one artifact or act per bullet; relative clauses only on the artifact ("that locks", "that collapsed"); comma-chained technical verbs; parenthetical specifics; a metric only where one exists; most end on a mechanism, not a number.

### Negatives (each must FAIL, with the reason the user gave)

N1 — user verdict: "看不懂" (can't understand it). Fails R5, R2.
> Built /eval, opening regression evals to skill writers: 8 CLI parameters only veterans got right became two plain-language messages; launch doc read by 60 in 24 hours.

N2 — user verdict: "太多废话，很多 clause 意义不明" (filler; clauses mean nothing). Fails R2, R1, R9.
> Cut any eval setup to two user messages, from a single experiment to a batch, down from the 8 parameters the eval CLI required. Built the planner that turns the first message into one form for whatever is still missing: the model reads the request, and a script works out the plan.

N3 — user verdict: "不是简历语言" (not resume language). Fails R3.
> Built /eval, a chat command for skill writers to regression-test a skill before publishing; setup that took 8 parameters only experts got right now takes two messages.

N4 — user verdict: "在简历里写负面数据而非进步" (negative data instead of progress). Fails R6.
> Split its planner in two: model translates the request into parameters, script computes the plan; the model-only version had stalled 10 minutes without launching.

N5 — user verdict: "这人看得懂吗" (would anyone understand this?). Fails R5.
> Hosted the agent's weekly bad-case review for 11 weeks, tracing each downvote through tool, MCP and skill layers to the one engineers could fix; upvote rate from 16% to 80%.

N6 — user verdict: "你写大学申请文书呢" (this is a college application essay). Fails R4, R3.
> Hosted the agent's weekly bad-case review for 11 weeks, root-causing each downvote and arguing user impact against engineering risk until each fix had a named owner; upvote rate from 16% to 80%.

N7 — rejected in the same batch as N6; metaphor as a result. Fails R3, R7 (no measured result).
> Split its planner in two: model translates the request into parameters, script computes the plan; a vague first message becomes a runnable plan after one round of plain-language questions.

