# Posadas Leñatero

Portfolio project derived from a **technical audit and refactor** of an existing hospitality website. The project focuses on clean static architecture, semantic HTML, responsive CSS, and a disciplined Git workflow, rather than framework usage.

**Live URL:** [https://posadas-lenatero.vercel.app/](https://posadas-lenatero.vercel.app/)

---

## Overview

This project originated as a **website audit** (structure, assets, accessibility, and deployment). It was later evolved into a **personal portfolio project** to demonstrate:

* Static site best practices
* Semantic and accessible HTML
* Maintainable CSS architecture
* Correct asset handling on Vercel
* Professional Git workflow and documentation

---

## Tech Stack

* **HTML5** (semantic structure, accessibility attributes)
* **CSS3** (custom reset, responsive layout, component-based sections)
* **JavaScript**: none (pure static site)
* **Vercel** (static hosting and CI/CD)

No frameworks, preprocessors, or build tools are used.

---

## Project Structure

```
/
├─ assets/
│  ├─ images/     # Content and UI imagery
│  ├─ icons/      # UI and action icons (SVG / WebP)
│  └─ styles/
│     └─ style.css
├─ favicon.ico
├─ index.html
└─ README.md
```

---

## HTML Structure

The HTML is organized around clear semantic sections:

* `header` with fixed navigation
* `nav` with accessible labels
* `main` content wrapper
* `section.hero` (hero image, overlay, CTA)
* `section#rates` (pricing grid with semantic `article` cards)

Accessibility considerations include:

* `aria-label` usage in navigation
* Descriptive `alt` attributes
* Logical heading hierarchy

---

## CSS Architecture

The CSS follows a clear, readable structure:

1. Global reset and defaults
2. Typography and base elements
3. Layout primitives (containers, grids)
4. Component sections:

   * Header / Navigation
   * Hero section
   * Pricing cards and grids

Design considerations:

* Responsive layout without media-query bloat
* High-contrast pricing elements
* Reduced-motion support
* Fixed header offset handling via `scroll-margin-top`

---

## Local Development

This is a fully static project.

You can run it by:

* Opening `index.html` directly in the browser, or
* Serving it with any static server (optional)

No installation or build steps are required.

---

## Deployment

* Deployment is handled automatically by **Vercel**
* The `main` branch represents **production**
* Any push to `main` triggers a production deployment

Static assets are served directly from the project root and `assets/` directory.

---

## Git Workflow

This project uses a **branch-per-change** workflow.

### Permanent Branch

* `main` → production (Vercel)

### Temporary Branches

Branches are created only when needed and deleted after merge.

```
feature/<short-description>   # New features
fix/<short-description>       # Bug fixes
chore/<short-description>     # Maintenance / config / structure
refactor/<short-description>  # Code improvements (no visual change)
hotfix/<short-description>    # Emergency production fixes
```

### Examples

```
feature/hero-section
fix/favicon-vercel-path
chore/vercel-static-structure
refactor/semantic-html
```

---

## Commit Message Guidelines

Commits are written in imperative, descriptive form.

Examples:

```
Fix favicon absolute path for Vercel
Add hero section CTA
Refactor semantic HTML structure
Chore clean unused assets
```

---

## Purpose

This repository exists to:

* Serve as a **personal portfolio project**
* Demonstrate real-world static site decisions
* Showcase clean HTML/CSS architecture
* Document a professional Git workflow suitable for collaboration

---

## License

This project is intended for portfolio and demonstration purposes.
