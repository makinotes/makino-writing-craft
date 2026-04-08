<div align="center">

# makino-writing-craft — Write clear, write compelling

> 一本 34 万字写作方法论，蒸馏成 7 条原则 + 10 个模块 + 28 项自检清单，给 AI 写作助手当质量层用。

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](LICENSE)
[![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-5A67D8.svg)](https://docs.anthropic.com/en/docs/agents-and-tools/claude-code/skills)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-gray.svg)](https://github.com/anthropics/claude-code)

[Features](#features) · [Install](#install) · [Usage](#usage) · [Frameworks](#key-frameworks-included) · [FAQ](#faq)

</div>

---

## Features

This is a **method library**, not a content generator. It provides structured writing guidance that any AI writing assistant can consume.

- **Layer 1: Principles** — 7 core beliefs (transparent glass, problem-driven, reader perspective, etc.)
- **Layer 2: Craft Modules** — 10 actionable modules from topic selection to revision
- **Layer 3: Checklist** — 28-item self-check across 7 categories

## Install

```bash
cd ~/.claude/skills/
git clone https://github.com/makinotes/makino-writing-craft.git
```

Then type `/makino-writing-craft` in Claude Code.

## Usage

```
/makino-writing-craft              # Interactive: assess draft stage, apply relevant modules
/makino-writing-craft review       # Review a draft against the full checklist
/makino-writing-craft checklist    # Print the 28-item self-check checklist
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

## FAQ

**Q: Is this a writer or a method library?**
Method library. It doesn't generate drafts — it provides craft guidance that writer skills consume. You can also use it standalone to review any draft.

**Q: What model works best?**
Any reasoning-capable model. The skill itself is just structured guidance — the model applies it to your draft.

**Q: Can I use this for non-Chinese writing?**
Yes. All principles and modules are language-agnostic. The checklist works for any prose.

## Update

```bash
cd ~/.claude/skills/makino-writing-craft && git pull
```

## License

Apache 2.0 — see [LICENSE](LICENSE) and [NOTICE](NOTICE)

## Credits

Methodology from: Liu Junqiang (刘军强), *The Craft of Writing* (写作是门手艺), Guangxi Normal University Press, 2020.
This skill is an open-source distillation for AI writing assistance. All intellectual credit belongs to the original author.

## Community & Contact

| | |
|---|---|
| ![飞书交流群](assets/feishu-group-qr.jpg) | ![马奇诺公众号](assets/wechat-qr-makino.jpg) |
| **飞书交流群** — 使用问题、Bug 反馈、功能建议 | **公众号「马奇诺」** — AI/Data/PKM 实践，后台留言也可以反馈 |

## Author

[makino](https://github.com/makinotes)
