# Portfolio — Victory Orobosa

**Live site: [victoryorobosa.netlify.app](https://victoryorobosa.netlify.app/)** ·
[Resume (PDF)](https://victoryorobosa.netlify.app/assets/Victory-Orobosa-Resume.pdf) ·
[LinkedIn](https://www.linkedin.com/in/victory-orobosa/)

The projects on it:

- **[AI Supply Chain Intelligence Platform](https://github.com/victory113/supply-chain-analyzer)** — turns any shipment CSV into computed KPIs, a risk score, and grounded explanations. [Live demo](https://supply-chain-analyzer.netlify.app/)
- **[SearchFlix](https://github.com/victory113/searchflix)** — which index should a search engine use? Seven data structures benchmarked over 12.4M IMDb titles
- **[Double DQN — Lunar Lander](https://github.com/victory113/dqn-lunar-lander)** — a reinforcement learning ablation that contradicted the expected result

A single-page portfolio. No framework, no build step: one HTML file, one stylesheet
(inline), one script (inline), and a folder of images.

```
portfolio/
├── index.html      The whole site — markup, styles, and behaviour
├── favicon.svg     Browser-tab icon, adapts to light/dark
├── netlify.toml    Netlify config: publish directory, headers, caching
├── assets/         Files referenced by index.html
│   ├── dashboard.png, dqn_divergence.png, searchflix-compare.png   project screenshots
│   ├── og-card.png                  the link-preview card
│   └── Victory-Orobosa-Resume.pdf   the resume linked from the header and contact card
└── README.md
```

## Running it locally

Open `index.html` in a browser, or — better, because it matches how Netlify serves it —
use the VS Code **Live Server** extension: right-click `index.html` → *Open with Live Server*.

## Deploying

Pushed to GitHub and connected to Netlify. Every push to `main` redeploys automatically.

- Build command: *(none)*
- Publish directory: `.`

## Link previews

The `og:` and `twitter:` meta tags at the top of `index.html` point at
`https://victoryorobosa.netlify.app/` and `assets/og-card.png`. They render the
preview card when the link is pasted into LinkedIn, Slack, or a DM. If the site
ever moves to a custom domain, update them and the `canonical` link together.

## Adding a project

Copy an existing `<article class="project">` block in `index.html` and edit it. Each one has
the same four parts: the `project-top` header (dates, stack, summary, links), an optional
`figure`, a `readout` strip of verified numbers, and one or more `block` sections of prose.

Keep `class="reveal"` on anything that should fade in on scroll.
