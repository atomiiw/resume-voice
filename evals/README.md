# Regression test for resume-voice

`rubric.md` is the judge rubric; `samples.md` holds the labelled positive and negative samples. `judges.md` defines five blind judges. `writer-prompt.md` is the writer's brief.

`private/` holds the user's facts, target brief and run logs. It is gitignored because it contains employer-internal details. To run the test on your own material, create `private/facts-<experience>.md` and `private/target-<role>.md` in the same shape.

Loop:
1. Calibrate all five judges on the labelled samples.
2. Fresh writer agent: SKILL.md + facts + target → bullets.
3. Five fresh judge agents score the bullets.
4. Any FAIL: decide whether the skill has a gap (fix SKILL.md) or the writer slipped (log it). Rerun.
5. Done after two consecutive clean rounds with different writer agents. Cap at five rounds.
