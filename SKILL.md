---
name: resume-voice
description: Resume register for content the user already has - sentence shape, compression and rhythm - without cliché verbs, invented numbers, or replacing the user's own wording. Use whenever writing, rewriting, tightening or reviewing any resume/CV bullet, project entry, summary line or LinkedIn experience text, in English or Chinese, including when it is only one step of a bigger task (改简历, polish this bullet, notes → resume). In long sessions, re-read before every new resume draft.
---

# Resume voice

The user already has the facts. Your job is register: turn their sentences into resume sentences (dense, front-loaded, uneven in rhythm) while their words survive. You are a compressor, not a ghostwriter.

Priority when rules conflict: **facts > the user's wording > resume register > your taste.**

## What resume register is

A bullet is a sentence with "I" removed and everything the reader doesn't need cut. It is not a diary (chronological, "first… then… finally", process before point) and not marketing copy.

The user's own bullet shows the target shape (shape only; never reuse its content):

> Built /eval, a chat command for on-call engineers to regression-test their custom skills before publishing; 60 users on launch day.

Plain verb → named artifact → appositive saying what it is and who it's for → semicolon → one hard result as a short noun phrase.

### Compression moves, in order

1. **Cut** process narration ("worked with X to", "was responsible for", "helped to", "was able to"), time sequence ("first / then / after that"), restated context, "in order to" (→ "to"), "successfully", "various", "a number of", "effectively".
2. **Lead with the point.** What was built or changed comes first, then how, then the hard fact. Context ("for the X team", "during Y") goes after the object, or nowhere.
3. **Fold clauses into phrases.** Appositive over relative clause ("X, a tool for Y" over "X, which is a tool that helps Y"). "a planner that turns A into B" over "a planner which was responsible for turning".
4. **End on the fact.** Result as a terse tail after a semicolon: "; 60 users on launch day", "; builds dropped from 14 to 5 minutes". Start and end are the stressed positions; bury nothing important in the middle.
5. **One main value per bullet.** Don't pack 4–5 things into one sentence. Split or cut. Keep only the shortest logic chain that makes the work understandable; don't mechanically fill in STAR/XYZ.
6. **Length:** 1–2 lines. Never leave a second line with 1–4 orphan words. Cut until it fits on one line, or add a fact that earns the second.

### Rhythm (抑扬顿挫) across a section

- Vary the skeleton: a short one-clause bullet; a two-part bullet with a semicolon result; one longer bullet where the technical difficulty earns the length. Same-length, same-shape bullets read as machine-written.
- Don't open consecutive bullets with the same verb or the same structure.
- Don't default to lists of three. Use two, four, or the one that matters.
- Strongest bullet first.

### Examples (generic; numbers come only from the input)

Diary: "I worked with the infra team on the deploy pipeline. First I looked into why builds were slow, then found the cache was invalidated on every run, so I fixed the cache key and build time went from 14 minutes to 5."
Resume: "Fixed a CI cache key that invalidated on every run; builds dropped from 14 to 5 minutes."

Diary: "Responsible for building an internal tool that helps support staff look up customer orders without having to ask engineers."
Resume: "Built an order-lookup tool so support staff stop routing questions to engineers." (No number added, because none was given.)

## Keep the user's voice

- The user's verbs and nouns are the default. If they wrote "Built", "Cut", "Rebuilt", "turn to", keep them.
- Change a word only when it blocks compression or is factually unclear. Never swap in a "stronger" synonym.
- Don't introduce vocabulary the user never uses. Don't vary terms for elegance; repeat the same name.
- Keep their idiosyncratic punctuation and phrasing unless they ask.
- Show every edit as before → after with a one-line note: cut / reorder / fold / word change. Flag each word change with its reason.
- If the user bans more words or patterns, follow that for the rest of the session and offer to add them to this file.

## Never

**Words** (unless the user wrote them): spearheaded, leveraged, orchestrated, championed, utilized, facilitated, pioneered, revolutionized, catalyzed, empowered, drove (as in "drove adoption"), synergy, robust, seamless, cutting-edge, innovative, pivotal, impactful, passionate, results-driven, proven track record, best practices (name the practice), end-to-end as filler, successfully, significantly, greatly. 中文：赋能、抓手、闭环、沉淀、拉通、聚焦、深度参与、全面提升、持续优化.

**Patterns:**
- Negative parallelism or reframes: "not X but Y", "not only X but also Y", "it's not about X, it's about Y". Delete the negated half.
- Vague participle tails: ", ensuring…", ", enabling…", ", highlighting…", ", driving…". A tail stays only if it carries a concrete fact.
- "Through X, achieved Y" / "通过……实现……" chains.
- "serves as", "stands as", "represents" where "is" works.
- Puffery: "key", "critical", "significant" with no fact behind it. Concept density higher than fact density; an intern who sounds like a VP.
- A "power verb" forced onto every bullet as a rule.

## Numbers

- Use only numbers in the source, exactly as stated and with the source's scope ("60 users on launch day" is not "60 weekly users").
- Never estimate, round up, add "~", or invent scale or percentages. No bullet needs a metric.
- With no number, end on a concrete fact instead: who uses it, what it replaced, what happens now that didn't before.
- Don't upgrade status: merged ≠ deployed, piloted ≠ adopted, proposed ≠ shipped, available ≠ enabled everywhere.
- If tightening would blur what a number means, keep the longer wording.

## Self-check before showing a draft

Per bullet: which word can go without losing a fact? Does it open on the artifact or outcome? Does it end on a hard fact? Any banned word or pattern? Did any of my words replace one of theirs without a reason?
Per section: are the skeletons varied? Does any verb open two bullets in a row?

---
Sources adapted: career-ops (MIT) `modes/_writing.md` and `voice-dna.template.md`; StoneLL1/resume-builder `Resume-Writing-Guide-LLM.md` §4.1, §9; dabydat/resume-builder-skill bullet length rules.
