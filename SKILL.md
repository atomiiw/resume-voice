---
name: resume-voice
description: Builds resume bullets from content the user already has. Reads the target role, company and industry; picks the one memorable point per bullet; finds the industry precedent it echoes; interviews the user one question at a time for the details that amplify it; then writes tight, rhythmic English that evokes the precedent without naming it, with no clichés, no invented numbers and the user's own wording kept. Use whenever writing, rewriting, translating, tightening or reviewing any resume/CV bullet, project entry, summary line or LinkedIn experience text, in English or Chinese, including when it is one step of a bigger task (改简历, 翻译简历, polish this bullet, notes → resume). In long sessions, re-read before every new resume draft.
---

# Resume voice

The user already has the facts. Your job is to decide what is worth remembering, then say only that, in resume register.

A resume is not a record of what happened. Each bullet is one claim a reader should still remember after six seconds. Translating or tightening sentence by sentence is the failure mode: Chinese can hold four facts in one line, English cannot, so the information hierarchy is redesigned, not carried over.

Priority when rules conflict: **facts > the one point > the user's wording > resume register > your taste.**

## Workflow

Run the steps in order for a new resume, a new target, or a new experience. For a one-line tweak, skip to step 5.

### 1. Read the sources before asking anything

Read everything already available: this conversation, attached files, the notes or vault the user points to, earlier resumes. Collect every fact, number and status for each experience. You ask the user only for what these don't contain.

### 2. Read the target

You need the role, company and industry. If you don't have them, that is your first question. Then work out, and show the user in a few lines:

- **The business:** what the company sells, who the customer is, and what this role does day to day.
- **What reads as frontier there now:** the concepts and practices this industry currently treats as sharp. For AI tooling this might be evals, agent harnesses, context engineering, or predictable and steerable AI. Derive them for this target and date. Search the web if you can, because these move fast.
- **The person they celebrate:** the temperament the company's culture rewards. Examples: first-principles and speed; care and honesty about limits; taste and craft; ownership of messy real-world deployment.

Everything after this is judged against this brief.

### 3. One point per bullet, one precedent per point

For each bullet (or each experience, if bullets aren't drawn yet):

- **Pick the one point:** the single most impressive, most memorable thing, as the target reader sees it. Everything else in the source is cut or kept only to serve this point.
- **Find one precedent:** a gold-standard case from the target industry (a product, a person, an engineering practice) that shares this point's spirit. Example: turning any eval setup into two chat messages has the spirit of Tesla's online store turning a dozens-of-options car order into a handful of taps.
- **Analyze why the user's version is hard:** compare it to the precedent. Usually the idea is known; the hard part is doing it here. Example: "collapsing a long form is an old idea, but making a sprawling, half-specified eval config land in two turns, inside a chat interface, for engineers who won't read docs, is hard." This analysis is what the bullet must make the reader feel.

Show the user a short table: bullet → the one point → precedent → why it's hard. The precedent is for your analysis and the user's eyes only. It never appears in the resume.

### 4. Interview, one question at a time

Find the missing detail that would most amplify each point: the size of the before-state, the constraint that made it hard, who it was for, the number that proves it, what happened next.

- Look in the sources first. Ask only for what is missing.
- Ask **one question per message**, most valuable gap first. Say in one line why it matters ("this would show how long the old setup was").
- Ask open questions. Never suggest an answer, a number or a "stronger" framing for the user to agree to.
- Stop when each point has enough to land. If the user doesn't know, write the bullet without that detail.

### 5. Write

- **Start from the user's latest draft.** If they already have a version, it is the base: make the fewest edits that fix facts and sharpen the point, and show each edit against their sentence. Don't redraft from scratch in your own phrasing.
- **Readable on first pass beats short.** Someone outside the project must understand each bullet without rereading. Compression never produces noun stacks ("maps the goal to missing inputs"), unexplained shorthand ("65–81s", "veterans"), or a contrast the reader has to decode. If cutting makes it cryptic, keep the longer, plain sentence.
- **Every clause serves the bullet's one point.** A clause that adds a second achievement, a process step or background the point doesn't need gets cut, however true it is. If a second point truly matters, it gets its own bullet, or it goes.
- **Evoke the precedent; never cite it.** Borrow its angle: what it chose to measure, what it removed, the before→after contrast it is known for, the side of the story it tells. Never use its name, slogan, signature phrase or obvious paraphrase. Test: the reader should feel this person is sharp without being able to say which product or person it reminds them of. If the source is recognizable, pull back.
  Example: the Tesla spirit is "count the user's actions, then cut them". A bullet that measures setup in messages ("from idea to running batch in two messages") carries it. Writing "few-click", "frictionless ordering" or naming Tesla does not.
- Then apply the register, voice, Never and Numbers rules below.
- Show each final bullet with one line under it: the point, and what was cut to protect it.

## Register

A bullet is a sentence with "I" removed and everything that doesn't serve the point cut. It is not a diary (chronological, "first… then… finally", process before point) and not marketing copy.

The user's own bullet shows the target shape (shape only; never reuse its content):

> Built /eval, a chat command for on-call engineers to regression-test their custom skills before publishing; 60 users on launch day.

Plain verb → named artifact → appositive saying what it is and who it's for → semicolon → one hard result as a short noun phrase.

**Compression moves:**
1. **Cut** process narration ("worked with X to", "was responsible for", "helped to"), time sequence, restated context, "in order to" (→ "to"), "successfully", "various", "effectively".
2. **Lead with the point**, then the how, then the hard fact. Context goes after the object, or nowhere.
3. **Fold clauses into phrases.** "X, a tool for Y" over "X, which is a tool that helps Y".
4. **End on the fact**, as a terse tail after a semicolon. Start and end are the stressed positions.
5. **Length:** 1–2 lines, usually shorter than you think. Never leave a second line with 1–4 orphan words.

**Rhythm across a section (抑扬顿挫):**
- Vary the skeleton: a short one-clause bullet; a two-part bullet with a semicolon result; one longer bullet where the difficulty earns the length.
- Don't open consecutive bullets with the same verb or structure. Don't default to lists of three.
- Strongest bullet first. Fewer, sharper bullets beat complete coverage: 2–3 per experience is normal.

## Keep the user's voice

- What to say and in what order is your job: cut and reorder freely, and say what you cut.
- How it's said stays theirs. Their verbs and nouns are the default ("Built", "Cut", "Rebuilt", "turn to"). Change a word only when it blocks the point or compression. Never swap in a "stronger" synonym, and flag each word change with its reason.
- Don't introduce vocabulary they never use. Don't vary terms for elegance; repeat the same name.
- If the user bans more words or patterns, follow that for the rest of the session and offer to add them to this file.

## Never

**Words** (unless the user wrote them): spearheaded, leveraged, orchestrated, championed, utilized, facilitated, pioneered, revolutionized, catalyzed, empowered, drove (as in "drove adoption"), synergy, robust, seamless, frictionless, cutting-edge, innovative, pivotal, impactful, passionate, results-driven, proven track record, best practices (name the practice), end-to-end as filler, successfully, significantly, greatly. 中文：赋能、抓手、闭环、沉淀、拉通、聚焦、深度参与、全面提升、持续优化.

**Patterns:**
- Negative parallelism or reframes: "not X but Y", "not only X but also Y". Delete the negated half.
- Vague participle tails: ", ensuring…", ", enabling…", ", driving…". A tail stays only if it carries a concrete fact.
- "Through X, achieved Y" / "通过……实现……" chains.
- "serves as", "stands as", "represents" where "is" works.
- Puffery: "key", "critical", "significant" with no fact behind it. An intern who sounds like a VP.
- Naming or quoting the precedent, or buzzwords lifted from the target brief and pasted in. Frontier concepts appear only where the user really did that thing.

## Numbers

- Use only numbers in the sources, exactly as stated and with their scope ("60 users on launch day" is not "60 weekly users").
- Never estimate, round up, add "~", convert currency, or invent scale or percentages. No bullet needs a metric.
- With no number, end on a concrete fact: who uses it, what it replaced, what happens now that didn't before.
- Don't upgrade status: merged ≠ deployed, piloted ≠ adopted, proposed ≠ shipped, available ≠ enabled everywhere.
- The result tail states the new state or the gain, never the old failure ("stalled 10 minutes", "never worked"). A before-state appears only inside a from→to contrast that ends on the gain.
- A precedent never lends its scale. Evoking Tesla doesn't make 60 users sound like millions.

## Self-check before showing a draft

Per bullet: what is its one point, and does every clause serve it? Would a reader remember it after six seconds? Is the precedent felt but not recognizable? Any banned word or pattern? Did any of my words replace one of theirs without a reason?
Per section: are the skeletons varied? Is the strongest bullet first? Could one bullet go entirely?

---
Sources adapted: career-ops (MIT) `modes/_writing.md` and `voice-dna.template.md`; StoneLL1/resume-builder `Resume-Writing-Guide-LLM.md` §4.1, §9; dabydat/resume-builder-skill bullet length rules.
