# Jesse Prime Portfolio Update

This package contains only the files changed for the September 2026 portfolio update. It adds Experience, Education, Publications and Manuscripts, and Awards and Honors sections to the homepage. It also adds a Background navigation link and refreshes the two corrected CVT diagram URLs.

## Apply the update

1. Extract this ZIP on your computer.
2. Open your local clone of the `jessebeprime.github.io` repository.
3. Copy `index.html`, `README.md`, `assets`, and `projects` from this package into the repository root. Allow the matching files to be replaced.
4. Confirm that the corrected diagrams exist at these exact, case-sensitive paths:
   - `assets/images/cvt/mechatronics-architecture.webp`
   - `assets/images/cvt/ratio-control-loop.webp`
5. Commit the changes and push them to the `main` branch.
6. In GitHub, open the repository's Actions tab and wait for the Pages deployment to finish successfully.
7. Open the live CVT page in a private window or perform a hard refresh.

## If the corrected diagrams have different names

GitHub Pages will not substitute a newly uploaded image automatically. The `src` value in `projects/cvt.html` must match the committed filename, extension, capitalization, and folder exactly.

The simplest fix is to replace the old files using the two paths above. If the corrected files are PNG or JPG files, either export them as WebP with those names or change the two `src` paths in `projects/cvt.html` to match the files you committed. Keep the `?v=20260922` suffix; it forces browsers to request a fresh copy after deployment.

Do not upload the ZIP itself to the repository. Extract it and copy its contents into the repository structure.
