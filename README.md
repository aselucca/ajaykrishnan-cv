# Ajaykrishnan Selucca Muralidharan · CV Site

A single-page personal CV website for Ajaykrishnan Selucca Muralidharan, highlighting research experience in machine learning-driven railway condition monitoring.

## Local development

Open `index.html` in your browser or use a lightweight web server (for example, `npx serve .`) to preview the page locally.

## Deploying to GitHub Pages

This repository includes an automated GitHub Actions workflow that publishes the site to GitHub Pages.

1. Push the repository to GitHub and ensure the default branch is named `main`.
2. In the GitHub repository, navigate to **Settings → Pages**.
3. Under **Build and deployment**, choose **Source: GitHub Actions**.
4. The `Deploy site to GitHub Pages` workflow will run automatically on every push to `main` (or you can trigger it manually from the **Actions** tab).
5. When the workflow completes, the site will be available at the GitHub Pages URL displayed in the workflow summary.

All static assets (`index.html`, the `images/` directory, and CV files in `cv/`) are published as part of the deployment artifact.
