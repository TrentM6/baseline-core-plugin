# Baseline Core

A complete AI system for product work. 12 domain skills, 13 shared frameworks, and customizable business context — so every skill works specifically for your business.

Skills provide methodology. Context makes it yours. Frameworks give structure.

## Getting Started

Baseline Core ships with templates for business context. You customize it once for your business, then upload your version as a plugin to Claude.

### 1. Download

Clone this repo or download the zip:

```
git clone https://github.com/TrentM6/baseline-core-plugin.git
```

### 2. Set Up Your Context

Open the folder with Claude Code and run `/setup`. It's a guided interview that asks about your business and generates your context files.

The setup skill will walk you through:
- **Identity** (required) — What you do, how you're positioned, what makes you different
- **Voice** (required) — How you sound, language rules, words to avoid
- **Product** (recommended) — What your product does, features, how it works
- **Users** (recommended) — User personas, goals, pain points
- **Audience** (recommended) — Who you market and sell to, buyer personas
- **Competitive** (recommended) — Competitors, market positioning, alternatives
- **Design** (recommended) — Colors, typography, design system
- **Formatting** (recommended) — Document structure conventions
- **Proof Points** (recommended) — Case studies, metrics, testimonials
- **Pricing** (recommended) — Pricing model, tiers, objection handling
- **Technical** (recommended) — Tech stack, architecture, integrations

Identity and voice are required — they get you most of the value. The rest adds depth for specific skills.

### 3. Upload to Claude

Once your context is populated, zip the folder and upload it as a plugin in Claude. Your customized plugin now works in any project, any directory — your business context travels with it.

### Updating Your Context

To update your context, go back to your local copy, edit the files in `context/` (or re-run `/setup`), re-zip, and re-upload.

### Updating the Plugin

When a new version of Baseline Core is released, run `/update` to pull the latest skills, frameworks, agents, and hooks from GitHub. Your context files are never touched — only system files get updated. After updating, re-zip and re-upload.

## What's Inside

**12 Skills** — Structured workflows for product work:

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

**13 Frameworks** — Reusable methodologies that skills draw from: workflow orchestration, prioritization, decision-making, strategy, research, messaging, UX heuristics, project management, stakeholder communication, facilitation, change management, pace layering, and session planning.

**3 Agents** — Background support that runs alongside skills:
- **Quality Review** — Checks deliverables against your voice, formatting, and content standards
- **Research** — Gathers market, competitive, or domain context without breaking conversation flow
- **Context Loader** — Synthesizes your context files into focused briefs for skills

**11 Context Files** — Your business knowledge, loaded by skills on demand:

| File | Required | Used by |
|------|----------|---------|
| `identity.md` | Yes | Every skill |
| `voice.md` | Yes | Every skill |
| `product.md` | No | UX Design, Prototyping, Product Communications, Technical Documentation |
| `users.md` | No | UX Design, Research & Synthesis, Product Analytics |
| `audience.md` | No | Product Marketing, Go-to-Market, Research |
| `competitive.md` | No | Product Marketing, Go-to-Market, Research, Strategic Advisory |
| `design.md` | No | Prototyping, UX Design, Visual Communication |
| `formatting.md` | No | Product Communications, Technical Documentation, Quality Review |
| `proof-points.md` | No | Product Marketing, Research |
| `pricing.md` | No | Go-to-Market Planning, Product Marketing |
| `technical.md` | No | Prototyping, Technical Documentation |

## How It Works

When you trigger a skill (like `/product-marketing` or `/strategic-advisory`), it loads:
1. Your business context (identity + voice, always)
2. Relevant extended context (product, users, audience, etc. — only when needed)
3. Shared frameworks (prioritization, messaging, etc. — based on the skill)
4. Skill-specific references (deeper guidance, loaded on demand)

The plugin's routing brain automatically matches your request to the right skill. If no skill matches, it uses your loaded business context to answer with general product expertise.

## Project Structure

```
baseline-core-plugin/
├── .claude-plugin/plugin.json    # Plugin manifest
├── hooks/hooks.json              # SessionStart routing brain
├── output-styles/                # Voice and formatting enforcement
├── agents/                       # Quality review, research, context loader
├── skills/                       # 12 domain skills + setup + update
├── frameworks/                   # 13 shared methodologies
└── context/                      # Your business knowledge (customizable)
    ├── core/                     # Identity + voice (required)
    └── extended/                 # Product, users, audience, competitive, design,
                                  # formatting, proof points, pricing, technical
```

---

Built by [Baseline](https://baselinestudio.co).
