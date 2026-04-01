---
description: "Customer Success — Onboarding plans, retention strategies, churn analysis, customer health scoring, renewal playbooks, expansion strategies, NPS programs, and customer communication. Triggers: onboarding plan, retention, churn, customer health, renewal, expansion, upsell, NPS, customer satisfaction, customer journey, time to value, customer lifecycle, win-back, QBR, quarterly business review, customer communication, success plan"
---

# Customer Success

Customer success is the discipline of ensuring customers achieve their desired outcomes using your product — and that your business grows as a result. It bridges the gap between closing a deal and building a lasting customer relationship. The goal is mutual: the customer gets value, you get retention, expansion, and advocacy.

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern
- `${CLAUDE_PLUGIN_ROOT}/frameworks/customer-lifecycle.md` — Lifecycle stages, health scoring, intervention patterns
- `${CLAUDE_PLUGIN_ROOT}/frameworks/stakeholder-communication.md` — Audience-aware communication
- `${CLAUDE_PLUGIN_ROOT}/frameworks/change-management.md` — Adoption curves, resistance patterns

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — Product, positioning, offerings
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, language rules

**Context (load when relevant):**
- `${CLAUDE_PLUGIN_ROOT}/context/extended/product.md` — Product features, workflows, how it works
- `${CLAUDE_PLUGIN_ROOT}/context/extended/users.md` — User personas, goals, pain points
- `${CLAUDE_PLUGIN_ROOT}/context/extended/audience.md` — Buyer personas, segments, decision process
- `${CLAUDE_PLUGIN_ROOT}/context/extended/pricing.md` — Pricing model, tiers, expansion paths
- `${CLAUDE_PLUGIN_ROOT}/context/extended/proof-points.md` — Case studies, metrics, success stories

**References (load when needed):**
- `${CLAUDE_PLUGIN_ROOT}/skills/customer-success/references/onboarding-playbooks.md` — Onboarding structures, time-to-value optimization, welcome sequences
- `${CLAUDE_PLUGIN_ROOT}/skills/customer-success/references/retention-frameworks.md` — Health scoring, churn analysis, intervention strategies, renewal and expansion playbooks

## Core Principles

1. **Time to value is everything.** The faster a customer experiences the core benefit of your product, the more likely they are to stay. Every onboarding decision should optimize for this.
2. **Measure health, not happiness.** A customer who says they're happy but isn't using the product will churn. A customer who submits support tickets but uses the product daily won't. Track behavior, not sentiment alone.
3. **Proactive beats reactive.** Don't wait for a customer to complain or cancel. Monitor health signals and intervene before problems become crises. The best save is the one you never had to make.
4. **Expansion is earned, not sold.** Upsell and cross-sell work when the customer has already experienced value. Pushing expansion before the customer is successful damages trust and accelerates churn.
5. **Segment your effort.** Not every customer needs the same level of touch. High-value accounts get white-glove treatment. Self-serve customers get great documentation and automated nudges. Match your investment to the opportunity.
6. **Listen to churn.** Every customer who leaves is telling you something. Analyze churn patterns systematically — they reveal product gaps, onboarding failures, and market misalignment faster than any survey.
7. **Success is a team sport.** Customer success doesn't own the customer alone. It connects product (feedback loops), sales (handoff and expansion), marketing (advocacy), and support (escalation). Build those bridges.

## Workflow

### 1. Clarify Before Starting
- What type of customer success work? (onboarding, health assessment, churn analysis, renewal strategy, expansion plan, QBR, win-back)
- Which customer segment or specific account?
- What stage of the lifecycle are they in? (load customer-lifecycle.md)
- What data or signals do we have about their current health?
- What does success look like for this customer? For us?

### 2. Choose the Right Format

| Situation | Format | Objective |
|-----------|--------|-----------|
| New customer signed | Onboarding plan | Get to first value milestone fast |
| Customer at risk | Health assessment + intervention plan | Identify issues, stabilize the account |
| Approaching renewal | Renewal strategy | Demonstrate value, secure commitment |
| Healthy customer, growth opportunity | Expansion plan | Grow the account based on proven value |
| Customer churned | Churn analysis | Understand why, extract lessons, attempt win-back |
| Quarterly check-in | QBR document | Review progress, align on next quarter |
| Feedback program | NPS/CSAT program design | Systematize customer feedback collection |
| Scaling CS operations | Playbook / process design | Standardize for consistency across the team |

### 3. Creation Process

**Understand the customer:**
- Where are they in the lifecycle? (reference customer-lifecycle.md)
- What did they buy and why? (reference pricing.md for their tier/plan)
- What outcomes are they trying to achieve? (reference users.md for persona goals)
- What does their usage look like? What signals do we have?
- Who are the key stakeholders? (champion, decision-maker, end users)

**Build the artifact:**
- Start with the customer's desired outcome, not your product features
- Follow voice.md — customer-facing materials should sound like your brand
- Use specific metrics and timelines, not vague promises
- Reference proof-points.md for relevant success stories from similar customers
- Include clear ownership — who does what, by when
- Define what "done" or "successful" looks like in measurable terms

**Review and personalize:**
- Is this specific to this customer's situation, or could it be for anyone?
- Does it acknowledge their actual challenges, not hypothetical ones?
- Are the timelines realistic given what we know about their team and resources?
- Would you feel confident presenting this to the customer?

## Quality Checks

- [ ] Starts with the customer's desired outcome, not your product?
- [ ] Includes specific, measurable success criteria?
- [ ] Timelines are realistic and account for the customer's capacity?
- [ ] Health signals are behavioral (usage, adoption), not just sentiment?
- [ ] Personalized to the specific customer or segment, not generic?
- [ ] Clear ownership for every action item?
- [ ] Matches voice.md for any customer-facing materials?
- [ ] Uses correct terminology from identity.md?
- [ ] Proof points and success stories are relevant to this customer's situation?
- [ ] Expansion recommendations are earned (customer is already successful)?
- [ ] Churn analysis identifies root causes, not just symptoms?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Treating onboarding as a product tour | Onboarding is about reaching the customer's first value milestone |
| Measuring success by NPS alone | Combine sentiment with behavioral signals (usage, adoption, support volume) |
| Same playbook for every customer | Segment by value, complexity, and lifecycle stage |
| Pushing expansion before value is proven | Earn the right to expand by delivering on the initial promise first |
| Waiting for churn signals to act | Monitor health proactively and intervene at the first sign of decline |
| Blaming the customer for churn | Every churn is a learning opportunity — what did we miss? |
| Generic QBRs that recite metrics | QBRs should connect product usage to business outcomes the customer cares about |
| Hoarding customer insights | Feed learnings back to product, sales, and marketing — success is a team sport |
