# Founder Scorecard

Free, no-login checks for any business or idea:

1. **Idea score (MOAT):** Margin, Operations, Advantage, TAM, each 1 to 10. Fund it, fix it, or flee it.
2. **Price headroom:** what your close rate says about your price, and the profit effect of a raise.
3. **30-day cash:** whether each customer's first 30 days of cash covers 2× the cost to get and serve them.
4. **Old email list:** what one reactivation offer to past customers might bring in.

Based on frameworks Codie Sanchez, Alex Hormozi, and Daniel Priestley shared on The Diary of a CEO. Not affiliated with or endorsed by them or the show. Educational rules of thumb only.

- Full app and API (Vercel): https://fund-fix-flee.vercel.app
- Scorecard (GitHub Pages): https://akiba-labs.github.io/founder-scorecard/

```
npm install
npm test
npm run build
npm run build:pages
```

`npm run build` is the Vercel app (scorecard, JSON API, share pages). `npm run build:pages` writes a static `out/` for GitHub Pages and checks that internal links and assets resolve under `/founder-scorecard`. Server routes stay in the repo; the Pages script only moves them aside for that build.

GitHub settings: **Settings → Pages → Build and deployment → Source: GitHub Actions**. Pushes to `main` deploy with `.github/workflows/pages.yml`. The copy-paste steps for the other tool repos are at the top of `scripts/build-pages.mjs`.
