---
description: "Prototyping — Coded prototypes, demos, POCs, clickable mockups, and technical feasibility proofs. Triggers: prototype, demo, POC, proof of concept, clickable mockup, coded prototype, technical feasibility, build a demo, quick prototype, interactive mockup, MVP prototype"
---

# Prototyping

Prototyping is the discipline of making ideas tangible quickly. It's about learning through building — creating just enough of something that you can see it, click it, test it, and learn from it before committing to full implementation.

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — Product, positioning
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, language rules
- `${CLAUDE_PLUGIN_ROOT}/context/extended/design.md` — Design system, colors, typography, visual standards

**Context (load when relevant):**
- `${CLAUDE_PLUGIN_ROOT}/context/extended/product.md` — Product features, workflows, current state
- `${CLAUDE_PLUGIN_ROOT}/context/extended/technical.md` — Tech stack, architecture, constraints

**References (load when needed):**
- `${CLAUDE_PLUGIN_ROOT}/skills/prototyping/references/prototyping-tools.md` — Tool selection guide
- `${CLAUDE_PLUGIN_ROOT}/skills/prototyping/references/prototyping-methods.md` — Fidelity levels, methods

## Core Principles

1. **Build to learn, not to ship.** Prototypes answer questions. They're not the product.
2. **Fidelity matches the question.** Paper for concepts. Code for interactions. Don't over-build.
3. **Speed over polish.** The faster you can test an idea, the faster you learn.
4. **Throw it away.** Prototypes are disposable. Don't get attached.
5. **Real enough to test.** If users can't react to it meaningfully, it's not real enough.
6. **One question per prototype.** Focus. Test one thing at a time.

## Workflow

### 1. Clarify Before Starting
- What question does this prototype need to answer?
- Who will test/review it?
- What's the right fidelity level?
- What are the technical constraints?
- What's the timeline?

### 2. Choose Fidelity Level

| Fidelity | When | Tools |
|----------|------|-------|
| Low (sketches, paper) | Exploring concepts | Paper, whiteboard |
| Medium (wireframes, clickable) | Testing flows | Figma, basic HTML |
| High (coded, realistic) | Testing interactions, selling vision | React, HTML/CSS/JS |

### 3. Build Process
1. Scope ruthlessly — what's the minimum to answer the question?
2. Start with the core interaction
3. Add just enough context for testing
4. Test as soon as it's "real enough"
5. Document what you learned
6. Decide: iterate, pivot, or proceed to build

## Quality Checks

- [ ] Answers the specific question it was built to test?
- [ ] Realistic enough for meaningful feedback?
- [ ] Scoped to the minimum needed?
- [ ] Tested with representative users?
- [ ] Learnings documented?
- [ ] Clear decision on next steps?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Over-building | Match fidelity to the question |
| Getting attached | Prototypes are disposable |
| Testing too many things | One question per prototype |
| Skipping testing | Always test with users |
| Prototype becomes the product | Plan to throw it away |
