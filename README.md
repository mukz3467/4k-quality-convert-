# 4K Quality Convert

A mobile-friendly, browser-based AI image upscaler and format converter.

## What it does
- Uses ONNX Runtime Web with a Real-ESRGAN general-purpose 4× super-resolution ONNX model hosted on Hugging Face.
- Runs image inference in the browser; the selected photo itself is not uploaded to a processing server.
- Upscales supported JPG, PNG, and WebP images, then resamples to the selected output dimensions, including standard 4K UHD (3840 × 2160) where the source aspect ratio permits.
- Lets users preview the original and result, choose an export format (JPG, PNG, or WebP), and download the result.
- Includes input-size checks and output-memory limits for browser safety.

## Model and limitations
The AI model is downloaded from the public model host on first use, so a working internet connection is required. AI upscaling can estimate plausible detail, but it cannot guarantee recovery of the exact detail missing from the original. Processing speed and maximum practical image size depend on the user's device and browser memory.

## Run locally
No build step is required. Open `index.html` in a modern browser or serve the repository using any static file server. Model loading requires internet access.

## Deploy
The project is a static HTML site and can be deployed on Vercel or GitHub Pages. Commit changes to the configured production branch to trigger a deployment when repository integration is enabled.

## License
MIT
