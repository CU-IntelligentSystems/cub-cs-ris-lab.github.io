# WIP (Work-in-Progress) Entries

This folder contains all work-in-progress log entries.

## Naming Convention

All WIP entries should follow this naming convention:
```
YYYY-MM-DD__<project-slug>__<presenter>.md
```

**Examples:**
- `2026-01-29__sonar-cv__arturo.md`
- `2026-01-29__acoustic-modem-energy-management__hamza-hussain.md`

Use lowercase with hyphens (kebab-case) for project slugs and presenter names.

## Creating a New WIP Entry

1. Copy the `TEMPLATE.md` file
2. Rename it following the naming convention above
3. **Remove** the `published: False` line from the frontmatter
4. Fill in the frontmatter:
   - `title`: "WIP: \<project-slug\> - \<presenter\> [\<YYYY-MM-DD\>]"
   - `date`: YYYY-MM-DD
   - `project`: project slug (must match the project page's `project` field)
   - `presenter`: Full Name
   - `tags`: relevant tags for the entry
   - `status`: current project status
   - `notetaker`: Full Name (person taking notes during the meeting)
5. Fill in the content sections (see Content Sections below)

## Frontmatter Reference

| Field | Required | Description |
|-------|----------|-------------|
| `title` | Yes | "WIP: \<project-slug\> - \<presenter\> [\<date\>]" |
| `layout` | Yes | Always `default` |
| `parent` | Yes | Always `WIP Log` |
| `nav_order` | Yes | Order in sidebar navigation |
| `date` | Yes | Entry date (YYYY-MM-DD) |
| `project` | Yes | Project slug (must match project page) |
| `presenter` | Yes | Presenter's full name |
| `tags` | Yes | List of relevant tags |
| `status` | Yes | Current project status |
| `notetaker` | No | Notetaker's full name |

## Status Values

- `exploring` - Initial research and feasibility study
- `implementing` - Active development
- `experiments` - Running experiments and collecting data
- `writing` - Writing papers or documentation
- `wrapping-up` - Finalizing results
- `maintenance` - Ongoing maintenance
- `concluded` - Project completed

## Content Sections

Each WIP entry has four main sections:

### 1) Snapshot (fill before meeting)
- Project goal (1-3 sentences)
- Summary of this update
- Links to project page, code repo, data, slides
- Publication/writing status

### 2) Since last update: progress (fill before meeting)
- What changed (bullets)
- Key results with metrics
- Artifacts produced (issues, plots, demos)

### 3) Current approach (fill before meeting)
- Method summary (problem, approach, assumptions)
- Setup (robot/hardware, sim/environment)

### 4) Feedback & next steps (fill after meeting)
- Help needed
- Discussion elements (questions, suggestions, concerns)
- Action items (decisions, next steps with owners)

## Project Slugs

Use the same slug as defined in the project's frontmatter. Current projects:
- `sonar-cv`
- `acoustic-modem-energy-management`

For new projects, use lowercase with hyphens (kebab-case).
