# Design

<!-- RECOMMENDED: This file defines your visual identity, design system, and UI patterns. Skills like Prototyping, UX Design, and Visual Communication use this to produce on-brand, production-ready output. -->
<!-- Fill in the sections that apply to you. The more detail you provide, the more accurate and consistent the output will be. -->
<!-- To generate this file automatically, run the /plugin-setup skill. -->

## Visual Theme & Atmosphere

(Describe the overall feel and personality of your design. What emotion or impression should someone get when they see your product or brand? Example:)
(- Clean, minimal, and professional — no decoration for decoration's sake)
(- Warm and approachable, not cold or corporate)
(- Information-dense but not cluttered — every element earns its place)

## Color Palette & Roles

(List your colors organized by their role in the system. Include hex values. Example:)

### Primary Colors
(- Brand Primary: #0066cc — buttons, links, primary actions)
(- Brand Secondary: #1a1a1a — text, headings)

### Surface & Background Colors
(- Page Background: #ffffff)
(- Card Background: #f9fafb)
(- Dark Surface: #1a1a1a — for inverted sections)
(- Hover/Active State: #f3f4f6)

### Semantic Colors
(- Success: #16a34a)
(- Warning: #f59e0b)
(- Error: #dc2626)
(- Info: #3b82f6)

### Neutrals
(- Text Primary: #111827)
(- Text Secondary: #6b7280)
(- Text Muted: #9ca3af)
(- Border: #e5e7eb)
(- Divider: #f3f4f6)

### Gradient System
(If you use gradients, describe them. If not, note that — e.g., "No gradients. Depth comes from surface layering and subtle shadows.")

## Typography

(Define your type system with specific sizes, weights, and usage. Example:)

### Font Families
(- Headlines: Inter — bold, confident, modern)
(- Body: Inter — clean, readable at all sizes)
(- Code: JetBrains Mono — monospaced, for technical content)

### Type Scale
(Define your hierarchy with specific values. Example:)

| Level | Size | Weight | Line Height | Letter Spacing | Usage |
|-------|------|--------|-------------|----------------|-------|
| Display | 48px | 700 | 1.1 | -0.02em | Hero headlines |
| H1 | 36px | 700 | 1.2 | -0.01em | Page titles |
| H2 | 24px | 600 | 1.3 | 0 | Section headings |
| H3 | 20px | 600 | 1.4 | 0 | Subsection headings |
| Body | 16px | 400 | 1.6 | 0 | Default text |
| Body Small | 14px | 400 | 1.5 | 0 | Secondary text |
| Caption | 12px | 500 | 1.4 | 0.01em | Labels, metadata |

### Typography Principles
(Any rules about how type is used. Example:)
(- One font weight for headings, one for body — no mixing)
(- Generous line height on body text for readability)
(- Tight letter spacing on large headings, slightly open on small labels)

## Component Stylings

(Describe how your key UI components look and behave. Example:)

### Buttons
(- Primary: filled background, white text, 8px radius, medium shadow)
(- Secondary: outlined, border color matches text, 8px radius)
(- Ghost: text only, no border, subtle hover background)
(- Sizes: small (32px height), medium (40px), large (48px))
(- Padding: 12px horizontal minimum, asymmetric for icon+text)

### Cards & Containers
(- Background: card surface color, 1px border)
(- Border radius: 12px for cards, 8px for inner elements)
(- Padding: 24px standard, 16px compact)
(- Shadow: subtle — e.g., 0 1px 3px rgba(0,0,0,0.1))

### Inputs & Forms
(- Height: 40px standard)
(- Border: 1px solid border color, 8px radius)
(- Focus state: 2px ring in primary color)
(- Labels: above input, 14px, medium weight)
(- Error state: red border, error message below)

### Navigation
(- Style: sticky top bar, clean background, clear hierarchy)
(- Active state: primary color underline or background)
(- Mobile: hamburger menu collapse)

### Tables
(- Header: slightly darker background, bold text)
(- Rows: alternating background or divider lines)
(- Cell padding: 12px horizontal, 8px vertical)

### Modals & Overlays
(- Backdrop: semi-transparent dark overlay)
(- Modal: card-style with close button, max-width constrained)
(- Animation: subtle fade or slide)

## Layout Principles

(Describe the foundational rules for how things are arranged. Example:)

### Spacing System
(- Base unit: 8px)
(- Scale: 4, 8, 12, 16, 24, 32, 48, 64, 96)
(- Section spacing: 64-96px between major sections)
(- Component spacing: 16-24px between related elements)

### Grid & Container
(- Max content width: 1200px, centered)
(- Column system: 12-column grid, 24px gutters)
(- Side padding: 16px mobile, 24px tablet, 32px desktop)

### Whitespace Philosophy
(How you think about empty space. Example:)
(- Generous margins between sections — let content breathe)
(- Tight spacing within related groups — proximity signals relationship)
(- Content islands: distinct sections with clear visual separation)

## Layout Patterns

(Define how specific page types or views are structured. Include the ones that apply to your product. Example:)

### Dashboard
(- Top: header with navigation and user actions)
(- Left: optional sidebar for navigation or filters)
(- Main: card grid or data panels, 2-3 columns on desktop)
(- Key metrics at top, detailed views below)

### Detail / Single Item View
(- Top: breadcrumb + title + actions)
(- Body: content area with optional sidebar for metadata)
(- Bottom: related items or activity feed)

### List / Table View
(- Top: search, filters, bulk actions)
(- Body: table or card list with pagination)
(- Empty state: illustration + CTA)

### Form / Editor
(- Single column, max-width 640px for readability)
(- Sections grouped with headings)
(- Actions pinned to bottom or top-right)

### Chat / Conversation
(- Messages: alternating alignment or color for sender/receiver)
(- Input: fixed to bottom, expandable textarea)
(- Timestamps: subtle, grouped by date)

### Kanban / Board
(- Horizontal scrolling columns)
(- Cards: draggable, compact information density)
(- Column headers with counts and add actions)

### Settings / Configuration
(- Left sidebar navigation for sections)
(- Right content area with form groups)
(- Save actions per section or global)

### Landing / Marketing Page
(- Hero: centered headline, subhead, CTA)
(- Feature sections: alternating layout, 2-3 columns)
(- Social proof: logos, testimonials, metrics)
(- Footer: links, legal, newsletter)

(Delete any layout patterns that don't apply to your product. Add custom ones that do.)

## Depth & Elevation

(How you create visual hierarchy through shadows and layering. Example:)

| Level | Usage | Style |
|-------|-------|-------|
| Flat | Default state, inline elements | No shadow, no border |
| Subtle | Cards, containers | 1px border or very soft shadow |
| Raised | Dropdowns, popovers, tooltips | Medium shadow (0 4px 12px rgba(0,0,0,0.1)) |
| Overlay | Modals, drawers, full overlays | Heavy shadow + backdrop |

### Depth Principles
(- Use shadow sparingly — most depth comes from surface color and borders)
(- Consistent shadow direction (top-down light source))
(- Interactive elements should feel slightly raised on hover)

## Do's and Don'ts

### Do
(- Maintain consistent spacing using the 8px grid)
(- Use semantic colors for their intended purpose)
(- Keep text readable — minimum 14px for body, adequate contrast)
(- Use whitespace generously between sections)
(- Follow the established component patterns)

### Don't
(- Don't mix border radius styles — pick one scale and stick with it)
(- Don't use more than 2-3 font weights total)
(- Don't create new color values — use the palette)
(- Don't add shadows where borders would suffice)
(- Don't sacrifice readability for aesthetics)

## Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|------|-------|-------------|
| Mobile | < 640px | Single column, stacked layout, hamburger nav |
| Tablet | 640-1023px | 2-column where appropriate, condensed spacing |
| Desktop | 1024px+ | Full layout, sidebar visible, multi-column grids |

### Responsive Principles
(- Mobile-first: design for small screens, enhance for larger)
(- Touch targets: minimum 44x44px on mobile)
(- Navigation collapses to hamburger on mobile)
(- Multi-column grids stack to single column)
(- Typography scales down proportionally — don't just shrink everything)
(- Images: responsive, maintain aspect ratio, constrained to container)

## Logo & Brand Assets

(Describe your logo usage rules and where assets live. Example:)
(- Primary logo: dark text on light backgrounds)
(- Inverse logo: white text on dark backgrounds)
(- Minimum clear space: 16px on all sides)
(- Minimum size: 24px height)
(- Assets location: /brand/assets/ or Figma link)

## Design Principles

(3-5 principles that guide all design decisions. These should be opinionated — if the opposite is also reasonable, it's a real principle. Example:)
(- Clarity over decoration — every element earns its place)
(- Consistency over novelty — use established patterns before inventing new ones)
(- Accessible by default — WCAG AA minimum, no exceptions)
(- Dense but not cluttered — maximize information without overwhelming)
(- Fast over fancy — no animations that slow down the experience)
