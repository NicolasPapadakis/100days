# One Hundred Days

A card a day from 27 August to 4 December 2026. You write one, seal it, and it's gone
until all 100 are done — then they replay in the order they were written.

Built for iPhone-width screens.

## Deploy

`index.html` is a single self-contained file — fonts, runtime and all logic are inlined.
No build step, no dependencies.

**Vercel:** import this repo. Framework preset: **Other**. Leave build command and output
directory empty. Vercel serves `index.html` at the root.

## Files

- `index.html` — the deployable build. This is the file that ships.
- `Hundred Days.dc.html` — the editable source. Re-bundle to `index.html` after changes.
- `support.js` — runtime used by the source file (already inlined into `index.html`).

## Data

Everything is stored locally in the browser (`localStorage`, key `hundred-days.v1`).
Nothing is sent anywhere. The write screen has **Back up** (downloads a JSON of all
entries) and **Restore** (loads one back) for moving between devices or browsers.
