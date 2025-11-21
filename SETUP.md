# Quick Setup Guide

## Quick Start (TL;DR)

1. **Create GitHub repository** (don't initialize with README)
2. **Run these commands:**

```bash
cd /srv/Alertim

# Add all files
git add .

# Commit
git commit -m "Initial commit: Alertim website"

# Rename branch to main (if needed)
git branch -M main

# Add your GitHub repository (replace with your URL)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git

# Push to GitHub
git push -u origin main
```

3. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Source: Branch `main`, Folder `/ (root)`
   - Save

4. **Your site will be live at:**
   - `https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME`
   - Or `https://YOUR_USERNAME.github.io` if repo is named `YOUR_USERNAME.github.io`

## File Structure

```
Alertim/
├── index.html          ← Entry point (redirects to Home.html)
├── Home.html          ← Home page
├── Projects.html      ← Projects page
├── Contact.html       ← Contact page
├── Home/              ← Home page images
├── Projects/          ← Projects page images
├── Contact/           ← Contact page images
├── README.md          ← Full documentation
└── .gitignore         ← Git ignore rules
```

## Next Steps

- See `README.md` for detailed instructions
- Test locally before pushing: `python3 -m http.server 8000`
- Update content by editing HTML files and pushing changes

