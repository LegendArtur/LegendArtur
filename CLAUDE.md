# CLAUDE.md

## Repository Overview

This is **LegendArtur/LegendArtur**, a GitHub profile repository for Artur Gubaidullin. GitHub renders `README.md` from this special-purpose repository directly on the user's profile page at `github.com/LegendArtur`.

## Repository Structure

```
LegendArtur/
└── README.md    # GitHub profile page content (HTML + Markdown)
```

There is no source code, build system, or dependencies — only a single static content file.

## File: README.md

The profile page uses a combination of HTML and Markdown:

- **Header image**: A banner image hosted on GitHub's user-content CDN
- **Badges**: Shields.io badges wrapped in HTML `<div>` elements for centered layout
- **LinkedIn link**: Points to `https://www.linkedin.com/in/arturgub/`

### Conventions

- Use `align="center"` on wrapper `<div>` elements for centered sections
- Badges use `style=for-the-badge` from shields.io
- Keep the HTML comment block at the top (lines 1–14) — it's a GitHub-provided template reference

## Development Workflow

Since there is no build step, the workflow is:

1. Edit `README.md`
2. Commit with a descriptive message (e.g., `Update README.md: add skills section`)
3. Push to `master` — changes appear on the GitHub profile immediately

### Branch Convention

- `master` is the production branch (rendered on the profile)
- Feature branches follow the pattern `<source>/description` (e.g., `claude/add-claude-documentation-BgwfL`)

## Git Conventions

- Commits are GPG-signed
- Commit messages are short and descriptive: `Update README.md (<brief description>)`
- Single contributor: Artur Gubaidullin

## Guidelines for AI Assistants

- **Do not** add build tools, package managers, or unnecessary config files — this repo intentionally has minimal structure
- **Do not** convert the README to pure Markdown if it uses HTML for layout — HTML is intentional for centering and badge display
- **Do** keep the profile README concise and visually clean
- **Do** preserve the existing HTML structure when adding new sections
- **Do** use shields.io badge format (`img.shields.io/badge/...?style=for-the-badge`) when adding new badges
- Any new sections should follow the existing centered `<div>` pattern for consistency
