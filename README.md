# Portfolio

My personal portfolio website.

## Open in Cursor

Double-click **`portfolio.code-workspace`** in this folder, or choose **File → Open Workspace from File…** and select that file. The workspace opens **portfolio** together with **TH - Academy** and **DaGlowApp** in the sidebar.

## Development

Run locally on port 7003:

```bash
python3 -m http.server 7003
```

Then visit: http://localhost:7003

## GitHub Pages

The site deploys via **GitHub Actions** (`.github/workflows/pages.yml`) on every push to `main`.

- In the repo **Settings → Pages → Build and deployment**, set **Source** to **GitHub Actions** (not “Deploy from a branch”).
- Private repos need a **paid GitHub plan** for Pages, or make the repo **public**.
- Root includes **`.nojekyll`** so static files are served as-is (no Jekyll).

After `git push`, check **Actions** for the latest run.

## Git remote

Use HTTPS without embedding tokens in `.git/config`. Authenticate with **GitHub CLI** (`gh auth login`) or macOS Keychain when you push.

