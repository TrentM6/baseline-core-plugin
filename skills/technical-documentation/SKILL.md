---
description: "Technical Documentation — User guides, help center articles, API docs, release notes, and how-to guides. Triggers: user guide, help center, API documentation, release notes, how-to guide, knowledge base, documentation, help docs, support article, changelog, onboarding docs, getting started guide"
---

# Technical Documentation

Technical documentation is the discipline of making products understandable. It bridges the gap between what the product can do and what users know how to do — through clear, structured, user-focused writing.

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — Product, positioning, terminology
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, language rules
- `${CLAUDE_PLUGIN_ROOT}/context/extended/formatting.md` — Document structure conventions

**Context (load when relevant):**
- `${CLAUDE_PLUGIN_ROOT}/context/extended/product.md` — Product features, workflows, current state
- `${CLAUDE_PLUGIN_ROOT}/context/extended/technical.md` — Tech stack, architecture, constraints

**References (load when needed):**
- `${CLAUDE_PLUGIN_ROOT}/skills/technical-documentation/references/documentation-standards.md` — Style guides, writing standards
- `${CLAUDE_PLUGIN_ROOT}/skills/technical-documentation/references/information-architecture.md` — Content organization, navigation

## Core Principles

1. **Write for the reader, not the product.** Users don't care how it works. They care how to use it.
2. **Task-oriented, not feature-oriented.** Organize around what users want to do, not what the product has.
3. **Scannable over comprehensive.** People scan docs looking for answers. Help them find it fast.
4. **Show, don't just tell.** Examples, screenshots, and code samples beat paragraphs of explanation.
5. **Keep it current.** Outdated docs are worse than no docs. Build update triggers into releases.
6. **Progressive disclosure.** Start simple. Let advanced users dig deeper.
7. **Test your docs.** Watch someone follow them. If they get stuck, the docs failed.

## Workflow

### 1. Clarify Before Starting
- What type of documentation?
- Who is the audience (technical level, context)?
- What task are they trying to complete?
- What format do they expect?
- What already exists?

### 2. Choose Document Type

| Type | Purpose | Audience |
|------|---------|----------|
| Getting Started | First-time onboarding | New users |
| How-To Guide | Complete a specific task | Users with basic knowledge |
| Reference | Look up specifications | Advanced users, developers |
| Conceptual | Understand how something works | All levels |
| Release Notes | What changed and why | Existing users |
| API Docs | Integrate with the product | Developers |

### 3. Writing Process

**Structure:** Outline before writing > organize by user task > use progressive disclosure.

**Write:** Lead with what they need to do > step-by-step instructions > include examples > note gotchas.

**Review:** Follow the steps yourself > test with a novice > check for accuracy > simplify language.

## Quality Checks

- [ ] Can a new user follow the instructions without help?
- [ ] Task-oriented (organized by what users do)?
- [ ] Scannable (headings, lists, short paragraphs)?
- [ ] Examples included?
- [ ] Accurate and up to date?
- [ ] Consistent terminology?
- [ ] Appropriate level of detail for audience?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Feature-oriented | Organize by user task |
| Wall of text | Use headings, lists, examples |
| Jargon without explanation | Define terms or use simpler language |
| Write once, forget | Build update triggers into releases |
| No examples | Always include examples |
