---
description: "Product Design — UX design, interface design, wireframes, user flows, prototyping, coded demos, UI copy, design systems, and accessibility. Triggers: design, interface design, wireframes, user flows, UI copy, design systems, accessibility, UX audit, interaction design, user journey, information architecture, prototype, demo, POC, proof of concept, clickable mockup, coded prototype, mockup, UI design, usability"
---

# Product Design

Product design spans the full spectrum from understanding users to building tangible prototypes. It combines UX thinking — research, information architecture, interaction design — with prototyping — making ideas real enough to test, validate, and learn from. The goal is always the same: craft experiences that serve user needs with clarity and intention.

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern
- `${CLAUDE_PLUGIN_ROOT}/frameworks/ux-heuristics.md` — Nielsen's heuristics, WCAG, cognitive load
- `${CLAUDE_PLUGIN_ROOT}/frameworks/research.md` — Research methods for discovery, validation, and usability testing

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — Product, positioning
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, language rules
- `${CLAUDE_PLUGIN_ROOT}/context/extended/design.md` — Design system, colors, typography, visual standards

**Context (load when relevant):**
- `${CLAUDE_PLUGIN_ROOT}/context/extended/product.md` — Product features, workflows, current state
- `${CLAUDE_PLUGIN_ROOT}/context/extended/users.md` — User personas, goals, pain points
- `${CLAUDE_PLUGIN_ROOT}/context/extended/technical.md` — Tech stack, architecture, constraints

**References (load when needed):**
- `${CLAUDE_PLUGIN_ROOT}/skills/product-design/references/ux-methods.md` — Journey mapping, personas, IA methods
- `${CLAUDE_PLUGIN_ROOT}/skills/product-design/references/design-principles.md` — Gestalt, hierarchy, affordance
- `${CLAUDE_PLUGIN_ROOT}/skills/product-design/references/ui-patterns.md` — Navigation, forms, data display, mobile
- `${CLAUDE_PLUGIN_ROOT}/skills/product-design/references/design-systems.md` — Component systems, tokens, documentation
- `${CLAUDE_PLUGIN_ROOT}/skills/product-design/references/design-critique.md` — Critique frameworks
- `${CLAUDE_PLUGIN_ROOT}/skills/product-design/references/ideation-methods.md` — Brainstorming, sketching, Crazy 8s
- `${CLAUDE_PLUGIN_ROOT}/skills/product-design/references/prototyping-tools.md` — Tool selection guide
- `${CLAUDE_PLUGIN_ROOT}/skills/product-design/references/prototyping-methods.md` — Fidelity levels, methods

## Core Principles

1. **Research before pixels.** Don't design until you understand the user's world.
2. **Clarity is kindness.** Every moment of confusion is a design failure.
3. **Design for the worst case.** The real user is distracted, tired, on bad wifi.
4. **Fidelity matches the question.** Paper for concepts. Code for interactions. Don't over-build.
5. **Build to learn, not to ship.** Prototypes answer questions. They're not the product.
6. **Test early, test ugly.** A sketch tested with users beats a polished mockup never validated.
7. **Constraints unlock creativity.** Limits force better solutions.
8. **Ship to learn.** Real usage teaches things research never can.

## Workflow

### 1. Clarify Before Starting
- What's the design challenge?
- Who are the users? What do they need?
- What constraints exist (technical, business, time)?
- What does success look like?
- What already exists?
- What question does this need to answer?

### 2. Choose the Right Approach

| Situation | Approach |
|-----------|----------|
| New product/feature | Discovery → IA → wireframes → prototype → test |
| Improving existing | Audit → identify issues → redesign → test |
| Design system work | Inventory → standards → components → documentation |
| Quick iteration | Sketch → test → refine |
| Validating a concept | Low-fi prototype → test with users → decide |
| Selling a vision | High-fi prototype → demo to stakeholders |
| Technical feasibility | Coded POC → evaluate constraints |

### 3. Design Process

**Understand:** Research users, map current experience, identify pain points, define success metrics. Load users.md and product.md for existing context.

**Explore:** Generate multiple concepts, sketch broadly before narrowing, consider edge cases early. Use ideation methods for structured brainstorming.

**Define:** Choose direction, create detailed wireframes, define interactions and states, write UI copy. Apply design.md for visual consistency.

**Build:** Choose the right fidelity level for the question being answered:

| Fidelity | When | What You Get |
|----------|------|-------------|
| Low (sketches, wireframes) | Exploring concepts, testing IA | Quick layout validation |
| Medium (clickable wireframes) | Testing flows, getting buy-in | Interactive walkthrough |
| High (coded prototype) | Testing interactions, selling vision | Realistic, testable demo |

**Validate:** Test with users, iterate on feedback, check against heuristics. Document what you learned. Decide: iterate, pivot, or proceed to build.

### 4. When Building Prototypes
1. Scope ruthlessly — what's the minimum to answer the question?
2. Start with the core interaction
3. Load technical.md to match the real stack when building coded prototypes
4. Add just enough context for testing
5. Test as soon as it's "real enough"
6. Document learnings and next steps

## Quality Checks

- [ ] Solves the identified user problem?
- [ ] Works for edge cases and error states?
- [ ] Accessible (WCAG 2.1 AA)?
- [ ] Consistent with design system (design.md)?
- [ ] Passes Nielsen's heuristics review?
- [ ] Content is clear and helpful?
- [ ] Works across device sizes?
- [ ] User can recover from errors?
- [ ] Prototype answers the specific question it was built to test?
- [ ] Fidelity matches the question being asked?
- [ ] Learnings documented and next steps clear?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Pixel-perfect too early | Start rough, refine with feedback |
| Designing in isolation | Collaborate with eng and product |
| Ignoring edge cases | Design the unhappy path too |
| Skipping user testing | Always validate with real users |
| Copy-paste patterns blindly | Understand why a pattern works |
| Over-building prototypes | Match fidelity to the question |
| Getting attached to prototypes | They're disposable — plan to throw them away |
| Testing too many things at once | One question per prototype |
