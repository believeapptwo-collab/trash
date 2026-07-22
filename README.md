# $TRASH — Official Website

One man's trash is another man's treasure.

A single-page static site for the **$TRASH** memecoin on Robinhood Chain.

- **Contract:** `0x7d7285afa84703021eb63ce75910b155b824c9c2`
- **X / Twitter:** [@trashcoin_rh](https://x.com/trashcoin_rh)
- **Chart:** [DEXScreener](https://dexscreener.com/robinhood/0xddcfc96c1929a96302f9a6eef7a8ff621927228b7b15def509bded85f3b4b226)

## Structure

```
trash-coin-site/
├── index.html                  # the whole site (HTML + CSS + JS)
└── assets/
    ├── favicon.png             # browser tab icon
    ├── trash-bag.webp          # hero image
    ├── memes/                  # meme gallery images
    │   ├── your-opinion-is-trash.webp
    │   ├── your-meme-is-trash.webp
    │   ├── why-is-everything-trash.webp
    │   ├── take-out-the-trash.webp
    │   ├── trash-or-treasure.webp
    │   ├── this-stinks-like-trash.webp
    │   └── trash-narrative-tbh.webp
    └── brand/                  # original full-quality brand resources (not used by the page)
        ├── trash-banner.png
        ├── trash-bag-original.png
        └── pink-gradient.png
```

## Run locally

No build step. Open `index.html` in a browser, or serve the folder:

```
npx serve .
```

## Deploy with GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set Source to **Deploy from a branch**, pick `main` and `/ (root)`, and save.
4. Your site goes live at `https://<username>.github.io/<repo-name>/`.

Also works as-is on Vercel, Netlify, or Cloudflare Pages (no build command, output directory: root).

## Editing

Everything lives in `index.html`:

- **Contract address** — the `<code id="ca">` element in the hero.
- **Chart** — the `<iframe>` in the `#chart` section (DEXScreener embed URL).
- **Social links** — search for `x.com/trashcoin_rh`.
- **Colors** — CSS variables at the top of the `<style>` block (`--pink`, `--paper`, etc.).

## Disclaimer

$TRASH is a meme coin with no intrinsic value and no expectation of financial return. Nothing here is financial advice.
