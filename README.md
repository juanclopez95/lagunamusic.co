# lagunamusic.co

The source for Laguna's public artist website.

## Deployment

GitHub Pages deploys the site automatically whenever a change is merged into `main`. The production domain is not switched until the GitHub preview is approved.

## Editing workflow

1. Juan asks Muse for a website change over WhatsApp.
2. Muse returns a structured change request using `MUSE_SITE_CHANGE_TEMPLATE.md`.
3. Codex creates a branch and pull request with the requested copy or asset changes.
4. Juan reviews the preview/diff and approves the pull request.
5. Merging to `main` deploys the update automatically.

Nothing publishes directly from WhatsApp, and Muse never needs DNS or GitHub administrator credentials.

## Local preview

```bash
cd "/Users/juanlopez/Desktop/Laguna Content Pipeline/01_PROJECTS/2026-10-18_lagunamusic-co_Website"
python3 -m http.server 4173
```

Open `http://localhost:4173`.

## Important files

- `index.html` — public site and copy
- `assets/` — optimized release artwork and Laguna lockup
- `content/WEBCOPY_lagunamusic-co_v3.txt` — approved copy reference
- `MUSE_SITE_CHANGE_TEMPLATE.md` — phone-to-GitHub handoff format
- `LAUNCH_CHECKLIST.md` — production cutover plan

