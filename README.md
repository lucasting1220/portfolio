# Lucas Ting — Personal Portfolio

Personal website built with vanilla HTML, CSS, and JavaScript.

## Structure

```
lucasting_portfolio/
├── index.html              # Main site (single-page)
├── Lucas_Ting_Resume.pdf   # Resume for download
└── README.md
```

## Sections

- **Hero** — Intro, bio, and CTAs
- **My Journey** — Animated experience & education timeline
- **Connect With Me** — Contact form + social links

## Local Development

No build tools required. Just open `index.html` in a browser:

```bash
open index.html
```

Or serve it locally:

```bash
npx serve .
```

## Deployment

Drop the folder contents into any static host:

| Host | Command |
|------|---------|
| [Vercel](https://vercel.com) | `vercel deploy` |
| [Netlify](https://netlify.com) | Drag & drop folder |
| GitHub Pages | Push to `gh-pages` branch |

## Contact Form

The form uses a `mailto:` fallback by default. To receive messages without opening a mail client, replace the form's `submit` handler in `index.html` with a [Formspree](https://formspree.io) endpoint:

```html
<form action="https://formspree.io/f/YOUR_ID" method="POST">
```

## To-Do

- [ ] Add Projects section
- [ ] Add GitHub/LinkedIn real URLs
- [ ] Wire up contact form to Formspree
- [ ] Add favicon
