# Wedding Invitation

A single-page wedding invitation. Visitors see a closed envelope first; tapping
the wax seal opens the flap and reveals the invitation (Save the Date,
Schedule, and Thank You).

## Edit the content

Open `index.html`, find the `CONFIG` object near the bottom (inside the
`<script>` tag, marked `EDIT ME`), and change:

- `names`, `kicker`, `heroLede`
- `dateNumerals`, `dateWords`, `dateSub`
- `schedule` — add/remove/edit the list of events
- `thankYouMessage`, `thankYouSignature`
- `footerNote` (e.g. your contact email)

Save the file — no build step, no dependencies.

## Deploy to GitHub Pages

1. Create a new repository on GitHub (public), e.g. `our-wedding`.
2. Add this `index.html` (and this README, optional) to the repo root:
   ```bash
   git init
   git add index.html
   git commit -m "Add wedding invitation"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. On GitHub, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to "Deploy from a branch",
   choose branch `main` and folder `/ (root)`, then **Save**.
5. GitHub will publish it at:
   `https://<your-username>.github.io/<repo-name>/`
   (takes a minute or two the first time).

That's it — share that link with your guests.
