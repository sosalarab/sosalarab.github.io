# Umar Sosal — Portfolio (GitHub Pages version)

The v3.2 portfolio as a static website for free GitHub Pages hosting.
Same design and content as the full-stack v3.2 — but no database and no admin:
GitHub Pages cannot run PHP. The contact form opens WhatsApp with the
visitor's message pre-written instead of saving to an inbox.

## Deploy (one time)

1. On github.com, create a **New repository**:
   - Name it exactly: `sosalarab.github.io` (your own GitHub username)
   - Set it to **Public**
   - Do NOT tick "Add a README" — this folder already has everything
   - Create repository
2. On the new repo page, click **"uploading an existing file"**.
3. Drag in the **contents of this folder** (`index.html`,
   `umar-portfolio-og-light.png`, `.nojekyll`, `README.md`) — the contents,
   not the folder itself. `index.html` must sit at the top level of the repo.
   (`.nojekyll` is a hidden file — if you can't see it, that's fine, upload
   the rest; it only speeds things up.)
4. Click **Commit changes**.
5. Go to **Settings → Pages**: under "Build and deployment", Source =
   **Deploy from a branch**, Branch = **main**, folder = **/ (root)**. Save.
6. Wait a few minutes, then open `https://sosalarab.github.io`.

## After it is live

- In `index.html`, change the `og:image` line to the full address
  `https://sosalarab.github.io/umar-portfolio-og-light.png` so shared
  links show the designed preview card. (There is a comment in the file
  marking the exact line.)
- Photos and project images are embedded inside `index.html`. To change
  one, the easy route is the full-stack version's admin panel; on this
  static copy, ask Muse to swap the image and re-upload the file.

## The full version

The database version (admin panel, message inbox, email alerts) is the
`umar-portfolio-v3.2-xampp.zip` package — it needs PHP hosting
(XAMPP locally, or a real host when you deploy for clients).
