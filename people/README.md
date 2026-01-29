# People Directory

This folder contains individual markdown files for each lab member.

## Adding a New Person

1. Copy `TEMPLATE.md`
2. Rename to `firstname__lastname.md` (lowercase, double underscore between first and last name)
   - Use hyphens for double last names: `maria__garcia-lopez.md`
3. Fill in the frontmatter fields

## Frontmatter Fields

| Field | Required | Description | Options |
|-------|----------|-------------|---------|
| `name` | Yes | First name | |
| `last_name` | Yes | Last name | |
| `group` | Yes | Lab role category | `faculty`, `phd`, `masters`, `undergrad`, `external` |
| `honorific_title` | No | Title prefix | e.g., `Dr.`, `Prof.` |
| `last_degree` | No | Highest degree | e.g., `PhD`, `MSc`, `BSc` |
| `public_url` | No | Personal website | Full URL |
| `status` | No | Activity status | `Active`, `Inactive` |
| `offboard` | No | Left the group | `Yes`, `No` |
| `research_focus` | No | Brief research description | |
| `projects` | No | Associated project slugs | e.g., `[sonar-cv, slam-mapping]` |

## Group Values

- `faculty` - Faculty and staff members
- `phd` - PhD students
- `masters` - Master's students
- `undergrad` - Undergraduate students
- `external` - External collaborators

## Offboarding

When a member leaves the lab, set `offboard: Yes`. They will be moved to the Alumni section automatically.
