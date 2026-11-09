# Bali Notion Weather Widget 🌴

A simple dark-mode, single-file weather widget for one chosen day and location. Intended for Notion `/embed` blocks.

## Publish on GitHub Pages

1. Create a **public** GitHub repository named `bali-notion-weather` (check **Add a README file** if using GitHub's site).
2. Upload the supplied `index.html` file into the repository root (or paste it using Add file → Create new file → `index.html`).
3. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**. Select `main`, `/ (root)`, then **Save**.
4. When it publishes, the page is at `https://JadyMcIntyre.github.io/bali-notion-weather/`.
5. In Notion, type `/embed`, paste one of the URLs below, and resize the block to roughly 240px tall.

## URL examples

- Sunday 29 November in Legian:
  `https://JadyMcIntyre.github.io/bali-notion-weather/?date=2026-11-29&location=Legian%2C%20Bali`
- Monday 30 November in Nusa Penida:
  `https://JadyMcIntyre.github.io/bali-notion-weather/?date=2026-11-30&location=Nusa%20Penida%2C%20Bali`
- Shorter version for a small Notion embed:
  `https://JadyMcIntyre.github.io/bali-notion-weather/?date=2026-11-29&location=Legian%2C%20Bali&compact=1`

The widget uses the **Visual Crossing Weather Timeline API** directly, without requiring an API key, as documented October 2026. Its free no-key service is subject to fair-use limits and requires attribution; the widget includes attribution. Data is cached for four hours locally to reduce requests.

> **Accuracy:** This is not a reliable day-specific forecast more than ~14 days out. The page labels long-range results `Seasonal estimate` and changes to a forecast when the date approaches.

## Troubleshooting

- GitHub Pages can take several minutes to publish after enabling it.
- If the widget says it cannot load weather, check the browser's developer console/network tab. Anonymous API limits or browser cross-origin access may affect requests; this setup has not been verified against the live API inside ChatGPT's environment.
- If a Notion embed fails, open the GitHub Pages URL in a browser first to check that the page has published.
