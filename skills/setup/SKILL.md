---
description: "Setup — Configure Baseline Core with your business context. Interviews you about your company and generates the context files that make every skill work for your specific business. Triggers: setup, configure, onboard, get started, set up context, customize plugin, initialize"
---

# Setup

This skill walks you through setting up the business context that powers every other skill in Baseline Core. It interviews you about your company, then generates context files tailored to your answers.

**Without context files, skills produce generic output. With them, every skill works specifically for your business.**

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern

No other context files are needed — this skill creates them.

## Core Principles

1. **Conversational, not form-filling.** Ask natural questions, not "Please provide your company name." Have a conversation. Extract what you need from how they talk about their business.
2. **Start with the required files.** Identity and voice are required. Everything else is recommended but optional. Get the essentials first, then offer to go deeper.
3. **Use their words.** When generating context files, use the language and phrasing the user actually used. Don't corporate-ify their answers. If they said "we help small teams ship faster," don't turn that into "we empower organizations to accelerate delivery."
4. **Generate, then refine.** Write the context file, show it to the user, and ask if it sounds like them. Iterate until it does. The voice file especially needs to feel right.
5. **One file at a time.** Don't try to gather all information upfront. Complete each context file before moving to the next. This keeps the conversation focused and gives the user a sense of progress.
6. **Detect existing context.** Before starting, check if any context files are already populated. If they are, offer to update them rather than starting from scratch.

## Workflow

### Phase 1: Check Current State

**Purpose:** Understand what's already set up.

**What to do:**
1. Read all 11 context files:
   - `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md`
   - `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md`
   - `${CLAUDE_PLUGIN_ROOT}/context/extended/product.md`
   - `${CLAUDE_PLUGIN_ROOT}/context/extended/users.md`
   - `${CLAUDE_PLUGIN_ROOT}/context/extended/audience.md`
   - `${CLAUDE_PLUGIN_ROOT}/context/extended/competitive.md`
   - `${CLAUDE_PLUGIN_ROOT}/context/extended/design.md`
   - `${CLAUDE_PLUGIN_ROOT}/context/extended/formatting.md`
   - `${CLAUDE_PLUGIN_ROOT}/context/extended/proof-points.md`
   - `${CLAUDE_PLUGIN_ROOT}/context/extended/pricing.md`
   - `${CLAUDE_PLUGIN_ROOT}/context/extended/technical.md`
2. Check which files have real content vs. template placeholders (HTML comments with instructions)
3. Report what's set up and what isn't

**Done when:** You've told the user which files are populated and which need setup.

---

### Phase 2: Identity (Required)

**Purpose:** Establish who the user is and what they do.

**What to do:**
1. Ask the user to tell you about their company or practice. Keep it conversational:
   - "Tell me about your company — what do you do and who do you do it for?"
   - "How do you describe what makes you different from alternatives?"
   - "What do you offer? Walk me through your products or services."
   - "Are there specific terms or words that matter to your brand?"
2. Listen for: company name, what they do, positioning, offerings, differentiators, values, terminology
3. Ask follow-up questions for anything that's vague or missing
4. Generate `identity.md` with their answers, organized into the file's sections
5. Show them the generated file and ask: "Does this capture it? Anything to add or change?"
6. Iterate until they approve
7. Write the final version to `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md`

**Done when:** The user has approved the identity file.

---

### Phase 3: Voice (Required)

**Purpose:** Define how the user sounds.

**What to do:**
1. Ask about their communication style:
   - "How would you describe the way you communicate? If you were writing an email to a customer, what would it sound like?"
   - "Are there words or phrases you never want to use?"
   - "Do you write as 'I' or 'we'?"
   - "Is your tone different when you're writing strategy vs. marketing vs. documentation?"
2. If the user has existing content (website, emails, docs), offer to look at it to extract voice patterns
3. Generate `voice.md` with their answers
4. Show them the file and ask: "Does this sound like you?"
5. Iterate until it feels right — voice is the most subjective file, so expect a round or two of revision
6. Write the final version to `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md`

**Done when:** The user has approved the voice file.

---

### Phase 4: Offer Extended Context

**Purpose:** Set up the recommended files that deepen skill performance.

**What to do:**
1. Tell the user: "The essentials are done — every skill will now work for your business. There are 9 more context files that make specific skills even better. Want to set any of these up now?"
2. Present the options with what they unlock:
   - **Product** — What your product does, features, how it works. Makes UX Design, Prototyping, Product Communications, and Technical Documentation grounded in your real product.
   - **Users** — User personas, goals, pain points, friction. Makes UX Design, Research, and Product Analytics work from real user needs.
   - **Audience** — Who you market and sell to, buyer personas. Makes Product Marketing, Go-to-Market, and Research target the right people. (Different from Users — audience is who you sell to, users is who interacts with the product.)
   - **Competitive** — Competitors, market positioning, alternatives. Makes Product Marketing, GTM, Research, and Strategic Advisory factor in real competition.
   - **Design** — Colors, typography, design system. Makes Prototyping, UX Design, and Visual Communication produce on-brand output.
   - **Formatting** — Document structure conventions. Makes Product Communications, Technical Documentation, and quality reviews follow your standards.
   - **Proof Points** — Case studies, metrics, testimonials. Makes marketing and sales skills back up claims with real evidence.
   - **Pricing** — Pricing model, tiers, objections. Makes Go-to-Market Planning, Product Marketing, and proposals reference real pricing.
   - **Technical** — Tech stack, architecture, integrations. Makes Prototyping and Technical Documentation compatible with your actual technology.
3. For each file the user wants to set up, follow the same pattern: conversational interview → generate file → show for approval → write final version
4. For files they skip, leave the templates in place — skills degrade gracefully without them

**Interview guides for each extended file:**

**Product:**
- "Tell me about your product — what does it do and what form does it take?"
- "What are the main features or capabilities?"
- "Walk me through what a user does from start to finish."
- "What makes your product different from alternatives, as a product?"
- "Where is it right now — live, beta, pre-launch? What are you building next?"

**Users:**
- "Who actually uses your product day-to-day? Describe them."
- "What are they trying to accomplish?"
- "What frustrates them about their current situation?"
- "Do you have different types of users who use it differently?"
- "How do your users talk about their work? What words do they use?"

**Audience:**
- "Who do you market and sell to? Is that the same person as the user?"
- "What problems do they have that lead them to you?"
- "What have they tried before finding you?"
- "How do they talk about their problems? What words do they use?"
- "Are there signals that someone is NOT a good fit?"

**Competitive:**
- "Who are your main competitors? What do they do well?"
- "Where do competitors fall short — and where do you win?"
- "What are the indirect alternatives? Spreadsheets, hiring someone, doing nothing?"
- "How do you position yourself relative to the market?"

**Design:**
- "What are your brand colors? Do you have hex values?"
- "What fonts do you use?"
- "Do you have a design system or component library? What are the key patterns?"
- "Any design principles that guide your visual decisions?"

**Formatting:**
- "Do you have conventions for how documents are structured?"
- "What does a typical report or PRD look like for you?"
- "Any specific formatting rules your team follows?"

**Proof Points:**
- "Do you have case studies or customer success stories?"
- "What measurable outcomes have you delivered?"
- "Do you have testimonials you can share?"
- "What's your background or credibility in this space?"

**Pricing:**
- "What's your pricing model? Free, freemium, paid tiers, custom?"
- "Walk me through the tiers and what each includes."
- "What's your pricing philosophy — what principles guide your pricing?"
- "What objections do you hear about pricing, and how do you handle them?"

**Technical:**
- "What's your tech stack? Frontend, backend, infrastructure."
- "How is your system architected at a high level?"
- "What external services or APIs do you integrate with?"
- "Are there technical constraints that affect product decisions?"

**Done when:** The user has set up or skipped each extended file.

---

### Phase 5: Summary

**Purpose:** Confirm what's set up and what's available.

**What to do:**
1. List all context files and their status (populated / template)
2. Remind the user they can run /setup again anytime to update or add files
3. Suggest trying a skill to see the context in action: "Try running one of the skills now — like /product-marketing or /strategic-advisory — and you'll see it working with your business context."

**Done when:** The user knows what's set up and how to use it.

## Quality Checks

- [ ] Identity file contains: company name, what they do, positioning, at least one offering, at least one differentiator
- [ ] Voice file contains: tone description, person (I/we/they), at least 3 language rules, at least 3 words to avoid
- [ ] Generated files use the user's own language, not corporate filler
- [ ] User explicitly approved each file before it was written
- [ ] Template placeholders (HTML comments) are removed from populated files
- [ ] Extended files were offered but not forced

## Anti-Patterns

- **Don't interrogate.** This should feel like a conversation, not a form. If the user gives a long answer that covers multiple sections, extract what you need — don't re-ask for each section individually.
- **Don't over-polish.** If the user says "we help startups not screw up their product launches," don't rewrite it as "we assist emerging organizations in optimizing their go-to-market execution." Keep their voice.
- **Don't skip showing the output.** Always show the generated file and get explicit approval before writing. The user needs to see it and feel like it represents them.
- **Don't require everything.** Identity and voice are required. Everything else is optional. If the user wants to stop after two files, that's fine.
- **Don't generate placeholder content.** If the user doesn't have case studies yet, don't make up placeholder ones. Leave the proof-points file as a template and tell them they can fill it in later.
