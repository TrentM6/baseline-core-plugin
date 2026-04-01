---
description: "Skill Building — Creating new skills, documenting expertise, and building skill reference files. Triggers: create a skill, new skill, build a skill, document expertise, skill architecture, skill template, add a new skill to the system"
---

# Skill Building

Skill building is the meta-skill of creating new skills for the Baseline System. It's about capturing domain expertise in a structured, reusable format that AI tools can execute consistently.

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — System terminology, positioning
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, language rules

**References (load when needed):**
- `${CLAUDE_PLUGIN_ROOT}/skills/skill-building/references/skill-architecture.md` — Skill structure, file formats, quality standards

## Core Principles

1. **Skills encode expertise, not instructions.** A skill captures how an expert thinks about a domain, not just a checklist.
2. **Specificity over generality.** A skill for "writing PRDs" is more useful than one for "writing."
3. **Principles drive quality.** Checklists catch errors. Principles prevent them.
4. **Test with real tasks.** A skill that hasn't been used on real work isn't done.
5. **Reference material adds depth.** The skill file provides methodology. References provide detail.
6. **Iterate based on output quality.** The measure of a skill is the quality of work it produces.

## Workflow

### 1. Clarify Before Starting
- What domain does this skill cover?
- What tasks will it be used for?
- Who is the target user?
- What expertise should it encode?
- What frameworks apply?

### 2. Skill Architecture

A complete skill consists of:

**Skill File (SKILL.md):**
- Description with trigger phrases
- Core principles (7-12)
- Workflow steps
- Quality checks
- Anti-patterns
- File loading instructions

**References (references/):**
- Detailed frameworks and methods
- Templates and examples
- Domain-specific knowledge

**Manifest (in the description):**
- What frameworks to load
- What context files to load
- What references are available

### 3. Building Process

1. **Research the domain** — Study how experts approach this work
2. **Identify principles** — What separates good from great in this domain?
3. **Design the workflow** — What steps does an expert follow?
4. **Create quality checks** — How do you know the output is good?
5. **Write reference materials** — Detailed guidance for specific situations
6. **Test with real tasks** — Use the skill on actual work
7. **Iterate** — Improve based on output quality

## Quality Checks

- [ ] Principles capture expert thinking (not just common sense)?
- [ ] Workflow is complete and actionable?
- [ ] Quality checks catch real problems?
- [ ] Anti-patterns reflect actual mistakes?
- [ ] References add depth beyond the skill file?
- [ ] Tested on real tasks?
- [ ] Under 3,000 words (detailed content in references)?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Checklist without principles | Principles that guide judgment |
| Too generic | Specific to the domain |
| Never tested | Always test with real work |
| All in one file | Skill file + references |
| Copied from templates | Encode actual expertise |
