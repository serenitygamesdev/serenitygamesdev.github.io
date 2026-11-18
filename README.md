# Serenity Games — website

Static site for GitHub Pages. No build step: `index.html` + `assets/`.

- `royal-minesweeper/`, `neon-minesweeper/`, `game-tap/` — privacy policy and terms per game
- `app-ads.txt` — AdMob authorized sellers
- Google Play link for a game: set `data-play` on its `<article class="game">` in `index.html`

Local preview: `python3 -m http.server` and open http://localhost:8000

## QR codes

`assets/img/qr-*.svg` are generated with [segno](https://pypi.org/project/segno/):

```python
import segno
segno.make(URL, error='m').save("assets/img/qr-NAME.svg", scale=1, border=2, dark="#0e1024", light="#ffffff", xmldecl=False)
```

then replace `width="N" height="N"` in the SVG with `viewBox="0 0 N N"`.
