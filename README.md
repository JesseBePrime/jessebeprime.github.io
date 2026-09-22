# Jesse Prime Robotics Design Portfolio

This repository contains the source files for https://jessebeprime.github.io.

The website is a static GitHub Pages site. It uses ordinary HTML and CSS, so there is no build command, package manager, or database.

## Repository structure

- index.html: Homepage and project overview
- projects/: Individual project case studies
  - cvt.html
  - ankle-exoskeleton.html
  - power-board.html
  - arm-swing-exosuit.html
- assets/css/styles.css: Shared visual styling and responsive layout
- assets/images/: Optimized portfolio images grouped by project
- 404.html: Page shown for an invalid address
- robots.txt and sitemap.xml: Search-engine files
- .nojekyll: Tells GitHub Pages to serve the files directly

Keep the folder names and file locations unchanged when uploading the site. The HTML files use those paths to locate the stylesheet and images.

## Publish through the GitHub website

1. Open the jessebeprime.github.io repository.
2. Choose Add file, then Upload files.
3. Upload the contents of this repository package, preserving the folders.
4. Commit the upload to the main branch.
5. Open Settings, then Pages.
6. Under Build and deployment, select Deploy from a branch.
7. Choose the main branch and the root folder, then save.
8. Visit https://jessebeprime.github.io after the deployment finishes.

GitHub's browser uploader may be inconvenient for nested folders. GitHub Desktop is usually easier:

1. Clone the jessebeprime.github.io repository in GitHub Desktop.
2. Copy all files from this package into the cloned repository folder.
3. Return to GitHub Desktop and review the changed files.
4. Commit with a message such as "Create portfolio website."
5. Select Push origin.

## Preview locally

From the repository folder, start a local web server:

    python -m http.server 8000

Then open http://localhost:8000 in a browser. Opening index.html directly may not load root-relative links correctly, so use the local server when previewing.

## Updating content

- Edit homepage text in index.html.
- Edit each project in its matching file under projects/.
- Replace an image with another file using the same name to update it without changing the HTML.
- If an image filename changes, update the matching src path in the HTML.
- Shared colors, spacing, and responsive behavior are defined in assets/css/styles.css.

### Replacing the CVT diagrams

The CVT page expects the corrected diagrams at these exact, case-sensitive paths:

- assets/images/cvt/mechatronics-architecture.webp
- assets/images/cvt/ratio-control-loop.webp

Replace the existing files at those paths rather than adding differently named images. If the corrected images are PNG or JPG files, export them as WebP or update both matching `src` values in `projects/cvt.html`. The image URLs include a version query so browsers request the new files after deployment.

## Review before public release

- Confirm that the lab permits publication of unpublished research details and CAD images.
- Confirm permission for every identifiable person shown in a photograph.
- Add approved quantitative test results where they strengthen a project.
- Check every page on both a desktop and a phone.
- Keep private data, unpublished source files, raw participant data, and credentials out of the repository.

No reuse license is included. The portfolio text and visual assets remain the property of their respective owners.
