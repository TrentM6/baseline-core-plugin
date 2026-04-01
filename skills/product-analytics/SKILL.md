---
description: "Product Analytics — Metrics, dashboards, funnel analysis, retention, A/B tests, and segmentation. Triggers: metrics, dashboards, funnel analysis, retention analysis, A/B tests, segmentation, analytics strategy, KPIs, measurement framework, experiment design, data storytelling, product metrics, conversion funnel, cohort analysis"
---

# Product Analytics

Product analytics turns data into product decisions. It's the discipline of defining what to measure, instrumenting products to capture it, analyzing patterns, and telling stories that drive action.

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — Product, positioning
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, language rules

**References (load when needed):**
- `${CLAUDE_PLUGIN_ROOT}/skills/product-analytics/references/metrics-framework.md` — North Star, HEART, pirate metrics
- `${CLAUDE_PLUGIN_ROOT}/skills/product-analytics/references/experimentation-guide.md` — A/B testing, statistical significance
- `${CLAUDE_PLUGIN_ROOT}/skills/product-analytics/references/data-storytelling.md` — Visualization, narrative, presenting data

## Core Principles

1. **Measure what matters, not what's easy.** Vanity metrics feel good but don't drive decisions.
2. **Decisions, not dashboards.** Analytics exists to inform action, not to look impressive.
3. **Context makes data meaningful.** A number without context is just a number.
4. **Correlation is not causation.** Be rigorous about what data can and cannot tell you.
5. **Simple metrics, complex analysis.** Keep metrics understandable. Let analysis go deep.
6. **Instrument before you need it.** Retroactive analytics is painful. Plan ahead.
7. **Confidence levels matter.** State statistical significance and sample sizes.

## Workflow

### 1. Clarify Before Starting
- What question are we trying to answer?
- What decision will this analysis inform?
- What data is available?
- What's the timeline?
- Who is the audience for the findings?

### 2. Choose the Right Approach

| Need | Approach |
|------|----------|
| Define what to measure | Metrics framework design |
| Understand user behavior | Funnel analysis, cohort analysis |
| Test a hypothesis | A/B test design and analysis |
| Monitor health | Dashboard design |
| Communicate findings | Data storytelling |

### 3. Analytics Process

**Define:** What question? What metric? What's the hypothesis?

**Collect:** What data exists? What needs instrumenting? What's the sample?

**Analyze:** Run the analysis. Check for patterns. Test significance.

**Communicate:** Tell the story. Lead with the insight. Make it actionable.

## Quality Checks

- [ ] Metric clearly defined?
- [ ] Data source reliable?
- [ ] Sample size sufficient?
- [ ] Statistical significance achieved (for experiments)?
- [ ] Alternative explanations considered?
- [ ] Insight is actionable?
- [ ] Findings presented clearly?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Vanity metrics | Measure what drives decisions |
| Data without context | Always provide comparison/baseline |
| P-hacking | Define hypothesis before analysis |
| Dashboard overload | Focus on decisions, not charts |
| Ignoring qualitative data | Combine quant with qual |
