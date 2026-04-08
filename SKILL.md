---
name: makino-writing-craft
invocation: user
description: "Writing Craft — Distilled writing methodology for clear, compelling long-form articles. 7 principles, 10 craft modules, 28-item checklist."
version: "1.0"
last_updated: "2026-04-08"
source: "Liu Junqiang, The Craft of Writing (2020)"
---

# Writing Craft — Write clear, write compelling

A distilled writing methodology extracted from Liu Junqiang's *The Craft of Writing* (34 万字, 29 chapters).
Reorganized by **writing action** (not by chapter) for practical use by AI writing assistants.

- Input: a draft, outline, or writing task
- Output: guided improvements at any stage (topic, structure, argument, style, self-check)
- NOT for: generating first drafts from scratch (use writer skills), academic paper formatting

## Commands

| Command | What it does |
|---------|-------------|
| `/makino-writing-craft` | Interactive: assess current draft stage, apply relevant craft modules |
| `/makino-writing-craft review <path>` | Review a draft against the full checklist |
| `/makino-writing-craft checklist` | Output the 28-item self-check checklist |
| `/makino-writing-craft principle <n>` | Explain principle N with examples |

## How this skill fits the writing pipeline

```
writer skill (makino-writer / jienima-writer / ai-xiahu-writer)
  calls → makino-writing-craft (as quality layer)
    ├── during outlining: topic + structure modules
    ├── during drafting: argument + narrative + style modules
    └── during review: full checklist
```

This skill is a **method library**, not a writer. It provides craft guidance that writer skills consume.
External users can also invoke it standalone for any writing task.

---

## Layer 1: Principles (Mindset)

7 core beliefs. Read these once, internalize, apply always.

### P1. Transparent Glass

Good writing is transparent glass — the reader sees the landscape behind it, not the glass itself.
Clarity over elegance. If the reader notices your prose style, you've failed.

**Anti-pattern**: purple prose, showing off vocabulary, "AI-flavored" flowery language.
**Test**: can a smart 15-year-old follow your argument?

### P2. Problem-Driven

Every article answers a question. No question, no article.
The question is the engine; everything else is fuel.

**Apply**: before writing, state your question in one sentence.
If you can't, you're not ready to write.

### P3. Reader's Perspective

Writing is not a diary. Switch from god-view to civilian-view.
Writing is fundamentally an act of empathy.

**4 angles**: ignoring readers (worst) → looking down → looking up → eye-level (best).
**Gift test**: good writing is like a good gift — chosen for the receiver, not the giver.

### P4. March's Three Principles

A good story balances three qualities (James March):
- **Interesting enough** to engage curiosity
- **Simple enough** to be understood
- **Credible enough** to be believed

If any one fails, the whole fails.

### P5. Tree-Shaped Argument

Arguments are trees, not lists.
- Root: main claim
- Branches: reasons (why should I believe this?)
- Leaves: evidence (how do you know?)

Every claim needs reasons. Every reason needs evidence. No floating assertions.

### P6. Tension is Story

Story = departure from the ordinary. The simplest definition: "Something happened!"
Tension comes in three forms:
- **Conflict**: opposing forces collide
- **Contrast**: opposites placed side by side
- **Paradox**: defying audience expectations

A paragraph without tension is a paragraph readers skip.

### P7. Courage to Cut

Material selection determines final quality.
Michelangelo: "The more stone wasted, the taller the statue."

Three cutting standards:
- **Relevant**: does it serve the main thread?
- **Proportional**: is the space allocation right?
- **Honest**: does it represent facts fairly?

---

## Layer 2: Craft Modules

10 modules, ordered by writing workflow. Each module is self-contained.

### C1. Topic Selection

**Goal**: find a question worth answering.

| Check | Rule |
|-------|------|
| Importance | Why should readers care? What's at stake? |
| Challenge | Can it be answered in one sentence? If yes, too easy |
| Novelty | What's new in my answer vs. existing answers? |

**5-question drill**:
1. Who cares about this?
2. Why do they care?
3. What answers already exist?
4. How is my answer different?
5. Why is mine better?

**Tip**: decompose big questions into actionable sub-questions.

### C2. Title Craft

**Goal**: a title that is understood in two reads and creates curiosity.

| Principle | Rule | Example |
|-----------|------|---------|
| Short > Long | Main title short and punchy; subtitle for details | "The Weakness of the Strong" |
| Concrete > Abstract | Paint a picture, not a concept | "When Everything Crumbles" vs "State Failure Analysis" |
| Question > Statement | Questions hook curiosity directly | "Who Will Survive?" |
| Tension > Flat | Conflict/contrast/paradox in the title | "Pricing the Priceless" |

**Ann Lander's ratio**: 90% appropriateness + 5% clarity + 5% drama.

**Anti-patterns**: jargon-stuffed academic titles, clickbait without substance, abstract concept pileups.

### C3. Structure

**Goal**: give the article a skeleton readers can follow.

**6 organizing patterns** (Royer):
1. Chronological (timeline)
2. Spatial (geography/scope)
3. Thematic (topic clusters)
4. Causal (cause → effect)
5. Comparative (A vs B)
6. Problem-Solution

**LOCK story structure** (for narrative articles):
- **L**ead: introduce the protagonist/subject
- **O**bjective: what they want to achieve
- **C**onfrontation: obstacles and conflicts
- **K**nockout: resolution with impact

**Practical rule**: outline the skeleton first, then fill non-linearly. Structure liberates the brain.

### C4. Argument

**Goal**: every claim supported, every support grounded.

**Toulmin model** (simplified):
```
Claim → because → Reason → based on → Evidence
         ↓                    ↓
     Qualifier            Rebuttal
   ("usually")        ("unless...")
```

| Trap | What it is | Fix |
|------|-----------|-----|
| Correlation ≠ Causation | Two things move together but one doesn't cause the other | Check for omitted variables, reverse causation |
| Cherry-picking | Only showing supporting evidence | Address counter-evidence explicitly |
| Floating assertion | Claim with no reason/evidence | Add the "why" and "how do you know" |

**Handle objections**: acknowledge the strongest counter-argument first, then explain why your position holds.

### C5. Narrative

**Goal**: make the reader feel, not just understand.

**Story elements**: character + events + sequence + point of view.

**4C framework**:
- **Causality**: events connected by cause-effect
- **Conflict**: protagonist faces obstacles
- **Complication**: plot thickens with twists
- **Character**: reader can relate to someone

**Kempton's story checklist**:
- Is it interesting?
- Does it educate?
- Does it surprise?
- Does it earn identification?
- Does it stir emotion?
- Does it challenge?
- Does it empower?

**Good stories trigger multiple emotional responses**: anxiety → excitement → satisfaction → awe.

### C6. Micro-Structure (Words & Sentences)

**Goal**: every sentence flows, every word earns its place.

**Word abstraction ladder**: prefer the basic level.
```
Life → Creature → Animal → Livestock → Horse → Palomino
(too abstract) ←————————————→ (too specific)
                    ↑ sweet spot (Horse, Apple, Table)
```

| Rule | Why | Anti-pattern |
|------|-----|-------------|
| Concrete nouns > Abstract nouns | Brain processes concrete faster | "sustainability paradigm" |
| Strong verbs > Weak verbs + adverbs | More vivid, more compact | "walked slowly" vs "shuffled" |
| Subject-verb clear | Reader knows who does what | Dangling modifiers, passive chains |
| Old → New information flow | Builds on what reader already knows | Random information order |
| Mix sentence lengths | Rhythm; short = punch, long = nuance | All same length = monotone |
| Active > Passive | Stronger, clearer | "Mistakes were made" |

**Bates Lunch Test**: can you explain your topic to a stranger over lunch? If not, you're writing for yourself.

### C7. Meso-Structure (Paragraphs & Sections)

**Goal**: each paragraph has one job; paragraphs connect logically.

- **Topic sentence first**: state the paragraph's point upfront
- **One paragraph, one idea**: if you find two ideas, split
- **Transitions**: bridge paragraphs with logical connectors (however, therefore, meanwhile)
- **Section rhythm**: vary paragraph lengths within a section

### C8. Framing

**Goal**: choose the right lens for your audience.

**Framing = choosing the camera angle.** Same facts, different frames, different impact.
"Fought and lost repeatedly" vs "Lost repeatedly but fought" — word order alone changes meaning.

**3-step framing process**:
1. **Position** your reader: who are they? What frameworks do they already hold?
2. **Distill** your thesis: one sentence, interesting + deep
3. **Crop** your material: only what serves the frame

**Audience differentiation**:
- Wide vs. narrow audience → adjust jargon level
- Expert vs. general → adjust depth vs. breadth
- Sympathetic vs. skeptical → adjust evidence weight

### C9. Reader Awareness

**Goal**: write for the reader, not for yourself.

**3 reader knowledge states** (and strategies):
| Reader knows... | Strategy |
|-----------------|----------|
| Nothing about the topic | Provide rich detail, open a window to the unknown |
| A little (most common) | Car-crash principle: hook what they think they know, reveal what they don't |
| A lot | Challenge assumptions, offer novel angles |

**Eye-level writing**: treat the reader as an equal. Not lecturing, not fawning.

### C10. Revision

**Goal**: transform the ugly first draft into a polished piece.

**3 stages of prose** (Walter Benjamin):
1. Musical (composing) — let ideas flow
2. Architectonic (building) — restructure, reorder
3. Textile (weaving) — polish word by word

**Practical revision steps**:
1. Read aloud: if you stumble, the reader will too
2. Cut 10%: force yourself to remove 10% of word count
3. Check every paragraph's topic sentence
4. Verify argument tree is complete (no floating claims)
5. Get a non-expert to read it

---

## Layer 3: Checklist

28 items across 7 categories. Use after completing a draft.

### Topic (4 items)
- [ ] Article answers a specific, stated question
- [ ] Reader has a reason to care about this question (importance)
- [ ] Question has depth — can't be answered in one sentence (challenge)
- [ ] My answer offers something new (novelty)

### Title (4 items)
- [ ] Title understood in two reads
- [ ] Title has concrete imagery (not abstract concept pileup)
- [ ] Title creates curiosity (question/tension/contrast)
- [ ] Title length appropriate (main title short, subtitle optional for detail)

### Structure (5 items)
- [ ] Article has a clear skeleton (can draw a structure diagram)
- [ ] Opening hooks within 30 seconds of reading
- [ ] Each paragraph has exactly one core point
- [ ] Paragraphs connect with logical transitions
- [ ] Ending lands with impact (not a fizzle)

### Argument (4 items)
- [ ] Every claim has supporting reasons
- [ ] Every reason has evidence/facts/data
- [ ] Causal claims withstand scrutiny (ruled out correlation traps)
- [ ] Major counter-arguments addressed

### Narrative (3 items)
- [ ] Article contains tension elements (conflict/contrast/paradox; at least one)
- [ ] Reader will feel an emotional response (curiosity/anxiety/satisfaction/awe)
- [ ] Stories serve the argument (not decoration)

### Style (6 items)
- [ ] Concrete words dominate (basic-level vocabulary)
- [ ] No hollow big words or abstract concept pileups
- [ ] Subject-verb relationships clear in every sentence
- [ ] Sentence lengths varied (short + long rhythm)
- [ ] Active voice predominates
- [ ] Reads smoothly aloud

### Reader (4 items)
- [ ] Accessible to non-expert readers (Bates Lunch Test)
- [ ] No unexplained jargon
- [ ] Eye-level tone (not lecturing, not fawning)
- [ ] Frame matches target audience

---

## Integration Guide

### For makino-writer / jienima-writer

Writer skills can reference this skill as a quality layer:

```
# In writer SKILL.md, add:
# Quality reference: makino-writing-craft Layer 2 (C1-C10) + Layer 3 checklist
```

Recommended integration points:
1. **Outline phase**: apply C1 (Topic) + C3 (Structure) + C8 (Framing)
2. **Draft phase**: apply C4 (Argument) + C5 (Narrative) + C6 (Micro-Structure)
3. **Review phase**: run full Layer 3 Checklist

### For standalone use

Anyone can invoke `/makino-writing-craft review` on any draft.
The skill will:
1. Identify the draft's current stage (outline / draft / near-final)
2. Apply relevant craft modules
3. Run applicable checklist items
4. Output specific, actionable suggestions (not vague "make it better")

---

## Gotchas

| Problem | Cause | Fix |
|---------|-------|-----|
| Skill outputs generic advice | Draft not read carefully | Always Read the full draft first, quote specific sentences when suggesting changes |
| Checklist feels mechanical | Applied all 28 items to a short piece | Scale checklist to article length: <2000 chars use 10 core items, full list for >5000 |
| Over-editing kills voice | Applying every micro-structure rule | Prioritize: argument tree > structure > style. Voice matters more than grammar |
| Conflict with writer skill style guide | Writing-craft says X, writer SSOT says Y | Writer skill's style guide (SSOT) wins on style; writing-craft wins on structure/argument |

---

## Source Attribution

Methodology distilled from:
- Liu Junqiang (刘军强), *The Craft of Writing* (写作是门手艺), Guangxi Normal University Press, 2020
- Referenced frameworks: Toulmin argument model, March's three principles, Kempton's story checklist, Royer's six structures, LOCK narrative model

This skill is an open-source interpretation for AI writing assistance. All intellectual credit belongs to the original authors.
