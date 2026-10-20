# AEGIS website (GlobalFive)

A single static page. No build step, no server code. Open `index.html` in a browser to preview it.

## Files
- `index.html` contains the whole site: content, styles and the interactive digital twin.
- `favicon.svg` is the browser tab icon.

Fonts load from Google Fonts. Without internet the page still works, using system fonts.

## Deploy (pick one)

**Netlify Drop (fastest, no account setup):** go to https://app.netlify.com/drop and drag this folder onto the page. You get a live link in seconds.

**GitHub Pages:** create a repository, upload both files to the root, then go to Settings → Pages → Deploy from branch → `main` / root. The site appears at `https://<username>.github.io/<repo>/`.

**Vercel:** run `npx vercel` inside this folder, or import the GitHub repository at vercel.com. Choose "Other" as the framework, with no build command.

## Editing
- Text is plain HTML. Search for a phrase and edit it in place.
- Colours are defined once at the top of the `<style>` block (`--teal`, `--amber`, and so on), with separate dark-mode values below them.
- Simulation settings are at the start of the `<script>` block: `LIMIT` (safe temperature), `MARGIN`, the CO2 factor `EF` and household use `FLAT_MONTH`.
- The demo numbers come from a simplified model and are illustrations, not measured results.
