---
description: "Content Writing — Blog posts, newsletters, social media, LinkedIn posts, email campaigns, case studies, and thought leadership. Triggers: write a blog post, newsletter, social media post, LinkedIn post, email campaign, content calendar, thought leadership, article, case study write-up, content strategy, social content, email sequence, weekly update"
---

# Content Writing

Content writing is the discipline of creating written material that serves a specific purpose for a specific audience. It's not about filling a content calendar — it's about communicating ideas that matter in a way that resonates with the people you're trying to reach.

## Before You Start

**Always load:**
- `${CLAUDE_PLUGIN_ROOT}/frameworks/workflow-orchestration.md` — Universal workflow pattern
- `${CLAUDE_PLUGIN_ROOT}/frameworks/messaging.md` — Messaging hierarchy, value propositions, proof points

**Context (always load):**
- `${CLAUDE_PLUGIN_ROOT}/context/core/identity.md` — Product, positioning
- `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md` — Tone, language rules

**Context (load when relevant):**
- `${CLAUDE_PLUGIN_ROOT}/context/extended/audience.md` — Target audience, how they talk
- `${CLAUDE_PLUGIN_ROOT}/context/extended/proof-points.md` — Case studies, metrics, testimonials
- `${CLAUDE_PLUGIN_ROOT}/context/extended/product.md` — Product features, workflows
- `${CLAUDE_PLUGIN_ROOT}/context/extended/competitive.md` — Competitors, market positioning

**References (load when needed):**
- `${CLAUDE_PLUGIN_ROOT}/skills/content-writing/references/content-formats.md` — Format-specific guides for each content type
- `${CLAUDE_PLUGIN_ROOT}/skills/content-writing/references/distribution-guide.md` — Platform-specific rules, best practices, and adaptation

## Core Principles

1. **One idea per piece.** Every piece of content should have one clear takeaway. If you can't state it in one sentence, you haven't found it yet.
2. **Write for the reader, not the algorithm.** Useful content gets shared. Gaming keywords produces forgettable content.
3. **Voice is everything.** Content that sounds like every other company might as well not exist. The voice.md file is your most important asset here.
4. **Proof over claims.** Every assertion should be backed by evidence — data, case studies, specific examples. Load proof-points.md when making claims.
5. **Lead with value.** Give the reader something useful in the first paragraph. Don't make them scroll to find out if this is worth their time.
6. **Repurpose aggressively.** A good blog post becomes a LinkedIn thread becomes a newsletter becomes a talk. Write once, adapt many times.
7. **Done is better than perfect.** Published content that helps someone beats a draft that never ships.

## Workflow

### 1. Clarify Before Starting
- What type of content? (blog, newsletter, social, email, case study)
- Who is the audience? (load audience.md)
- What's the one takeaway?
- What action should the reader take after?
- What evidence or proof points are available? (load proof-points.md)
- Where will this be published? (determines format, length, tone)

### 2. Choose the Right Format

| Goal | Format | Typical Length |
|------|--------|---------------|
| Establish expertise | Blog post / article | 800-2000 words |
| Nurture existing audience | Newsletter | 300-800 words |
| Drive awareness | LinkedIn post | 100-300 words |
| Quick engagement | Twitter/X thread | 5-15 tweets |
| Direct conversion | Email campaign | 150-400 words per email |
| Build credibility | Case study write-up | 500-1500 words |
| Thought leadership | Long-form article | 2000-4000 words |
| Community building | Social media content | Varies by platform |

### 3. Writing Process

**Research & Outline:**
- Identify the core insight or argument
- Gather supporting evidence (proof-points.md, product.md, competitive.md)
- Outline the structure: hook → main argument → supporting points → conclusion/CTA
- Identify the single most important sentence in the piece

**Draft:**
- Write the hook first — if the first paragraph doesn't earn the second, nothing else matters
- Follow voice.md strictly — this is where brand consistency lives
- Use concrete examples over abstract claims
- Write more than you need, then cut

**Edit:**
- Read it out loud — does it sound like the voice in voice.md?
- Cut everything that doesn't serve the one takeaway
- Check claims against proof-points.md — can you back this up?
- Verify terminology against identity.md
- Ensure the CTA is clear and specific

**Adapt:**
- If repurposing for a different platform, adjust format and length
- Load distribution-guide.md for platform-specific rules
- Keep the core message, change the packaging

## Quality Checks

- [ ] Has one clear takeaway?
- [ ] Hook earns the reader's attention in the first paragraph?
- [ ] Matches voice.md — tone, language rules, words to avoid?
- [ ] Claims backed by evidence from proof-points.md?
- [ ] Terminology consistent with identity.md?
- [ ] Appropriate length for the format and platform?
- [ ] Clear call to action?
- [ ] Would the target audience (audience.md) find this useful?
- [ ] No filler paragraphs — every paragraph earns its place?

## Anti-Patterns

| Anti-Pattern | Instead |
|--------------|---------|
| Writing for everyone | Write for one specific reader from audience.md |
| Starting with "In today's world..." | Start with the insight or a hook |
| Burying the point | Lead with the takeaway, then support it |
| Making claims without evidence | Back every assertion with proof-points.md |
| Sounding like every other company | Follow voice.md aggressively — your voice is the differentiator |
| Perfectionism before publishing | Ship it, learn from the response, iterate |
| One-and-done content | Repurpose across formats and platforms |
| Writing about yourself | Write about the reader's problem, then connect to your solution |
