# Onboarding Playbooks

Structures for customer onboarding, time-to-value optimization, and welcome sequences. Load this when creating onboarding plans or improving the onboarding experience.

---

## Onboarding Plan Structure

An onboarding plan is a shared document between you and the customer. It sets expectations, assigns ownership, and defines what "done" looks like.

### Standard Onboarding Plan

**1. Welcome & Expectations** (shared in first interaction)
- What the customer bought and why (restate their goals from the sales process)
- What onboarding looks like: timeline, milestones, who's involved
- What you need from them (access, data, stakeholder time)
- What "successful onboarding" means in specific terms

**2. Success Criteria**
- Define 1-3 measurable outcomes that mark a successful onboarding
- These should be the customer's goals, not your product metrics
- Example: "Your team can independently create and publish a campaign without support assistance" not "User has logged in 5 times"

**3. Milestone Map**

| Milestone | What Happens | Owner | Target Date | Definition of Done |
|-----------|-------------|-------|-------------|-------------------|
| Kickoff | Intro call, align on goals, assign stakeholders | CS + Customer | Day 1 | Goals documented, stakeholders identified |
| Setup | Account configured, integrations connected | CS + Technical | Week 1 | Core setup complete, data flowing |
| First Value | Customer completes core workflow end-to-end | Customer + CS | Week 2-3 | Customer achieves primary use case independently |
| Adoption | Team trained, usage expanding | Customer | Week 4-6 | Multiple users active, self-sufficient |
| Handoff | Onboarding complete, transition to ongoing CS | CS | Week 6-8 | Success criteria met, cadence established |

**4. Stakeholder Map**

| Role | Name | Responsibility | Engagement Level |
|------|------|---------------|-----------------|
| Executive Sponsor | [Name] | Approves resources, removes blockers | Monthly check-in |
| Champion | [Name] | Day-to-day driver, internal advocate | Weekly |
| End Users | [Names/Teams] | Product users | Training sessions |
| Technical Contact | [Name] | Integrations, data, access | As needed |

**5. Risk Register**
- What could delay onboarding? (common: stakeholder availability, data readiness, competing priorities)
- Mitigation plan for each risk
- Escalation path if risks materialize

---

## Onboarding by Segment

Not every customer needs the same onboarding. Match the investment to the opportunity.

### High-Touch (Enterprise / High-Value)

**Characteristics:** Large contract, complex implementation, multiple stakeholders, long sales cycle

**Onboarding approach:**
- Dedicated CS manager assigned before contract closes
- Sales-to-CS handoff meeting with full context transfer
- Custom onboarding plan co-created with the customer
- Weekly check-in calls during onboarding
- Executive sponsor engagement at kickoff and first milestone
- On-site or virtual training sessions for end users
- Formal onboarding review at completion

**Timeline:** 4-12 weeks depending on complexity

### Mid-Touch (Growth / Mid-Market)

**Characteristics:** Medium contract, standard implementation, 1-2 key stakeholders

**Onboarding approach:**
- Shared CS manager (1:many)
- Templated onboarding plan, personalized for their goals
- Kickoff call + 2-3 scheduled check-ins
- Self-serve training with CS available for questions
- Automated email sequence supplements human touchpoints

**Timeline:** 2-4 weeks

### Low-Touch / Self-Serve (SMB / Free-to-Paid)

**Characteristics:** Small contract or free tier, simple setup, individual user or small team

**Onboarding approach:**
- Automated welcome sequence (email or in-app)
- Product tours and tooltips for first-time setup
- Help center and video walkthroughs
- Triggered outreach if user stalls (no login after 3 days, setup incomplete after 7)
- Community or office hours for questions
- Human intervention only if health signals indicate risk

**Timeline:** 1-2 weeks (mostly self-driven)

---

## Welcome Sequences

### Email Welcome Sequence (Self-Serve / Low-Touch)

**Email 1 — Welcome (Immediately after signup)**
- Welcome them by name
- Restate the core value: "You signed up to [achieve X]. Here's how to get there."
- One clear CTA: the single most important first step
- Don't overwhelm — no feature lists, no 10-step guides

**Email 2 — First Value (Day 2-3)**
- Guide them to the first "aha moment"
- Show the shortest path to experiencing the core benefit
- Include a specific example or walkthrough
- CTA: complete the core workflow

**Email 3 — Tips & Depth (Day 5-7)**
- Share one power-user tip relevant to their use case
- Link to a success story from a similar customer
- CTA: try the next feature or invite a teammate

**Email 4 — Check-In (Day 10-14)**
- "How's it going?" — genuinely ask
- Provide help resources for common sticking points
- If they haven't reached first value, offer direct help
- CTA: reply to this email or book a call

**Email 5 — Social Proof (Day 21)**
- Share a relevant case study or testimonial
- Reinforce the value they should be experiencing by now
- If they're active: invite to community, ask for feedback
- If they're inactive: last gentle nudge before reducing cadence

### Rules for Welcome Sequences
- Each email should have exactly one CTA
- Space them out — daily emails feel like spam
- Personalize based on their plan, role, or use case when possible
- Track opens and clicks to identify at-risk users early
- Stop the sequence if they've already achieved the milestone (don't send "complete setup" if they already did)

---

## Time to First Value (TTFV)

### What It Is
The elapsed time between when a customer signs up (or signs a contract) and when they first experience the core benefit of your product. This is the single most important onboarding metric.

### How to Measure It
1. Define what "first value" means for your product. Be specific.
   - Not: "User logged in"
   - Better: "User completed their first [core action] and saw [result]"
2. Measure the median time from signup/contract to that event
3. Segment by customer type — enterprise TTFV will be longer than self-serve

### How to Reduce It
- **Remove setup friction:** Every step between signup and value is a potential drop-off point. Cut ruthlessly.
- **Front-load the win:** Get them to the "aha" moment before asking them to configure, customize, or optimize.
- **Use templates and defaults:** Don't make them start from scratch. Pre-populate with sensible defaults or templates.
- **Guided first experience:** Walk them through the core workflow the first time. Product tours, setup wizards, or a human guide.
- **Defer non-essential setup:** Integrations, team invites, advanced configuration — these can wait. First value can't.

### TTFV Benchmarks (General)
- Self-serve SaaS: minutes to hours (target: under 1 hour)
- SMB with setup: 1-7 days
- Mid-market: 1-3 weeks
- Enterprise: 4-8 weeks

If your TTFV is significantly longer than these benchmarks for your segment, onboarding is likely your biggest retention lever.

---

## Sales-to-CS Handoff

The handoff between sales and customer success is where context dies if you're not intentional about it.

### What CS Needs from Sales

| Information | Why It Matters |
|------------|---------------|
| Why they bought (specific pain, not "liked the product") | Defines what "success" means for this customer |
| Who was involved in the decision | Identifies stakeholders and champions |
| What they were promised (explicitly and implicitly) | Sets the bar for delivery |
| What competitors they evaluated | Reveals what they're comparing you to |
| Timeline or urgency drivers | Shapes onboarding pace |
| Red flags or concerns raised during sales | Forewarns CS about potential friction |
| Technical environment or constraints | Informs implementation approach |

### Handoff Process
1. Sales completes handoff document before or at contract signature
2. CS reviews and prepares questions
3. Internal handoff meeting: Sales, CS, and (if relevant) technical implementation
4. Joint introduction: Sales introduces CS to the customer, reinforcing continuity
5. CS takes over with full context — the customer should never have to repeat themselves

### Anti-Pattern: The Cold Handoff
"Here's your CSM, good luck!" — the customer feels abandoned by the person they trusted (sales) and dumped on a stranger (CS). Always make the introduction warm, explain what happens next, and have CS demonstrate that they already know the customer's situation.
