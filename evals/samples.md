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

> Designed and implemented a custom 5-stage pipelined CPU in Verilog running at 25 MHz, featuring hazard bypassing and memory-mapped I/O for motor control, servo control, and keyboard interfacing.

> Designing the XNOR banks, popcount trees, and threshold comparators for all 8 neuron lanes — each lane reduces a 16-bit XNOR comparison to a 5-bit population count via a half-adder/full-adder tree before a threshold comparator produces a 1-bit neuron output.

> Leading redesign of the team's power distribution PCB, increasing continuous current capacity from 20A to 40A while integrating a 97.6% efficient 48V→12V converter, Hall-effect current sensing, precharge, emergency-stop, and protection circuitry.

> Eliminated secret-data-dependent timing side channels across multiple tensor backend operations in a forked open-source ML framework (Burn) by rewriting branching logic into constant-time implementations.

> Diagnosed and fixed an incorrect declassification boundary in an IFC-labeled training pipeline, correcting label propagation from the data-item level to the tensor level to restore compile-time security guarantees.

(The last five are from a hardware engineer's resume the user rates highly; its layout is wider, about 110 characters per line, so these run 2–3 lines there.)

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


N8 — user verdict: "我读不懂" (I can't read it). Passed R1–R12 with all five judges in round 7. Fails R0.
> Built /eval, a chat command for any skill writer to regression-test a skill, taking eval setup from expert-only to two messages — /eval's planner answers the first with plain-language choices for only what is missing and runs the eval on the second.
> Rebuilt the support bot's knowledge base as a structured database, delivering answers as exact steps with the matching screenshot plus a live lookup of the user's task session; first stop before a human for users in a 4,500-member group.
