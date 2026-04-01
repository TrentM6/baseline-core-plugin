---
description: "Baseline Core voice and formatting — applies the user's voice rules and clean document structure to all output"
---

# Voice & Formatting

Apply these rules to all output.

## Voice

Before producing any output, check if the user's voice context has been loaded from `${CLAUDE_PLUGIN_ROOT}/context/core/voice.md`. If it has, follow those voice rules exactly — tone, person, language rules, words to avoid, and context-specific adjustments.

If no voice context is loaded, use these defaults:
- **Clear and direct.** No hedging, no filler, no over-qualifying.
- **Professional but human.** Sound like a person, not a brand.
- **Specific.** Concrete details over vague claims.
- **Active voice.** Short sentences. Cut anything that doesn't add meaning.

## Formatting

These formatting rules apply regardless of the user's voice settings:

- **One H1 per document.** Clear and specific.
- **H2 for sections, H3 for subsections.** Don't go deeper than H3 unless necessary.
- **Paragraphs:** 2-3 sentences max. No walls of text.
- **Lists:** One line per item, parallel structure, no more than 7 items without grouping.
- **Tables:** 2-4 columns, short cells, clear headers. Use for comparisons and structured data.
- **Bold** for key terms and labels. *Italic* for quotes and slight emphasis. `Code` for technical terms and file names.
- **Blockquotes** for key insights, takeaways, and quotes.
- Use `---` between major sections.
- Everything should be scannable. If someone can't skim headers and understand the document, restructure.

If the user has a `${CLAUDE_PLUGIN_ROOT}/context/extended/formatting.md` file with custom formatting conventions, those override the defaults above.
