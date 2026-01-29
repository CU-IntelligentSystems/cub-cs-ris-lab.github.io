# Research Lab - Public Log Website

This website serves as the public research log and knowledge base for our Research Lab.

We document ongoing work-in-progress updates, decisions, and lessons learned so results are easy to track over time and simple for new researchers to pick up. Each project page links to relevant code, datasets, experiment artifacts, and meeting logs to promote reproducibility and smooth handovers.

## Website Structure

- **Home** (`index.md`) - Overview and quick links
- **Projects** (`projects.md`) - Summary of all research projects
- **WIP Log** (`wip-log.md`) - Latest work-in-progress entries across all projects
- **People** (`people.md`) - Lab members and their contributions

### Directories

- `projects/` - Individual project pages
- `wip/` - Work-in-progress log entries

## Creating WIP Entries

WIP entries follow a standardized template to ensure consistency and completeness.

1. Copy `wip/TEMPLATE.md`
2. Rename following the convention: `YYYY-MM-DD__<project_slug>__<presenter>.md`
   - Example: `2024-03-15__tactile-grasping__john-doe.md`
3. Fill in the frontmatter and content sections
4. The entry will automatically appear on the WIP Log and People pages

See `wip/README.md` for detailed instructions.

## Technical Details

This site uses:
- [Jekyll] static site generator
- [Just the Docs] theme
- [GitHub Pages] for hosting
- GitHub Actions workflow for automatic deployment

### Building and Previewing Locally

1. Install [Jekyll] and [Bundler]
2. Run `bundle install`
3. Run `bundle exec jekyll serve`
4. Preview at `localhost:4000`

The built site is stored in the `_site/` directory.

### Publishing on GitHub Pages

The site automatically builds and deploys via GitHub Actions when changes are pushed to the main branch.

To set up:
1. Go to Settings > Pages > Build and deployment
2. Select Source: GitHub Actions
3. Push changes to trigger deployment

## Naming Conventions

**Project slugs:** Use lowercase with hyphens (kebab-case)
- Examples: `tactile-grasping`, `legged-locomotion`, `slam-mapping`

**WIP filenames:** `YYYY-MM-DD__<project_slug>__<presenter>.md`
- Examples: `2024-03-15__tactile-grasping__john-doe.md`

## License

This repository is licensed under the MIT License.

---

[Jekyll]: https://jekyllrb.com
[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[Bundler]: https://bundler.io
