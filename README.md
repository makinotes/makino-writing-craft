# makino-writing-craft

Distilled writing methodology for AI writing assistants. 7 principles, 10 craft modules, 28-item checklist.

Extracted from Liu Junqiang's *The Craft of Writing* (写作是门手艺, 34万字, 29 chapters), reorganized by **writing action** for practical use.

## What it does

This is a **method library**, not a content generator. It provides structured writing guidance that any AI writing assistant can consume.

- **Layer 1: Principles** — 7 core beliefs (transparent glass, problem-driven, reader perspective, etc.)
- **Layer 2: Craft Modules** — 10 actionable modules from topic selection to revision
- **Layer 3: Checklist** — 28-item self-check across 7 categories

## Quick start

Install the skill into your Claude Code project:

```bash
# Copy SKILL.md to your skills directory
cp SKILL.md /path/to/your/.claude/skills/makino-writing-craft/SKILL.md
```

Then invoke:
```
/makino-writing-craft              # Interactive mode
/makino-writing-craft review       # Review a draft
/makino-writing-craft checklist    # Print the 28-item checklist
```

## Integration with writer skills

This skill works as a quality layer for existing writer skills:

```
your-writer-skill
  ├── outline phase → C1 (Topic) + C3 (Structure) + C8 (Framing)
  ├── draft phase   → C4 (Argument) + C5 (Narrative) + C6 (Micro-Structure)
  └── review phase  → Full Layer 3 Checklist
```

## Key frameworks included

| Framework | Source | Used for |
|-----------|--------|----------|
| Transparent Glass | Liu Junqiang | Style principle |
| March's Three Principles | James March | Story quality test |
| Toulmin Model | Stephen Toulmin | Argument structure |
| LOCK Structure | James Scott Bell | Narrative skeleton |
| Kempton Checklist | Mark Kempton | Story quality check |
| Abstraction Ladder | S.I. Hayakawa | Word choice |
| Bates Lunch Test | Robert H. Bates | Readability check |

## License

MIT

## Credits

Methodology from: Liu Junqiang (刘军强), *The Craft of Writing*, Guangxi Normal University Press, 2020.
This skill is an open-source distillation for AI writing assistance. All intellectual credit belongs to the original author.
