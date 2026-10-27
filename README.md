# 4K Quality Convert

A lightweight, mobile-friendly image resizer and format converter. It runs entirely in the browser and does not upload selected images to a server.

## Features
- Resize an image toward a 3840-pixel long edge (4K target), or choose 2× / 4× dimensions.
- Convert between JPG, PNG, and WebP.
- Preview the original and converted image.
- Download the result.
- Responsive layout and basic SEO metadata.
- Client-side validation for image types, file size, and very large output dimensions.

## Run locally
No build step is required. Open `index.html` in a modern browser, or serve the repository with any static file server.

## Publish with GitHub Pages
1. Open this repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch `main` and folder `/(root)`, then save.
4. Wait for the Pages deployment to finish and use the **Visit site** link.

See the [official GitHub Pages guide](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).

## Important limitation
This tool uses browser canvas interpolation. It enlarges/resizes pixels but does not use AI to reconstruct missing image detail. Output dimensions are capped at 40 megapixels to reduce the risk of browser memory issues.

## License
MIT
