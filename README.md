# Why Cells "Turn Off" & Chronic Disease

A curated, human-readable study wiki distilling **Part 1** (complete public text) of A Midwestern Doctor's three-part Cell Danger Response series:

> A Midwestern Doctor (Feb 1, 2026). ["Why Do Cells 'Turning Off' Underlie So Many Chronic Diseases?"](https://www.midwesterndoctor.com/p/why-do-cells-turning-off-underlie). *The Forgotten Side of Medicine* (Substack), integrating Dr. Robert K. Naviaux's Cell Danger Response (CDR) research (2014–2025).

**Live site:** https://iamflipse.github.io/cells-turning-off-wiki/  
**Companion wiki (Part 3 — Systemic Treatments & Health Cycle):** https://iamflipse.github.io/cell-danger-response-wiki/

## Layout

- `src/` — markdown pages (`index.md`, `about.md`, `concepts/`, `reference/`)
- `book/` — generated static `mdbook` output (built locally; published via `gh-pages` branch)
- `tools/mdbook` — local `mdbook` binary (ignored in git)

## Rebuild & Republish

```sh
./tools/mdbook build -d book
git add -A && git commit -m "update" && git push origin main
```

To republish the static site to GitHub Pages, copy `book/*` plus `.nojekyll` into an orphan `gh-pages` branch commit and force-push to `origin gh-pages`.
