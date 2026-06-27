# 🍞 Bread Zaddy

Just some vibe-coded games — a **mobile** version and a **desktop** version.

Live at [breadzaddy.com](https://breadzaddy.com). Both games live in one
`index.html`: it sniffs your device (phone → mobile, otherwise → desktop) and
runs the chosen one. Force a version with `?v=mobile` or `?v=desktop`.

## What's here

| File | What it is |
|---|---|
| `src/desktop.html` | The desktop game (single self-contained file) — **edit here** |
| `src/mobile.html` | The mobile game (single self-contained file) — **edit here** |
| `index.html` | Built artifact: both games inlined; `?v=` (or device sniff) picks which runs |
| `build.mjs` | Compiles `src/*` → `index.html` |
| `public/radio/` | Shared radio audio clips |

## Develop

Edit the games in `src/`, then rebuild the page GitHub Pages serves:

```
npm run build     # src/desktop.html + src/mobile.html  ->  index.html
npm run serve     # static server on http://localhost:8000
npm run dev       # build, then serve
```

`index.html` is generated — never hand-edit it (it's committed only because GitHub
Pages serves it directly). Always edit `src/` and run `npm run build`.
