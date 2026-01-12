# Repository Overview: Simone Rotondi's Personal Website

## 1. The Point of this Repo
This repository hosts the source code for the personal website of **Simone Rotondi**, a PhD researcher at INRIA specializing in robotics, control, and soft manipulation. 

**Primary Goals:**
-   **Portfolio:** Showcase academic work and research projects (Soft Manipulation, GNSS/RTK, Robotics Utilities).
-   **Professional Presence:** Provide a biography ("About"), current status ("Now"), and contact information.
-   **Community Hub:** Host the "BrainJuice" section, a space for discussions on artificial and human intelligence (`brainjuice.html`).

**Technical Approach:**
-   **Static Site:** Hosted on GitHub Pages.
-   **Simplicity:** Pure HTML/CSS with minimal Vanilla JS (no complex build chain).
-   **Accessibility & UX:** Responsive design, dark/light mode support, and semantic HTML.

## 2. Structure
The repository is organized for simplicity and ease of maintenance.

### Core Files
-   `index.html`: **Main Landing Page**. Contains the Hero section, About, Selected Work, Now page, and Contact form.
-   `projects.html`: **Detailed Projects**. Expanded descriptions of research work (e.g., Soft Manipulation experiments, RTK navigation).
-   `brainjuice.html`: **Community Page**. Overview of the BrainJuiceClub, including topics, formats, and notes/links.
-   `_config.yml`: **GitHub Pages Config**. Sets the site title, description, and Jekyll theme (currently `jekyll-theme-minimal`, mainly for metadata defaults).

### Assets (`/assets`)
-   `css/styles.css`: **Global Styles**. Handles layout, typography, and theming. 
    -   *Key:* The `:root` selector defines CSS variables (colors, fonts) for easy theming (e.g., `--accent` color).
-   `img/`: **Images**. Stores static assets like profile photos (`simone_sapienza.jpeg`), logos (`logo.ico`), and placeholders.

## 3. Development & Maintenance
Since this is a static site, no build process is strictly required for local development.

### How to Run
-   **Simple Server:** Run `python3 -m http.server 8000` in the root directory and visit `http://localhost:8000`.
-   **Deployment:** Changes pushed to the `main` branch are automatically deployed by GitHub Pages.

### Customization Guide
-   **Content Updates:** Edit the HTML files directly. Look for comment markers or clear section tags (`<section id="now">`).
-   **Styling:** Modify `assets/css/styles.css`. 
    -   *Theme:* Dark/Light mode logic is handled in the inline `<script>` at the bottom of each HTML page and persists via `localStorage`.
-   **Contact Form:** The form in `index.html` points to a Formspree endpoint. Update the `action` URL if the endpoint changes.

## 4. Guidelines for AI Agents & Contributors
-   **Code Style:** Maintain the existing indentation (2 spaces) and semantic HTML structure.
-   **CSS:** Use existing utility classes where possible (e.g., `.card`, `.btn`, `.section`) to maintain visual consistency.
-   **Navigation:** If adding a new page, ensure it is linked in the `<nav>` section of `index.html` and the specific page's header.