---
description: "Sales Enablement — Proposals, pitch decks, outreach emails, demo scripts, objection handling, follow-up sequences, and sales collateral. Triggers: write a proposal, pitch deck, sales deck, outreach email, cold email, demo script, objection handling, follow-up, sales collateral, prospect email, close the deal, sales sequence, proposal template"
---

# Sales Enablement

Sales enablement is the discipline of creating materials and strategies that help close deals. It bridges the gap between marketing positioning and actual sales conversations — turning your messaging and proof points into tools that help you (or your team) sell effectively.

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern
- `${CLAUDE_PLUGIN_ROOT}/frameworks/messaging.md` — Messaging hierarchy, value propositions
- `${CLAUDE_PLUGIN_ROOT}/frameworks/stakeholder-communication.md` — Audience-aware communication

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — Product, positioning, offerings
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, language rules

**Context (load when relevant):**
- `${CLAUDE_PLUGIN_ROOT}/context/extended/audience.md` — Target audience, buyer personas, decision process
- `${CLAUDE_PLUGIN_ROOT}/context/extended/competitive.md` — Competitors, how you win
- `${CLAUDE_PLUGIN_ROOT}/context/extended/pricing.md` — Pricing model, objection handling
- `${CLAUDE_PLUGIN_ROOT}/context/extended/proof-points.md` — Case studies, metrics, testimonials
- `${CLAUDE_PLUGIN_ROOT}/context/extended/product.md` — Product features, workflows

**References (load when needed):**
- `${CLAUDE_PLUGIN_ROOT}/skills/sales-enablement/references/proposal-templates.md` — Proposal structures, SOW formats, pricing presentation
- `${CLAUDE_PLUGIN_ROOT}/skills/sales-enablement/references/outreach-playbooks.md` — Cold outreach, follow-ups, sequences, demo scripts

## Core Principles

1. **Solve their problem, don't sell your product.** Every piece of sales collateral should start with the prospect's pain, not your features. Load audience.md to understand their world.
2. **Proof over promises.** Prospects trust evidence — case studies, metrics, testimonials. Load proof-points.md and use real numbers. "We helped Company X reduce onboarding time by 60%" beats "We improve efficiency."
3. **Know the competition.** Load competitive.md so you can position against alternatives without trashing them. Acknowledge what competitors do well, then explain why you're better for this specific situation.
4. **Match the stage.** A cold outreach email is different from a proposal after a demo. Know where the prospect is in the decision process (audience.md) and match your tone and content.
5. **Personalize, don't template.** Use templates as starting points, then customize for the specific prospect. Generic outreach gets ignored.
6. **Price with confidence.** Load pricing.md and present pricing as an investment, not a cost. Address objections proactively.
7. **Follow up without being annoying.** Persistence works. Being pushy doesn't. Add value with every touch.

## Workflow

### 1. Clarify Before Starting
- What type of sales material? (proposal, outreach, deck, script, follow-up)
- Who is the prospect? (role, company, stage in decision process)
- What do we know about their specific situation?
- What's the objective? (book a meeting, close a deal, handle an objection)
- What proof points are most relevant to this prospect?

### 2. Choose the Right Format

| Stage | Format | Objective |
|-------|--------|-----------|
| Cold outreach | Email / LinkedIn message | Book a meeting |
| Warm introduction | Intro email / brief | Establish relevance |
| Discovery | Question guide / agenda | Understand their needs |
| Demo | Demo script / talking points | Show relevant value |
| Proposal | Proposal document / SOW | Formalize the offering |
| Objection | Response framework | Address concerns |
| Follow-up | Email sequence | Maintain momentum |
| Close | Summary + next steps | Get to yes |
| Post-sale | Onboarding plan / handoff | Deliver on promises |

### 3. Creation Process

**Research the prospect:**
- Who are they? What does their company do?
- What problem are they likely facing? (reference audience.md buying triggers)
- Have they tried alternatives? (reference competitive.md)
- What proof points are most relevant to their situation?

**Draft the material:**
- Start with their problem, not your product
- Follow voice.md for tone — sales materials still sound like you
- Use messaging.md for value prop hierarchy
- Include specific evidence from proof-points.md
- Present pricing from pricing.md with context and confidence
- End with a clear, specific next step

**Review and personalize:**
- Does this feel generic or specific to the prospect?
- Would you respond to this if you received it?
- Is the ask clear and reasonable for this stage?
- Check against identity.md for correct terminology

## Quality Checks

- [ ] Starts with the prospect's problem, not your product?
- [ ] Includes specific evidence (case studies, metrics)?
- [ ] Matches voice.md — doesn't switch to "sales mode"?
- [ ] Uses correct terminology from identity.md?
- [ ] Pricing presented with confidence and context?
- [ ] Personalized to the specific prospect, not generic?
- [ ] Clear call to action appropriate for the sales stage?
- [ ] Competitive positioning is honest and specific?
- [ ] Would you respond to this if you received it?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Leading with features | Lead with the prospect's problem |
| Generic "Dear Sir/Madam" | Personalize with specific research |
| Trashing competitors | Acknowledge their strengths, differentiate honestly |
| Hiding the price | Present pricing with confidence and context |
| Long-winded proposals | Be concise — respect their time |
| Following up with "just checking in" | Add value with every touchpoint |
| Using a different voice for sales | Follow voice.md — consistency builds trust |
| Making promises you can't keep | Underpromise, overdeliver — use real proof points |
