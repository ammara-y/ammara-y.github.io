# Setup

Edit before publishing:
- `index.html` — email (`mailto:you@example.com`), github/twitter/scholar links (`#` placeholders), publication links, surname if you want one in the `<title>` / hero.

# Deploy on GitHub Pages (free)

1. Create a new repo on GitHub — name it `yourusername.github.io` if you want it at the root domain, or anything else for a project page.
2. Push these three files (`index.html`, `style.css`, `script.js`) to the repo root:
   ```
   git init
   git add .
   git commit -m "site"
   git branch -M main
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git push -u origin main
   ```
3. Repo → **Settings → Pages** → under "Build and deployment", set Source to **Deploy from a branch**, branch `main`, folder `/ (root)** → Save.
4. Live in ~1 min at `https://yourusername.github.io` (or `https://yourusername.github.io/repo-name` for a project repo).

Custom domain: add a `CNAME` file with your domain, point DNS at GitHub's IPs, set it in Settings → Pages.
