# Copilot Instructions

- **Project type**: Static personal site (plain HTML + shared `style.css`). No build, bundle, or runtime dependencies.
- **Entry points**: `index.html` (home), `projects.html`, `fun.html`; shared assets `style.css`, `photo.webp`, `Siddharth_Narsipur_Resume.pdf`.
- **Styling**: All pages import `style.css`, which defines the container layout, typography, link hover states, and mobile breakpoint at 768px. Reuse existing classes (`container`, `content`, `experience`, `experience-header`, `bullet`, `back-link`, `links`) to stay consistent and mobile-friendly.
- **Layout pattern**: Pages generally wrap content inside `.container > .content`, with optional `.profile-img` on the home page and a `back-link` at the top of secondary pages.
- **Links**: Use relative links between local pages (e.g., `projects.html`, `fun.html`). External links open in the same tab; keep them as plain anchors. Maintain existing link text styles (no buttons).
- **New pages**: Start from the structure in `projects.html`/`fun.html`: include the shared stylesheet, add a `back-link` to `index.html`, then content grouped in `.experience` blocks with `.experience-header` and `.bullet` for short descriptions.
- **Content tone**: Concise, resume-like bullet phrasing. Keep page titles in the `<title>` tag and `<h1>` aligned (e.g., "Projects - Siddharth Narsipur").
- **Assets**: Place new images at root or a simple folder and reference with relative paths. Keep `alt` text meaningful. Prefer WEBP for photos when practical.
- **Accessibility**: Preserve heading order, provide `alt` on images, and ensure link text is descriptive (not "click here").
- **Responsiveness**: Avoid adding fixed widths; lean on existing flex layout and media query in `style.css` to keep pages readable on mobile.
- **Testing**: No automated tests; open HTML files in a browser to verify layout and links. Ensure new pages load without console errors.
- **Deploy assumption**: Site likely served from the repo root (e.g., GitHub Pages). Avoid absolute root paths; use relative paths to keep links working locally and on Pages.
