# Trustworthy Tool-Using & Skill-Based AI Agents — Workshop Website

Static site for the proposed **NeurIPS 2026 workshop** on the security, privacy,
evaluation, and deployment of tool-using and skill-based AI agents.

It is a single self-contained `index.html` (no build step, no dependencies).
`.nojekyll` tells GitHub Pages to serve the files as-is.

## Local preview

Open `index.html` in a browser, or:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a new GitHub repo (e.g. `trustworthy-agents-26`).
2. Push this folder:
   ```bash
   git remote add origin git@github.com:<owner>/trustworthy-agents-26.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Build and deployment**, set
   **Source = Deploy from a branch**, **Branch = `main` / `(root)`**, Save.
4. The site goes live at `https://<owner>.github.io/trustworthy-agents-26/`
   within a minute or two.

For a clean root URL like `https://<name>.github.io/`, name the repo
`<name>.github.io` instead.

## Editing

All content and styling live in `index.html`. To update speakers, dates, or
topics, edit the relevant `<section>`. The submission button is marked
`data-submit` — point its `href` at the OpenReview link once it exists.

## Status / TODO

- Dates are **tentative**, pending workshop acceptance.
- Speaker statuses: Yang Xiang, Ming Ding = confirmed; David Lo, Shuai Wang = invited (pending).
- Add the OpenReview submission URL when the call opens.
- Optional: add a custom domain via a `CNAME` file.
