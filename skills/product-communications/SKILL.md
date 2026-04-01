---
description: "Product Communications — PRDs, product briefs, feature specs, stakeholder updates, launch briefs, and decision docs. Triggers: PRD, product requirements document, product brief, feature spec, stakeholder update, launch brief, decision doc, write a PRD, engineering handoff, product spec, status update, launch communication"
---

# Product Communications

Product communications is writing documents that move work forward. PRDs, specs, briefs, and updates that align teams, capture decisions, and enable execution. Good product docs reduce meetings, prevent misalignment, and create shared understanding.

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern
- `${CLAUDE_PLUGIN_ROOT}/frameworks/stakeholder-communication.md` — Stakeholder communication frameworks

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — Product terminology, positioning
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, writing style
- `${CLAUDE_PLUGIN_ROOT}/context/extended/formatting.md` — Document structure conventions

**Context (load when relevant):**
- `${CLAUDE_PLUGIN_ROOT}/context/extended/product.md` — Product features, workflows, current state

**References (load when the task needs detailed guidance):**
- `${CLAUDE_PLUGIN_ROOT}/skills/product-communications/references/document-templates.md` — PRD, brief, spec templates
- `${CLAUDE_PLUGIN_ROOT}/skills/product-communications/references/communication-dynamics.md` — Audience adaptation, executive summaries

## Core Principles

1. **Write to decide, not to document.** Best product docs force clarity and drive decisions.
2. **Audience determines format.** Engineers need different detail than executives.
3. **Start with the why.** Every doc answers "why are we doing this?" before "what."
4. **Explicit over implicit.** Assumptions, trade-offs, out-of-scope items belong in the doc.
5. **Living documents, not artifacts.** Date updates, note changes, keep current.
6. **Brevity is respect.** Say what needs said in as few words as possible.
7. **Async-first.** Write docs that work without you in the room.

## Document Types

| Document | Purpose | Audience | Length |
|----------|---------|----------|--------|
| **Product Brief** | Align on opportunity and direction | Leadership, cross-functional | 1-2 pages |
| **PRD** | Define what to build and why | Engineering, design, QA | 3-8 pages |
| **Feature Spec** | Technical detail for implementation | Engineering | Variable |
| **Stakeholder Update** | Communicate progress and decisions | Leadership | 1 page max |
| **Launch Brief** | Coordinate go-to-market | Cross-functional | 1-2 pages |
| **Decision Doc** | Capture and communicate a decision | Anyone affected | 1 page |

## Workflow

### 1. Clarify Before Starting
- What type of document?
- Who is the audience?
- What decision does this enable?
- What do they already know?
- What's the timeline?

### 2. Writing Process
**Structure First:** Choose type > outline sections > identify known vs. needs research > get structure reviewed.

**Draft:** Start with context and problem (the "why") > core content > supporting detail > explicit trade-offs and out-of-scope.

**Review:** Read as if you have no context > cut ruthlessly > check for ambiguity > verify accuracy.

**Finalize:** Add version/date > note open questions > specify next steps and owners.

## Quality Checks

- [ ] Can someone with no context understand the key points?
- [ ] Is the "why" clear before the "what"?
- [ ] Success criteria defined?
- [ ] Scope explicitly stated (in and out)?
- [ ] Trade-offs acknowledged?
- [ ] Open questions listed with owners?
- [ ] Right level of detail for the audience?
- [ ] Facts and figures verified?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Solution-first | Problem before solution, always |
| Kitchen sink | Right level of detail for the audience |
| Write once, abandon | Living document with update dates |
| No clear ask | Every doc needs "so what now?" |
| Template worship | Adapt format to the need |
