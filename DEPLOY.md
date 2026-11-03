# Deploy (GitHub Pages) — do not run without operator approval

This tree is a **static** site (no build step required).

## Option A — user site repo `D3F4UL7T/D3F4UL7T.github.io`

1. Create empty repo `D3F4UL7T.github.io` (public).
2. Copy contents of `d3f4ult-site/` to repo root (including `css/`, `index.html`, …).
3. Settings → Pages → Deploy from branch `main` / root.
4. Site URL: `https://d3f4ul7t.github.io/`

## Option B — project pages

1. Create repo e.g. `D3F4UL7T/site`.
2. Push site files to `main`.
3. Settings → Pages → branch `main` / root (or `/docs`).
4. URL: `https://d3f4ul7t.github.io/site/`

## Profile README

Copy `github-profile/README.md` into the special repo `D3F4UL7T/D3F4UL7T` as `README.md`.

## Workflow (optional)

If you later want Actions, use `actions/upload-pages-artifact` only after you enable Pages. Not required for pure static HTML.

## Verify

- Open `index.html` locally in a browser.
- Check mobile width (~375px).
- Confirm all nav links and GitHub URLs.
- Ensure no tokens in files (`grep -R ghp_ .` should be empty).
