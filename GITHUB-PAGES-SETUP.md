# GitHub Pages Setup Guide

Your repository is now configured to automatically build and deploy to GitHub Pages. Here's what to do:

## Enable GitHub Pages

1. Go to **Settings** → **Pages** in your GitHub repository
2. Under "Source", select **Deploy from a branch**
3. Set branch to `gh-pages` and folder to `/ (root)`
4. Click **Save**

Your GitBook will be published at: `https://spycrypto.github.io/the-veil-knowledge-base/`

## How It Works

- Every push to `main` triggers the GitHub Actions workflow
- The workflow builds the GitBook and creates a `gh-pages` branch
- GitHub Pages automatically serves the built content

## Local Testing

To preview your GitBook locally before pushing:

```bash
cd ./the-veil-knowledge-base

# Install GitBook
npm install -g gitbook-cli

# Serve locally
gitbook serve

# Open http://localhost:4000 in your browser
```

## Adding Content

1. Create new research, frameworks, or community content in appropriate directories
2. Update `SUMMARY.md` to add chapters to the table of contents
3. Follow guidelines in `STRUCTURE.md`
4. Commit and push to `main`
5. GitHub Actions will automatically rebuild and redeploy

## Troubleshooting

If the build fails:
1. Check the **Actions** tab in your GitHub repository
2. Click the failed workflow run for detailed logs
3. Common issues:
   - Invalid YAML in `book.json` — validate syntax
   - Broken links in `SUMMARY.md` — verify file paths
   - Missing files referenced in TOC — create the files

## What's Included

✅ **Manifesto** — Core vision and principles  
✅ **Directory Structure** — Organized research, frameworks, and community spaces  
✅ **Contribution Guidelines** — STRUCTURE.md with format templates  
✅ **GitHub Pages Deployment** — Automatic CI/CD via Actions  
✅ **Table of Contents** — SUMMARY.md with navigation links  

## Next Steps

1. Enable GitHub Pages (see above)
2. Add sample research or framework content
3. Expand SUMMARY.md as content grows
4. Invite collaborators and start building!

---

Your knowledge base is ready to scale. Start contributing! 🎉
