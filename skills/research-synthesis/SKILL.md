---
description: "Research & Synthesis — User research, interviews, surveys, competitive analysis, and synthesis. Triggers: user research, interviews, synthesis, discovery interviews, validation testing, competitive analysis, research planning, research reports, user interviews, understand users, customer research, interview guide, usability testing, survey design"
---

# Research & Synthesis

Research & Synthesis is the discipline of understanding users deeply through structured inquiry and turning raw observations into actionable insights. It spans discovery, validation, and synthesis.

## Before You Start

Load the following files to execute this skill properly:

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern
- `${CLAUDE_PLUGIN_ROOT}/frameworks/research.md` — Research methodologies

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — Product, positioning, terminology
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, language rules

**Context (load when relevant):**
- `${CLAUDE_PLUGIN_ROOT}/context/extended/users.md` — User personas, goals, pain points
- `${CLAUDE_PLUGIN_ROOT}/context/extended/competitive.md` — Competitors, market positioning

**References (load when the task needs detailed guidance):**
- `${CLAUDE_PLUGIN_ROOT}/skills/research-synthesis/references/interview-guide.md` — Interview guide creation
- `${CLAUDE_PLUGIN_ROOT}/skills/research-synthesis/references/research-report.md` — Research report writing
- `${CLAUDE_PLUGIN_ROOT}/skills/research-synthesis/references/validation-report.md` — Validation report writing
- `${CLAUDE_PLUGIN_ROOT}/skills/research-synthesis/references/synthesis-methods.md` — Affinity mapping, thematic analysis
- `${CLAUDE_PLUGIN_ROOT}/skills/research-synthesis/references/competitive-analysis.md` — Competitive landscape mapping

## Core Principles

1. **Research before recommendations.** Understand the problem space first.
2. **Evidence over opinion.** Ground every insight in data. Quote users. Show your work.
3. **Actionable or it's not an insight.** Every finding must answer "so what?"
4. **Honest findings, even when uncomfortable.** Report what you found, not what stakeholders want to hear.
5. **Appropriate rigor for the stakes.** Match methodology to the question.
6. **Past behavior, not hypotheticals.** "Tell me about the last time..." beats "Would you ever..."
7. **Follow the energy.** When participants lean in, go deeper.
8. **Confidence levels matter.** "5 of 5 struggled" is different from "2 of 5 mentioned."

## Workflow

### 1. Clarify Before Starting

- **What decision are we trying to make?** Specific question, not vague curiosity
- **What do we need to learn?** What information would change the decision?
- **Who are we researching?** Specific user segment or persona
- **What do we already know?** Existing data, past research, assumptions
- **What's the timeline?** When does this decision need to be made?
- **What's the output?** Report, presentation, working session?

### 2. Choose the Right Method

| Goal | Method | Sample Size |
|------|--------|-------------|
| Understand problems and needs | Discovery interviews | 6-12 |
| Test if a solution resonates | Validation interviews | 5-8 |
| Test usability of existing product | Usability testing | 5-7 |
| Quantify attitudes or preferences | Survey | 100+ |
| Understand competitive landscape | Competitive analysis | 5-10 competitors |

### 3. Prepare Research Materials

**For interviews:** Define participant criteria, create screener questions, write interview guide, plan logistics.

**For validation:** Clarify what you're testing, confirm problem exists, prepare materials, define success criteria.

### 4. Conduct Research

- Stay neutral — don't lead or validate
- Ask about past behavior, not hypotheticals
- Follow the energy — go deeper when they engage
- Capture verbatim quotes (exact words matter)
- Note non-verbal reactions and hesitations
- Let silence work

### 5. Synthesize Findings

**The synthesis ladder:**

| Level | Question | Example |
|-------|----------|---------|
| Observation | What did you see/hear? | "3 of 5 users clicked Settings first" |
| Pattern | What keeps coming up? | "Users expect settings to be primary navigation" |
| Insight | What does this mean? | "Users come with specific tasks, not to explore" |
| Implication | So what should we do? | "Optimize for task completion, not discovery" |

### 6. Deliver Findings

All deliverables should include: research question and methodology, key findings with evidence, confidence levels, specific actionable recommendations, and next steps.

## Competitive Intelligence

Use competitive analysis when entering a new market, positioning a product, prioritizing features, or identifying differentiation opportunities.

**Process:** Define scope (direct, indirect, adjacent) > Gather information (product, marketing, reviews, pricing) > Analyze systematically > Synthesize into insights.

## Quality Checks

- [ ] Research question clearly stated?
- [ ] Method matches the question?
- [ ] Sample size sufficient?
- [ ] Questions open and non-leading?
- [ ] Findings grounded in evidence?
- [ ] Confidence levels stated?
- [ ] Recommendations specific and actionable?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Leading questions | Ask open, neutral questions |
| Confirmation bias | Actively seek disconfirming data |
| Solution-first | Always confirm problem first |
| Hypothetical questions | Ask about past behavior |
| Cherry-picking quotes | Show the full picture |
| Skipping synthesis | Always synthesize into themes |
