Publishing the Privacy Policy via GitHub Pages
=============================================

Files added:

- `docs/privacy-policy.md` — the privacy policy Markdown document.
- `docs/.nojekyll` — disables Jekyll processing.
- `.github/workflows/deploy-pages.yml` — GitHub Actions workflow to publish `docs/` to the `gh-pages` branch.

What happens next
------------------

1. When you push these changes to the `main` branch, the workflow `Deploy docs to GitHub Pages` will run and publish the `docs/` folder to the `gh-pages` branch.
2. Once the workflow completes, your site should be available at:

   `https://<github-username>.github.io/<repository>/`

   Replace `<github-username>` with the repository owner (e.g., `Konayuma`) and `<repository>` with `roominateprivacypolicy`.

Notes and manual steps
----------------------

- If GitHub Pages does not automatically serve the `gh-pages` branch, go to the repository's **Settings → Pages** and ensure the Source is set to the `gh-pages` branch.
- You can also choose to serve Pages directly from the `docs/` folder on `main` via repository Settings → Pages. If you prefer that approach, the workflow can be removed.
- It may take a minute or two after deployment for the site to become available.

If you want a custom domain, add a `CNAME` file under `docs/` or configure the Pages settings.
