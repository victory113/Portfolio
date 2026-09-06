# Portfolio — victoryorobosa

A single-page portfolio. No framework, no build step: one HTML file, one stylesheet
(inline), one script (inline), and a folder of images.

```
portfolio/
├── index.html      The whole site — markup, styles, and behaviour
├── favicon.svg     Browser-tab icon, adapts to light/dark
├── netlify.toml    Netlify config: publish directory, headers, caching
├── assets/         Images referenced by index.html
│   └── dashboard.png
└── README.md
```

## Running it locally

Open `index.html` in a browser, or — better, because it matches how Netlify serves it —
use the VS Code **Live Server** extension: right-click `index.html` → *Open with Live Server*.

## Deploying

Pushed to GitHub and connected to Netlify. Every push to `main` redeploys automatically.

- Build command: *(none)*
- Publish directory: `.`

## After the first deploy

Replace the placeholder domain in the `og:` and `twitter:` meta tags at the top of
`index.html` with the real site URL, so link previews resolve. Those tags are what
render the preview card when the link is pasted into LinkedIn, Slack, or a DM.

## Adding a project

Copy an existing `<article class="project">` block in `index.html` and edit it. Each one has
the same four parts: the `project-top` header (dates, stack, summary, links), an optional
`figure`, a `readout` strip of verified numbers, and one or more `block` sections of prose.

Keep `class="reveal"` on anything that should fade in on scroll.
