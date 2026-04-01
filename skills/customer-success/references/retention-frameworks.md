# Retention Frameworks

Health scoring, churn analysis, intervention strategies, renewal and expansion playbooks. Load this when working on retention, renewals, expansion, or churn prevention.

---

## Customer Health Score — Implementation Guide

The customer-lifecycle.md framework defines the health scoring concept. This reference provides the implementation details.

### Step 1: Choose Your Signals

Pick 5-8 signals that you can actually measure. Don't design the perfect health score — design one you can start using this week.

**Usage signals (strongest predictors):**
- Login frequency (daily/weekly/monthly active users)
- Core feature usage (are they using the thing they bought it for?)
- Breadth of usage (how many features in use?)
- Depth of usage (how intensively?)
- User adoption ratio (active users / total licensed users)

**Engagement signals:**
- Response time to CS outreach
- Meeting attendance rate
- QBR participation
- Feature request submissions (engagement signal, not complaint)
- Community participation

**Support signals:**
- Ticket volume trend (increasing = concerning, but filing tickets = engaged)
- Ticket severity distribution
- Resolution satisfaction
- Time since last support interaction (too long can mean disengagement)

**Relationship signals:**
- Executive sponsor still in role?
- Champion still engaged?
- Multiple contacts or single-threaded?
- Willingness to take reference calls or provide testimonials

**Outcome signals:**
- Are they achieving the goals they stated during onboarding?
- Are they hitting usage milestones on the expected timeline?
- Have they reported ROI or business impact?

### Step 2: Weight and Score

Assign weights based on what actually correlates with retention and churn in your business. Start with intuition, refine with data.

**Example scoring model:**

| Signal | Weight | Scoring |
|--------|--------|---------|
| Core feature usage | 25% | Daily=100, Weekly=70, Monthly=40, Rare=10 |
| User adoption ratio | 20% | >80%=100, 50-80%=70, 20-50%=40, <20%=10 |
| Engagement responsiveness | 15% | High=100, Medium=60, Low=20 |
| Support health | 15% | Positive trend=100, Stable=70, Negative trend=30 |
| Relationship depth | 15% | Multi-threaded=100, 2-3 contacts=60, Single-threaded=20 |
| Outcome achievement | 10% | On track=100, Behind=50, Not measured=40 |

### Step 3: Set Thresholds and Actions

| Score | Status | Cadence | Action |
|-------|--------|---------|--------|
| 80-100 | Healthy | Quarterly QBR | Explore expansion, request referrals |
| 60-79 | Neutral | Monthly check-in | Identify blockers, drive deeper adoption |
| 40-59 | At Risk | Biweekly outreach | Escalate internally, create recovery plan |
| 0-39 | Critical | Weekly or more | Executive escalation, save plan, honest conversation |

### Step 4: Review and Calibrate

- Review health scores monthly as a team
- Compare scores against actual churn — are the scores predictive?
- Adjust weights quarterly based on what you learn
- Don't over-automate — human judgment catches what algorithms miss

---

## Intervention Playbooks

### At-Risk Account Recovery

**When to use:** Health score drops to At Risk (40-59) or shows a sustained declining trend.

**Step 1: Diagnose** (before reaching out)
- What changed? Check usage data, support tickets, stakeholder changes.
- Is this a product issue, a people issue, or a priority issue?
- How long has the decline been happening?

**Step 2: Outreach** (direct, honest, specific)
- Contact the champion first: "I've noticed [specific observation]. I want to make sure we're delivering value. Can we talk?"
- Don't be vague. Reference specific data: "Your team's usage dropped 40% last month" not "I wanted to check in."
- Listen more than talk. The goal is diagnosis, not a pitch.

**Step 3: Recovery plan**
- Co-create with the customer — don't hand them a plan
- 2-3 specific actions with owners and dates
- Short timeline (2-4 weeks) with a check-in halfway through
- Escalate to executive sponsor if champion alone can't fix it

**Step 4: Monitor**
- Increase check-in frequency during recovery
- Track the specific metrics that triggered the alert
- If recovery plan doesn't show results in 4 weeks, escalate further

### Critical Account Save

**When to use:** Health score drops to Critical (0-39) or customer explicitly signals intent to leave.

**Step 1: Executive alignment** (internal)
- Brief your leadership on the situation
- Decide what you're willing to offer (discounts, contract flexibility, custom support)
- Agree on the "walk-away" point — what's not worth saving?

**Step 2: Honest conversation**
- Request a call with the customer's decision-maker, not just the champion
- Lead with honesty: "I know things haven't gone the way either of us expected. I want to understand what happened and whether there's a path forward."
- Listen to their full perspective before proposing solutions

**Step 3: Save offer** (if appropriate)
- Address their specific concerns with specific solutions
- Don't over-promise. Under-promise and over-deliver.
- Include a success plan with clear milestones and a review date
- Make it easy to say yes (reduce friction, offer concessions if warranted)

**Step 4: Win or learn**
- If saved: treat this as a new onboarding. Rebuild from scratch.
- If lost: conduct a thorough churn analysis. Feed learnings back to the team.

---

## Renewal Playbook

Renewals should be a non-event if CS is done right. If renewal is stressful, something upstream is broken.

### 90-60-30 Renewal Framework

**90 days before renewal:**
- Review health score and usage trends
- Identify any unresolved issues or open support tickets
- Prepare a value summary: what they achieved, in their terms
- Internal alignment: any pricing changes, new features, or contract adjustments to propose?

**60 days before renewal:**
- QBR or check-in with the customer
- Present the value summary: "Here's what you've accomplished this year"
- Discuss their goals for the next period
- If expansion is appropriate, introduce it here (new features, additional seats, higher tier)
- Surface any concerns early — don't wait for the renewal conversation

**30 days before renewal:**
- Formal renewal conversation
- Present the renewal terms (ideally, this is straightforward if 90 and 60 went well)
- Address any remaining concerns
- Get commitment and process the renewal

### Renewal Value Summary

A one-page document that makes the renewal decision easy. Structure:

**1. What you set out to achieve** (their original goals)
**2. What we accomplished** (specific outcomes, metrics, milestones)
**3. What's next** (their goals for the next period and how you'll support them)
**4. Renewal terms** (what they're renewing, any changes, investment)

Use real numbers. "Your team saved 12 hours per week on reporting" beats "We helped improve efficiency."

---

## Expansion Playbook

### When to Expand

Expansion is appropriate when ALL of these are true:
- Customer health score is 70+ (Healthy or strong Neutral)
- They've achieved their primary success criteria
- The expansion aligns with a need they've expressed or demonstrated
- The timing is right (not mid-crisis, not right before renewal negotiation)

### Expansion Types

| Type | What It Is | Signal |
|------|-----------|--------|
| **Upsell** | Move to a higher tier or plan | Hitting plan limits, asking about premium features |
| **Cross-sell** | Add a complementary product or module | New use case emerging, adjacent team interested |
| **Seat expansion** | Add more users | New teams onboarding, user requests from non-licensed staff |
| **Usage expansion** | Increase volume or capacity | Approaching limits, growing usage patterns |

### How to Position Expansion

- **Lead with their success:** "You've been getting great results with X. Based on your usage patterns, Y could help you [specific outcome]."
- **Connect to their goals:** "You mentioned wanting to [goal]. [Expansion] is how other customers like you have gotten there."
- **Show the math:** "You're currently at 90% of your plan limit. Moving up gives you [specific benefits] for [specific investment]."
- **Don't pressure:** If they're not ready, respect it. A customer who expands when ready stays longer than one who was pushed.

---

## Win-Back Playbook

### When to Attempt Win-Back

Worth attempting when:
- The customer churned for fixable reasons (product gap now filled, support issue now resolved, pricing now flexible)
- The customer left on good terms (not hostile)
- At least 3-6 months have passed (give them space)
- You have something genuinely new to offer

Not worth attempting when:
- They were never a good fit
- They left due to trust violations
- The core issue that caused churn hasn't been addressed

### Win-Back Approach

**Step 1: Acknowledge**
- "I know [product] didn't work out for you last time. I respect that decision."

**Step 2: What's changed**
- Be specific: "Since you left, we've [built X, fixed Y, changed Z]"
- Only mention changes relevant to why they left

**Step 3: Low-commitment offer**
- Don't ask them to re-commit immediately
- Offer a trial, a demo of what's new, or a conversation
- "Would it be worth 15 minutes to see if [specific change] addresses what was missing?"

**Step 4: If they return**
- Treat them as a new customer for onboarding purposes
- Assign a senior CS person — they need to trust you again
- Over-communicate during the first 90 days
- Monitor health signals closely

---

## QBR (Quarterly Business Review) Structure

### For High-Touch Accounts

**1. Review period summary** (5 min)
- Key metrics and trends from the past quarter
- Presented in their business terms, not your product terms

**2. Outcomes achieved** (10 min)
- What they set out to accomplish vs. what happened
- Celebrate wins specifically: "Your team reduced [X] by [Y]%"
- Acknowledge gaps honestly

**3. Usage insights** (5 min)
- Adoption trends, feature usage, areas of opportunity
- "Your team is getting strong value from X. There's an opportunity with Y that similar companies use to [outcome]."

**4. Their priorities for next quarter** (10 min)
- What are their goals? What's changing in their business?
- This is the most important section — listen more than present

**5. Our plan to support those priorities** (10 min)
- Specific actions, timelines, and owners
- Include relevant product roadmap items (only what's committed, not aspirational)
- Expansion conversation if appropriate

**6. Open discussion** (10 min)
- Feedback, concerns, questions
- End with agreed next steps

### QBR Anti-Patterns
- Reading a slide deck at them for 45 minutes
- Focusing on your product metrics instead of their business outcomes
- Skipping the "what are your priorities" conversation
- Using the QBR as a surprise expansion pitch
- Not sending a summary with action items after
