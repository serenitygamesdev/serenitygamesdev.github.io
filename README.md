# Serenity Games — website

Static site for GitHub Pages. No build step: `index.html` + `assets/`.

- `royal-minesweeper/`, `neon-minesweeper/`, `game-tap/` — privacy policy and terms per game
- `app-ads.txt` — AdMob authorized sellers
- Google Play link for a game: set `data-play` on its `<article class="game">` in `index.html`

Local preview: `python3 -m http.server` and open http://localhost:8000
