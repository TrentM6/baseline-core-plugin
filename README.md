# Baseline Core

A complete AI system for product work. 12 domain skills, 13 shared frameworks, and customizable business context — so every skill works specifically for your business.

## What's Inside

**Skills** — Structured workflows for product work:

| Skill | What it does |
|-------|-------------|
| Strategic Advisory | Roadmaps, prioritization, OKRs, strategic decisions |
| Research & Synthesis | User research, interviews, competitive analysis |
| Product Communications | PRDs, specs, briefs, stakeholder updates |
| UX Design | Interface design, wireframes, flows, UI copy |
| Product Analytics | Metrics, dashboards, A/B tests, segmentation |
| Prototyping | Coded prototypes, demos, POCs |
| Project Management | Planning, sprints, tracking, risk management |
| Technical Documentation | User guides, API docs, release notes |
| Visual Communication | Presentations, diagrams, data visualization |
| Product Marketing | Positioning, messaging, content, launch briefs |
| Go-to-Market Planning | Launch planning, channel strategy, distribution |
| Skill Building | Create new skills for the system |

**Frameworks** — Reusable methodologies that skills draw from: workflow orchestration, prioritization, decision-making, strategy, research, messaging, UX heuristics, project management, stakeholder communication, facilitation, change management, pace layering, and session planning.

**Agents** — Background support that runs alongside skills:
- **Quality Review** — Checks deliverables against your voice, formatting, and content standards
- **Research** — Gathers market, competitive, or domain context without breaking conversation flow
- **Context Loader** — Synthesizes your context files into focused briefs for skills

**Context** — Your business knowledge, loaded by every skill:
- `identity.md` — Who you are, what you do, how you're positioned
- `voice.md` — How you sound, language rules, words to avoid
- `design.md` — Colors, typography, design system
- `formatting.md` — Document structure conventions
- `audience.md` — Who you serve, their pain points, how they talk
- `proof-points.md` — Case studies, metrics, testimonials

## Getting Started

1. Install the plugin
2. Run `/setup` — a guided interview that builds your context files in about 5 minutes
3. Start using skills — every skill now works with your business context

The `/setup` skill asks you about your company, how you communicate, and who you serve, then generates context files from your answers. Identity and voice are required. Design, formatting, audience, and proof points are recommended but optional.

You can run `/setup` again anytime to update your context.

## How It Works

Skills provide methodology. Context makes it yours. Frameworks give structure.

When you trigger a skill (like `/product-marketing` or `/strategic-advisory`), it loads:
1. Your business context (identity + voice, always)
2. Relevant extended context (audience, proof points, etc. — only when needed)
3. Shared frameworks (prioritization, messaging, etc. — based on the skill)
4. Skill-specific references (deeper guidance, loaded on demand)

The plugin's routing brain automatically matches your request to the right skill. If no skill matches, it uses your loaded business context to answer with general product expertise.

## Context Files

Context files are the customizable layer. They live in `context/` and start as templates with instructions. The `/setup` skill populates them through conversation, or you can edit them directly.

| File | Required | Used by |
|------|----------|---------|
| `identity.md` | Yes | Every skill |
| `voice.md` | Yes | Every skill |
| `design.md` | No | Prototyping, UX Design, Visual Communication |
| `formatting.md` | No | Product Communications, Technical Documentation, Quality Review |
| `audience.md` | No | Product Marketing, Go-to-Market, Research |
| `proof-points.md` | No | Product Marketing, Research |

Without context files, skills still work — they just produce generic output. With identity and voice alone, you get 80% of the value. The extended files add depth for specific skills.

## Project Structure

```
baseline-core-plugin/
├── .claude-plugin/plugin.json    # Plugin manifest
├── hooks/hooks.json              # SessionStart routing brain
├── output-styles/                # Voice and formatting enforcement
├── agents/                       # Quality review, research, context loader
├── skills/                       # 12 domain skills + setup
├── frameworks/                   # 13 shared methodologies
└── context/                      # Your business knowledge (customizable)
    ├── core/                     # Identity + voice (required)
    └── extended/                 # Design, formatting, audience, proof points
```

---

Built by [Baseline](https://baselinestudio.co).
