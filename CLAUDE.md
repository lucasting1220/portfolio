# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Local Development

No build tools or dependencies. Open directly in a browser:

```bash
open index.html
# or serve locally:
npx serve .
```

## Architecture

The entire site is a single file: `index.html`. All HTML, CSS, and JavaScript live there — no bundler, no framework, no npm.

**Sections (in order):**
- `#hero` — landing screen with intro and CTA buttons
- `#journey` — animated timeline of experience/education + skills
- `#connect` — contact form and social links

**JavaScript (three features, all in a `<script>` tag at end of `<body>`):**
- Navbar scroll blur — adds `.scrolled` class to `#navbar` on scroll
- Timeline animations — `IntersectionObserver` fades `.timeline-entry` elements in as they scroll into view
- Contact form — `mailto:` fallback; replace with Formspree `action` URL to avoid opening a mail client

**CSS variables** (defined on `:root`) control the entire dark theme: `--bg`, `--surface`, `--text-primary`, `--text-secondary`, `--accent-primary`, `--border`.

**Responsive breakpoint:** 768px — timeline goes single-column, nav collapses.

## Open To-Dos

- Add Projects section
- Replace placeholder GitHub/LinkedIn URLs (`/lucasting`, `/in/lucasting`) with real ones
- Wire contact form to Formspree (`<form action="https://formspree.io/f/YOUR_ID" method="POST">`)
- Add favicon
