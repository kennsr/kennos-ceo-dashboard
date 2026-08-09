# KennOS CEO Dashboard

A static site. `index.html` fetches `data.json` at load time and renders
the dashboard — to update any figure, edit `data.json` and push. No build
step, no database.

## Deploy on Netlify (Git-based)
1. Push this repo to GitHub (or GitLab/Bitbucket).
2. In Netlify: **Add new site → Import an existing project** → pick this repo.
3. Build command: leave blank. Publish directory: `.` (already set in netlify.toml).
4. Deploy. Every future `git push` auto-redeploys — no rebuild needed since it's plain static files.

## Updating data
Edit `data.json`, commit, push. That's it — index.html has no hardcoded numbers.
