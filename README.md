# CellLab — Interactive Animal Cell Explorer

A standalone interactive animal cell explorer based on an original glossy 3D cell illustration. Explore organelles, switch biological activity modes, adjust animation speed and zoom, and take a guided tour.

## Quick start

Open `index.html` in Chrome, Edge, Firefox, or Safari. No server, package manager, API key, or build step is required.

## Publish on GitHub Pages

1. Create a public GitHub repository named `animal-cell-explorer`.
2. Upload **the extracted files** in this folder to the repository root. `index.html` must be at the top level of the repository (not inside the ZIP or a nested folder).
3. Open the repository **Settings → Pages**.
4. Select **Deploy from a branch** as the source, then choose **main** and **/(root)**; save.
5. GitHub Pages will publish at `https://YOUR_USERNAME.github.io/animal-cell-explorer/` (replace YOUR_USERNAME). Publication may take several minutes.

GitHub Pages site publishing is public. Check the repository's visibility, images, and other assets before deploying.

## Files

- `index.html` — complete interactive site with the rendered cell image embedded (no external dependencies).
- `nucleus.html` — interactive nucleus lesson with five structures, process views, labels, and a guided lesson.
- `nucleus/index.html` — `/nucleus/` entry link that forwards to the lesson; `/nucleus.html` remains the canonical page.
- `assets/nucleus-model.png` and `assets/nucleus-labeled.png` — nucleus lesson illustrations.
- `assets/reference-cell.png` — source illustration for future editing.
- `assets/animation-preview.mp4` — 8-second preview video.
- `.nojekyll` — disables Jekyll processing on branch-based GitHub Pages deployments.

## Nucleus lesson

Click the nucleus in the main cell view or choose **Explore inside the nucleus** to open the child lesson. Use the breadcrumb or **Back to the animal cell** to return. Both `nucleus.html` and the `/nucleus/` entry work under the GitHub Pages project path.

Select any of five structures, choose a biological process, or follow the guided lesson. Labels and animation can be toggled independently. Reduced-motion preferences start animations paused. Escape closes an expanded explanation first; press it again to return to the whole cell.

Before publishing, serve the repository with a local static server and check the parent-to-lesson navigation, both entry URLs, images, structure controls, process modes, and return navigation at desktop and mobile widths.

## Updating

Edit `index.html`, commit, and push to `main`. GitHub Pages republishes after the push.

## Technical note

This is an interactive, image-based 2.5D visualization with simulated biological processes, not an independently rigged 3D cell or a quantitative biological model.
