# Repository Guidelines

## Project Structure & Module Organization
- `index.html` – home/landing with hero, about, selected work, now, and contact.
- `projects.html` – detailed project writeups and links.
- `brainjuice.html` – BrainJuice overview and notes placeholders.
- `assets/css/styles.css` – shared styling; accent color lives in `:root --accent`.
- `assets/img/` – add your own images (e.g., `profile.jpg`, OG/thumb assets).
- `_config.yml` – GitHub Pages/Jekyll config (minimal theme, title/description).

## Build, Test, and Development Commands
- Static site; no build step required. Open `index.html` in a browser or use a simple server: `python -m http.server 8000`.
- GitHub Pages deploys from `main` automatically after pushes.

## Coding Style & Naming Conventions
- HTML: semantic sections (`header`, `nav`, `main`, `section`, `article`, `footer`), ordered headings, ARIA labels for toggles.
- CSS: keep variables in `:root`, prefer utility classes already present (cards, grids, buttons). Use 2-space indentation.
- JS: minimal vanilla scripts; keep theme/menu logic unobtrusive and placed at the bottom of the page.
- Paths: keep assets under `assets/` (e.g., `assets/img/<name>.png`).

## Testing Guidelines
- No automated tests yet; for changes, manually verify on mobile and desktop, check dark/light mode, nav toggle, and Formspree placeholder.
- If adding scripts, test in modern browsers and ensure no console errors.

## Commit & Pull Request Guidelines
- Commit messages: short imperative summaries (e.g., “Add project cards”, “Tweak accent color”). Current history uses concise, action-led messages.
- PRs (if opened): include a brief description, screenshots of key sections (light/dark + mobile/desktop) for UI changes, and note any new links/endpoints (e.g., Formspree).

## Security & Configuration Tips
- Replace `simone@example.com` and other placeholder links before publishing.
- Update Formspree `action` URL in `index.html` for the contact form, or remove the form if unused.
- Keep OG image URLs valid; replace `assets/img/placeholder-card.png` with a real asset and adjust meta tags if renamed.
