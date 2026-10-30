# resume-voice

A Claude Code / agent skill that turns content you already have into resume bullets:

1. Reads the target role, company and industry: what reads as frontier there, and what kind of person they celebrate.
2. Picks the one memorable point per bullet and the industry precedent it echoes.
3. Interviews you one question at a time for the details that amplify that point.
4. Writes tight, rhythmic bullets that evoke the precedent without naming it.

It does not add cliché verbs, invent numbers, or replace your own wording.

## Install

```bash
git clone https://github.com/atomiiw/resume-voice.git ~/.claude/skills/resume-voice
```

The skill loads automatically for any resume, CV or LinkedIn writing task. You can also call it directly with `/resume-voice`.

See [SKILL.md](SKILL.md) for the rules.
