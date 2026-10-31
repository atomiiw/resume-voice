---
name: resume-voice
description: Writes resume bullets from facts the user already has, in real resume register. Reads the target role and industry; picks the one memorable point per bullet and the industry precedent it echoes; interviews the user one question at a time; writes verb-led, artifact-centred bullets that end on a gain; judges every draft against evals/rubric.md before showing it. No clichés, no invented numbers, no narrative, and the user's own wording kept. Use whenever writing, rewriting, translating, tightening or reviewing any resume/CV bullet, project entry, summary line or LinkedIn experience text, in English or Chinese, including as one step of a bigger task (改简历, 翻译简历, polish this bullet, notes → resume). In long sessions, re-read before every new resume draft.
---

# Resume voice

The user has the facts. Your job: decide the one thing each bullet should make a reader remember, then say it in resume register. A resume describes things built and results measured. It never tells the story of the person's effort.

Priority when rules conflict: **facts > the one point > the user's wording > register > your taste.**

## 1. Register spec

The user's own bullet is the specification. Shape only; never reuse its content:

> Built /eval, a chat command for on-call engineers to regression-test their custom skills before publishing; 60 users on launch day.

Slots, in order:

```
[verb] [artifact], [appositive: what it is / for whom / to do what] [optional: one mechanism phrase]; [result: noun phrase with a number]
```

More of the user's own bullets, from their previous resume (shape only):

> Built a moving platform system that locks the player into its momentum, fixed jitter from overlapping movement and angled landings.
> Diagnosed that Gemini content-filter rejects 50%+ of valid requests, built auto-retry with randomized prompt variation.
> Built a storage system for nested popups (popups in popups) with a fully persisted hierarchy, re-anchoring popups on page reload via DOM text-matching.

A third reference the user rates highly is a hardware engineer's resume. Shape only:

> Designing the XNOR banks, popcount trees, and threshold comparators for all 8 neuron lanes — each lane reduces a 16-bit XNOR comparison to a 5-bit population count via a half-adder/full-adder tree before a threshold comparator produces a 1-bit neuron output.
> Eliminated secret-data-dependent timing side channels across multiple tensor backend operations in a forked open-source ML framework (Burn) by rewriting branching logic into constant-time implementations.
> Leading redesign of the team's power distribution PCB, increasing continuous current capacity from 20A to 40A while integrating a 97.6% efficient 48V→12V converter, Hall-effect current sensing, precharge, emergency-stop, and protection circuitry.

What it adds: present-participle openers for ongoing work ("Leading", "Designing"); coordinated verbs ("Designed and implemented"); numbers with units wherever they exist (25 MHz, 20A to 40A, 97.6%, 2.5 mW); lists of named components are welcome when each is concrete; after a dash or colon, a clause whose subject is a **component of the artifact** explaining how it works is fine ("— each lane reduces…"); a bullet may run to a third line when every clause is a technical specific.

What all three share: one artifact or technical act per bullet; the hard part is named as a specific mechanism ("permutation and sign ambiguity", "jitter from overlapping movement and angled landings"); industry-standard technology is named (React/ProseMirror, Cinemachine, DOM); a parenthetical carries a concrete specific; a number appears only where one exists. **The result tail is optional.** Most of the user's best bullets end on the mechanism, not a metric. When a number exists, end on it; otherwise end on the most concrete technical specific.

**Allowed grammar:** verb opener with no subject: past tense for finished work, present participle for ongoing work ("Leading redesign of…"), optionally preceded by one adverb ("Independently instructing"), or a noun-phrase status such as "First design hire for an edtech startup;"; coordinated verbs ("Designed and implemented"); after a dash or colon, a finite clause whose subject is a component of the artifact and which explains the mechanism ("— each lane reduces a 16-bit comparison to a 5-bit count"); further verbs chained by commas or participles when each names a technical act on the same artifact ("Built X…, designed Y, fixed Z"); appositives ("X, a tool for Y"); a relative clause **that modifies the artifact and says what it does** ("a system that locks the player into its momentum"); prepositional phrases; parentheticals with specifics "(50+ variables, 40+ tokens)"; a from→to phrase; after a semicolon, a verbless noun phrase or a second verb-led clause ("; grew DAU across 350,000+ users").

**Forbidden grammar:** a main-clause subject that is the person, the team, a before-state or an old version ("I", "the team", "setup", "the version"); a relative clause that introduces a before-state, a comparison or a new subject ("setup that took 8 parameters…", "the version that let the model plan"); narrative connectors ("until", "despite", "after", "then", and "while" when it sequences a story; "while integrating X" as a simultaneous technical act is fine); metaphorical verbs ("becomes", "turns into", "unlocks"); a clause with its own subject after the semicolon.

**Four traps the grammar rules don't catch by themselves:**
- **The implied subject of every verb is the candidate.** "; asked before a human" reads as the candidate asking. A fact about users or the artifact goes in a noun phrase ("; users' first stop before a human") or an artifact-modifying relative clause ("a bot users now @ before a human").
- **No verbless noun phrase mid-bullet on a comma.** "…threads, answers as exact steps…" misparses as a list. Attach with a participle ("delivering answers as…"), "with", or a parenthetical.
- **At most one absolute phrase.** "with the model only mapping…, a script computing…" needs a second read. For a two-part mechanism use an infinitive of purpose plus a participle ("Designed X to keep the model to Y, leaving Z to a script that…") or a colon with a compact list ("X: model maps the request to parameters, script computes the plan").
- **Verbs belong to the thing that does them.** A database stores; the bot answers. "a knowledge base that answers" makes the reader stumble; "a knowledge base the bot answers from" does not.
- **What the artifact does is a relative clause on the artifact, never a connector clause.** "a bot that answers in exact steps" is fine; "…knowledge base, so it answers in exact steps" gives a mid-bullet finite verb to the artifact and fails.
- **No symbols or chat shorthand as words.** "the group's first @ before a human" is unreadable; write "first stop before a human" or "users @-mention it before a human".
- **A from-state names its object.** "(a ~10-minute run, no runnable plan)" leaves "run of what" and "plan of what" open; "from a planner that ran 10 minutes without producing a test plan" does not.
- **No stacked prepositions, no yoked objects.** "a database the bot answers from in exact steps and the right screenshot" stacks "from in" and hangs "screenshot" off "in". Read each bullet aloud once; a stumble is a rewrite.
- **A behaviour belongs to the people who do it, at the source's scope.** "the 4,500-member group's first stop" makes the whole group the actor; the source says "users … first". Write "users in the 4,500-member group" or "first stop before a human for users in…".
- **A number stays on the noun it came with.** "10–12 root causes per meeting" cannot become "10–12 downvotes a week". Before using any number, name the noun it modifies in the source and keep that noun.
- **Mechanism nouns at reader level.** "declared questions and dependencies" is design-doc shorthand; "a script that asks only for what is missing and orders the steps" is what a reader can picture.

**A design-decision bullet needs a consequence, and has a fixed shape.** Stating the architecture ("model fills slots, code decides") shows taste; a reader believes it only with an outcome. Use this skeleton:

> [Redesigned/Split] [artifact] from [before-state as a noun phrase with its number] to [outcome as a noun phrase]: [component] does X, [component] does Y.

The from→to hangs on a verb that takes one ("cutting setup from…to…", "taking a run from…to…"), never on "Split" or "Redesigned [artifact]", which read as "separated from". The thing that moved is named ("setup", "a run"), not left to "a launch". Both sides of the from→to are **noun phrases** ("from about 10 minutes of unbounded model planning to a launch on the second message"). A relative clause on the from-side ("from one that let the model plan", "from the version that…") is the banned before-state form, and a "to" that names a structure ("to two parts") is not an outcome. The colon list after it carries the mechanism. If the outcome and the mechanism don't both fit in two lines, the mechanism loses a component, never the outcome.

**Project entries** get a one-line plain description under the title ("In-store AI try-on: scan a tag, upload a photo, preview fit across sizes."), so the bullets can be purely technical.

**Stance: describe the thing, not the person.** No effort, persuasion, resistance, feelings or struggle. Difficulty is shown only through four carriers: a scale number, a constraint written as a noun phrase ("for engineers who never read docs"), a from→to contrast, or the mechanism. If the hard part is interpersonal, show its outcome (who now owns what, what number moved), never the pushing.

**Clause test.** Every clause carries exactly one of: what was built · for whom / to do what · one technical mechanism · the result. A clause that carries none is cut, however true. A clause that a reader can't attach to one of these is cut.

**Readability.** A smart reader outside the project understands every noun on first pass. Industry-standard technology names (React, Cinemachine, DOM, MCP) are fine; project-internal layer names, codenames and team shorthand are generalised or cut. No abbreviations the reader has to expand ("65–81s", "8 params"). If compressing makes it cryptic, keep the plain version.

**Length.** 1–2 lines in the target layout (the user's current layout fits about 84 characters per line, so about 170). A third line is allowed only when every clause is a technical specific: a component, a number with a unit, a named mechanism. Never a final line with 1–4 orphan words.

**Rhythm across a section.** Strongest bullet first. Openers differ. Skeletons differ: at most two bullets in a section end on a "; result" tail; the others end on a mechanism, a parenthetical specific, or carry their from→to inside the body. Two consecutive bullets never share a skeleton (two from→to bullets in a row, both landing on "two…", read as one shape twice). Two bullets never land on the same specific ("two messages" in one, "the second message" in the next reads as the same win twice). Lead with the bullet the target reader would phone you about, which is not always the one with the biggest number. Two to four bullets per experience; coverage is not a goal.

## 2. Workflow

For a new resume, target or experience, run all steps. For a one-line tweak, run 5 and 6.

1. **Read the sources first.** The conversation, attached files, the notes or vault the user points to, earlier resumes. Ask only for what they don't contain.
2. **Target brief** (role, company, industry; ask if unknown). Write a few lines for the user: the business and the role's day-to-day; what reads as frontier in that industry today (search the web, it moves fast); the temperament the culture rewards. Every later judgement is against this brief.
3. **One point, one precedent, per bullet.** Pick the single most memorable thing as the target reader sees it. Find one gold-standard case in the target industry that shares its spirit. State why the user's version is hard compared to it. Show this as a table; the precedent never enters the resume. **End the step with a written "must carry" list per bullet**: the two to four elements without which the point is not expressed (the behaviour, the mechanism that caused it, the scale). This list is a hard constraint on steps 5 and 6; compression cuts optional detail, never a must-carry element.
4. **Interview, one question per message.** Most valuable gap first; say in one line why it matters. Open questions only: never suggest an answer, a number or a framing. Stop when each point can land.
5. **Write** to the register spec. Evoke the precedent through its angle (what it measured, what it removed, its from→to) and never through its name, slogan or recognisable phrase. Under each bullet, one line: the point, and what was cut to protect it.
6. **Judge before showing.** Principles are not enough here: writers who had read every rule above still produced comma-attached noun phrases and moved a number onto a different noun. Do this mechanically, in writing, for every bullet:
   - **Grammar parse.** Write out: the opener (verb form); every comma-attached phrase with its head word (a participle, or an appositive noun renaming the artifact, is fine; any other bare noun such as "setup" or "answers" is a rewrite); every finite verb with its subject (the candidate implied, or a component after a dash/colon; anything else is a rewrite); what follows the semicolon (a verbless noun phrase or a candidate-verb clause only).
   - **Number trace.** For every number: the source line, the noun it modifies there, the noun it modifies in the bullet. Different noun = rewrite.
   - **Point check.** For every must-carry element from step 3: the words in the bullet that carry it. A missing element is a rewrite, not a shortening.
   - **Outsider read.** Underline every noun a reader outside the project could not picture, and every symbol used as a word.
   - Then run `evals/rubric.md` criterion by criterion. If a subagent is available, give it only the rubric, the facts and the draft, and let it judge blind. A bullet that fails any criterion is not shown to the user.

## 3. Keep the user's voice

- What to say and in what order is your job: cut and reorder freely, and say what you cut.
- How it's said is theirs. Their verbs and nouns are the default. Change a word only when it blocks the point or the register, and flag each change with its reason. Never swap in a "stronger" synonym.
- The user's existing draft is the register reference, not a base to patch. Rebuild each bullet around its point; carry their words over.
- Don't introduce vocabulary they never use. Don't vary a term for elegance; repeat the name.
- Bans the user adds during a session hold for the session; offer to add them here.

## 4. Numbers

- Only numbers from the sources, exactly as stated, with their scope ("60 read the launch doc in 24 hours" is not "60 users").
- Never estimate, round, convert currency, or invent scale. No bullet needs a metric. A design target or projection may appear only if the source labels it so and the bullet keeps the label ("targeting 500–600 MHz at an estimated 2.5 mW").
- Never upgrade status: merged ≠ deployed, piloted ≠ adopted, proposed ≠ shipped.
- Don't strike the user's numbers reflexively. A derived number (a complement, a ratio) is theirs if the arithmetic holds; ask what it measures, then find the wording that is honest and keeps the weight.
- A bullet ends on a mechanism, a specific, or a gain. The old state appears only inside a from→to that ends on the gain. Never "stalled", "never worked", "failed" as the ending.
- A precedent never lends its scale.

## 5. Never

**Words** (unless the user wrote them): spearheaded, leveraged, orchestrated, championed, utilized, facilitated, pioneered, revolutionized, catalyzed, empowered, drove, synergy, robust, seamless, frictionless, cutting-edge, innovative, pivotal, impactful, passionate, results-driven, proven track record, best practices, end-to-end as filler, successfully, significantly, greatly. 中文：赋能、抓手、闭环、沉淀、拉通、聚焦、深度参与、全面提升、持续优化.

**Patterns:** negative parallelism ("not X but Y"); vague participle tails (", ensuring…", ", enabling…"); "through X, achieved Y" / 通过……实现……; "serves as" for "is"; puffery with no fact behind it ("key", "critical"); an intern who sounds like a VP; the precedent's name or slogan; frontier buzzwords pasted from the target brief where the user didn't do that thing.

## 6. Failure modes (each one was rejected by a real user)

| Looks like | Why it fails | Rejected example |
|---|---|---|
| Sentence-by-sentence translation | Chinese holds four facts per line; English can't. Hierarchy must be redesigned | A TryIt bullet carrying interviews, channel choice and validation site in one sentence |
| Compressed shorthand | Reader must decode | "8 CLI parameters only veterans got right became two plain-language messages" |
| Filler clauses | Clause carries none of the four slots | "from a single experiment to a batch"; "one form for whatever is still missing" |
| Prose | Subject + relative clause = an essay sentence | "setup that took 8 parameters only experts got right now takes two messages" |
| Negative tail | Resume states gains | "; the model-only version had stalled 10 minutes without launching" |
| Insider jargon | Outsider can't picture it | "through tool, MCP and skill layers to the one engineers could fix" |
| College-essay narrative | Person-centred effort story | "root-causing each downvote and arguing user impact against engineering risk until each fix had a named owner" |
| Metaphor as result | Not a fact | "a vague first message becomes a runnable plan" |
| Grammatically clean, point lost | Passes every surface rule but drops the mechanism or scale that made the point ("assigning 101 action items" for "ran the weekly loop that turned user downvotes into fixes 15 engineers owned") | A round that passed grammar and facts and was rejected by the user for forgetting what the bullet was for |

The corrected shape for the same facts is always the spec in §1: thing built, for whom, mechanism if it earns its place, number.

---
Sources adapted: career-ops (MIT) `modes/_writing.md` and `voice-dna.template.md`; StoneLL1/resume-builder `Resume-Writing-Guide-LLM.md` §4.1, §9; dabydat/resume-builder-skill length rules.
