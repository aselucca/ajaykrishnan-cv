# cvsite
A personal webpage to share on behalf of CV
# Ajaykrishnan Selucca Muralidharan · CV Site

A single-page personal CV website for Ajaykrishnan Selucca Muralidharan, highlighting research experience in machine learning-driven railway condition monitoring.

## Tech stack
- Static HTML enhanced with [Tailwind CSS](https://tailwindcss.com/) via CDN.
- Minimal vanilla JavaScript for theming, mobile navigation, and utility helpers.
- Lightweight inline SVG illustrations for the profile portrait, organisation logos, and skill icons.

## Key features
- Sticky navigation with smooth scrolling across About, Experience, Projects, Skills, Publications, and Contact sections.
- Light/dark mode toggle with persisted preference.
- Research- and industry-focused project highlights with expandable insight panels.
- Adaptive CV call-to-action that detects whether a PDF is present locally and falls back to a "Request CV" prompt if none is provided.
- Contact form launches the visitor's email client with a prefilled message template.

## Local development
This is a static site—open `index.html` directly in a browser to preview. For a better development workflow you can use a simple HTTP server, for example:

```bash
python -m http.server
```

Then browse to `http://localhost:8000`.

## Customisation notes
- Update the SVG artwork in `images/` if you want to tailor the illustrations to your own branding. Each file is human-readable and can be tweaked in any vector editor or text editor.
- Place your downloadable PDF at `cv/ajaykrishnan_cv.pdf`. The path is git-ignored by default; add it manually when deploying.
- Adjust the contact form JavaScript/mailto address in `index.html` if you prefer a different workflow or service.
- Tailor meta tags in `index.html` for SEO and analytics requirements.

## Image reference guide
The site uses a small set of SVGs so everything stays text-based and version-control friendly:

- `images/profile-portrait.svg` – abstract portrait block that personalises the hero without relying on a raster headshot.
- `images/logo-ltu.svg`, `images/logo-primesoft.svg`, `images/logo-applied-materials.svg` – lightweight institution logos reinforcing the employment timeline.
- `images/icon-python.svg`, `images/icon-pytorch.svg`, `images/icon-gcp.svg` – skill icons supporting the tooling grid.
- `images/og-cover.svg` – open graph preview ensuring shared links render with a descriptive banner.

Project cards intentionally avoid placeholder artwork so you can drop in real screenshots when available without removing existing assets.

## Working with binary assets
- Binary artefacts such as PDFs and raster imagery (PNG/JPG) remain excluded from version control via `.gitignore`. Optimised SVGs in `images/` are tracked for design consistency.
- Keep personal high-resolution assets locally and swap them during deployment if required.
- For pull requests, commit the SVG or textual sources only to simplify reviews and avoid large file quotas.

## Deployment
The site can be deployed to GitHub Pages, Netlify, or any static hosting provider. Upload the repository contents as-is; no build step is required.

## Version control tips
- Local development in this workspace happens on the `work` branch. To publish the latest changes to your remote `dev` branch, push explicitly with:

  ```bash
  git push origin work:dev
  ```

- After pushing once, set the upstream so future pushes only need `git push`:

  ```bash
  git push --set-upstream origin work:dev
  ```

- You can confirm the commit landed remotely with `git log origin/dev -1` or by checking the branch on GitHub.