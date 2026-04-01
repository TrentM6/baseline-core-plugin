---
description: "UX Design — Interface design, wireframes, user flows, UI copy, design systems, and accessibility. Triggers: interface design, wireframes, user flows, UI copy, design systems, accessibility, UX audit, interaction design, user journey, information architecture, design critique, usability, UI design, mockup, prototype design"
---

# UX Design

UX design is the discipline of understanding users deeply and crafting experiences that serve their needs with clarity and intention. It spans research, strategy, and execution — from discovering what users need to designing interfaces that make complex tasks feel effortless.

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern
- `${CLAUDE_PLUGIN_ROOT}/frameworks/ux-heuristics.md` — Nielsen's heuristics, WCAG, cognitive load

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — Product, positioning
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, language rules
- `${CLAUDE_PLUGIN_ROOT}/context/extended/design.md` — Design system, colors, typography, visual standards

**References (load when needed):**
- `${CLAUDE_PLUGIN_ROOT}/skills/ux-design/references/ux-methods.md` — Journey mapping, personas, IA methods
- `${CLAUDE_PLUGIN_ROOT}/skills/ux-design/references/design-principles.md` — Gestalt, hierarchy, affordance
- `${CLAUDE_PLUGIN_ROOT}/skills/ux-design/references/ui-patterns.md` — Navigation, forms, data display, mobile
- `${CLAUDE_PLUGIN_ROOT}/skills/ux-design/references/design-systems.md` — Component systems, tokens, documentation
- `${CLAUDE_PLUGIN_ROOT}/skills/ux-design/references/design-critique.md` — Critique frameworks
- `${CLAUDE_PLUGIN_ROOT}/skills/ux-design/references/ideation-methods.md` — Brainstorming, sketching, Crazy 8s

## Core Principles

1. **Research before pixels.** Don't design until you understand the user's world.
2. **Clarity is kindness.** Every moment of confusion is a design failure.
3. **Design for the worst case.** The real user is distracted, tired, on bad wifi.
4. **Constraints unlock creativity.** Limits force better solutions.
5. **Test early, test ugly.** A sketch tested with users beats a polished mockup never validated.
6. **Ship to learn.** Real usage teaches things research never can.
7. **Advocate, but collaborate.** Fight for user needs, understand business realities.

## Workflow

### 1. Clarify Before Starting
- What's the design challenge?
- Who are the users? What do they need?
- What constraints exist (technical, business, time)?
- What does success look like?
- What already exists?

### 2. Choose the Right Approach

| Situation | Approach |
|-----------|----------|
| New product/feature | Discovery > IA > wireframes > prototype > test |
| Improving existing | Audit > identify issues > redesign > test |
| Design system work | Inventory > standards > components > documentation |
| Quick iteration | Sketch > test > refine |

### 3. Design Process

**Understand:** Research users, map current experience, identify pain points, define success metrics.

**Explore:** Generate multiple concepts, sketch broadly before narrowing, consider edge cases early.

**Define:** Choose direction, create detailed wireframes, define interactions and states, write UI copy.

**Validate:** Test with users, iterate on feedback, check against heuristics.

## Quality Checks

- [ ] Solves the identified user problem?
- [ ] Works for edge cases and error states?
- [ ] Accessible (WCAG 2.1 AA)?
- [ ] Consistent with existing patterns?
- [ ] Passes Nielsen's heuristics review?
- [ ] Content is clear and helpful?
- [ ] Works across device sizes?
- [ ] User can recover from errors?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Pixel-perfect too early | Start rough, refine with feedback |
| Designing in isolation | Collaborate with eng and product |
| Ignoring edge cases | Design the unhappy path too |
| Skipping user testing | Always validate with real users |
| Copy-paste patterns | Understand why a pattern works |
