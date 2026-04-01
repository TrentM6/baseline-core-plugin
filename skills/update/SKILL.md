---
description: "Update — Pull the latest Baseline Core skills, frameworks, agents, and hooks from GitHub while preserving your business context. Triggers: update, upgrade, get latest version, update plugin, update skills, check for updates, new version"
---

# Update

This skill updates your Baseline Core plugin to the latest version from GitHub. It replaces system files (skills, frameworks, agents, hooks, output styles) while preserving your business context files.

**Your context files are never touched. Only Baseline Core system files get updated.**

## Before You Start

No files need to be loaded — this skill manages the update process directly.

## Core Principles

1. **Never touch context.** The `context/` folder is the user's business knowledge. It is never modified, overwritten, or deleted during an update. This is the most important rule.
2. **Show what changed.** After updating, clearly report what was added, changed, or removed so the user knows what's new.
3. **Preserve custom skills.** If the user has added custom skills (via /skill-building), those should not be removed. Only update skills that match the names of official Baseline Core skills.
4. **Confirm before acting.** Show the user what will change before making any modifications. Updates should not be automatic.

## Workflow

### Phase 1: Check Current Version

**Purpose:** Understand what version the user has.

**What to do:**
1. Read `${CLAUDE_PLUGIN_ROOT}/.claude-plugin/plugin.json` to get the current version
2. Tell the user what version they're running

**Done when:** The user knows their current version.

---

### Phase 2: Fetch Latest Version

**Purpose:** Get the latest Baseline Core files from GitHub.

**What to do:**
1. Clone or download the latest version from `https://github.com/TrentM6/baseline-core-plugin`
2. Compare the fetched version against the current version
3. If they're the same, tell the user they're up to date and stop
4. If there's a newer version, proceed to Phase 3

**Done when:** You have the latest files and know what's different.

---

### Phase 3: Show Changes

**Purpose:** Let the user see what will change before applying anything.

**What to do:**
1. Compare the fetched files against the current plugin files
2. Identify:
   - **New skills** — skills that exist in the latest version but not locally
   - **Updated skills** — skills that have changed (different content)
   - **New frameworks** — frameworks added in the latest version
   - **Updated frameworks** — frameworks that have changed
   - **Updated agents** — any changes to agent files
   - **Updated hooks** — any changes to hooks.json
   - **Updated output styles** — any changes to output style files
   - **New context templates** — new context files added (will be added as empty templates, not overwriting existing populated files)
3. Present a summary: "Here's what will change:"
   - List each change with the file name and what's different
   - Clearly note: "Your context files will not be modified"
4. Ask: "Want to proceed with the update?"

**Done when:** The user has reviewed and approved the changes.

---

### Phase 4: Apply Update

**Purpose:** Update the system files while preserving context.

**What to do:**
1. Replace these directories/files with the latest versions:
   - `skills/` — Replace all official Baseline Core skill folders. Do NOT delete folders that don't exist in the latest version (they may be custom skills the user created).
   - `frameworks/` — Replace all framework files
   - `agents/` — Replace all agent files
   - `hooks/hooks.json` — Replace the hook file
   - `output-styles/` — Replace all output style files
   - `.claude-plugin/plugin.json` — Update the version number
2. For any NEW context template files in the latest version:
   - If the user doesn't have that file yet, add it as a template
   - If the user already has a populated version, do NOT overwrite it
3. **DO NOT touch** any existing files in `context/core/` or `context/extended/` that have real content

**Done when:** All system files are updated.

---

### Phase 5: Summary

**Purpose:** Confirm what was updated.

**What to do:**
1. List everything that was updated
2. If new skills were added, briefly describe what they do
3. If new context templates were added, mention them and suggest running /setup to populate them
4. Confirm the new version number
5. Suggest starting a fresh session to use the updated plugin

**Done when:** The user knows what changed and how to use the new features.

## Quality Checks

- [ ] No context files were modified or deleted
- [ ] Custom skills (user-created) were preserved
- [ ] Version number in plugin.json was updated
- [ ] User approved the changes before they were applied
- [ ] Summary accurately reflects what changed

## Anti-Patterns

- **Don't auto-update.** Always show changes and get approval first.
- **Don't touch context.** Even if context file templates have changed in the new version, don't overwrite populated context files. The user's business knowledge is sacred.
- **Don't delete custom skills.** If a skill folder exists locally but not in the latest version, it's probably a custom skill the user created. Leave it alone.
- **Don't skip the summary.** The user needs to know what changed so they can take advantage of new features.
