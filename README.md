# Dilun Panduka — Portfolio

A single-page portfolio site built from your résumé, styled as a live systems dashboard: your career shows up as a versioned changelog (v0.1.0 → v4.0.0), your skills as a config file, and your projects as deployed services.

## Files
- `index.html` — the whole site (HTML/CSS/JS, no build step, no dependencies to install)
- `resume.pdf` — your résumé, linked from the "Download résumé" buttons

## Deploy to GitHub Pages (free)

1. Create a new **public** repository on GitHub — name it anything, e.g. `portfolio`.
   (If you want it at `https://<username>.github.io` directly with no sub-path, name the repo exactly `<your-github-username>.github.io` instead.)
2. Upload `index.html` and `resume.pdf` to the repo (drag-and-drop on the GitHub web UI works fine, or use git — see below).
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
6. Wait 1–2 minutes. Your site will be live at:
   - `https://<your-github-username>.github.io/<repo-name>/` (normal repo), or
   - `https://<your-github-username>.github.io/` (if you named the repo `<username>.github.io`)

### Using git from the command line instead
```bash
git init
git add index.html resume.pdf
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```
Then do steps 3–6 above.

## Notes
- I left the two references off the public page on purpose — publishing someone else's personal phone number and email on a page anyone can scrape isn't great for them. Happy to add a "references available on request" line, or a private version, if you want.
- To update content later, edit the text directly inside `index.html` (it's plain HTML — search for the text you want to change) and push again; Pages redeploys automatically within a minute or two.
- Want a custom domain later (e.g. `dilunpanduka.dev`)? GitHub Pages supports that too, under Settings → Pages → Custom domain.
