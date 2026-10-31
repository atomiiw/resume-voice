# Writer prompt

You are given three files and nothing else: `SKILL.md`, a facts file, and a target brief. Read all three fully, then write the bullets for the experience in the facts file.

Rules:
- Follow `SKILL.md` exactly. Its §1 register spec and §6 failure modes are binding.
- Use only facts in the facts file. Where the facts file marks a number as unconfirmed or an opinion, do not use it.
- Steps 2–4 of the workflow are done for you: the target brief is step 2; the facts file contains the one point and precedent per bullet (step 3) and the interview answers (step 4). Start at step 5, then run step 6 yourself before returning.
- Return exactly: the bullets in order, then one line under each giving the one point and what was cut. Nothing else.
