# One-time GitHub setup

This file is a checklist for you (the repo owner) to run through once, right after pushing this folder to a new GitHub repository. Delete it afterward if you like — it isn't part of the plugin or its docs.

1. **Create the repository.**
   On GitHub: **New repository** → set visibility to **Public** → do **not** initialize with a README/license/gitignore (this folder already has a README and gitignore) → create.

   **Note:** this folder deliberately contains no plugin source code and no LICENSE file — it's a documentation/community hub for a commercial plugin, not an open-source release. Don't add the plugin's actual source to this repo.

2. **Push this folder.**
   ```
   cd github-project
   git init
   git add .
   git commit -m "Initial public release"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```

3. **Enable Discussions.**
   Repo → **Settings → General → Features → Discussions** → check the box.

4. **Set up the Discussion categories.**
   Go to the **Discussions** tab → **New discussion** → **New category**, and create three categories matching the templates already included under `.github/DISCUSSION_TEMPLATE/`:
   - **Ideas** (format: Open discussion) — feature/skin suggestions
   - **Q&A** (format: Question / Answer) — installation help, troubleshooting
   - **Show and tell** (format: Open discussion) — screenshots, setups

   GitHub auto-loads a matching `.yml` template from `.github/DISCUSSION_TEMPLATE/` once a category with the same name exists, so the forms in this repo (with the fields already written) will show up automatically.

5. **Optional: repo description and topics.**
   Add a short description (e.g. "Now Playing media panel for Stream Deck +") and topics like `streamdeck`, `elgato`, `plugin` in the repo's **About** panel — helps discovery.

6. **Link back to the store listing.**
   Add the plugin's Elgato Marketplace URL to the README's intro line and the repo's **About** panel, once you have it — right now the README just says "available through the Elgato Marketplace" without a link.
