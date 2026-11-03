# Tilt & Tone

A browser-based interactive sound instrument. The project is packaged as a static website and can be hosted directly with GitHub Pages.

## Run locally

Open `index.html` in a modern browser (Chrome, Edge, Safari, or Firefox). For the most reliable audio and recording behaviour, run it through a local web server rather than opening the file directly.

A simple option with Python installed:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish with GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`, `README.md`, and `.nojekyll` from this folder to the repository's root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. Wait for GitHub Pages to publish the site. The URL will appear in the Pages section.

## Notes

- The app is self-contained: its HTML, CSS, JavaScript, and embedded logo are all inside `index.html`.
- Audio starts after the first user interaction because browsers restrict autoplay.
- Use HTTPS (GitHub Pages provides it) for browser media features. Microphone permission may be required only if you later add microphone input; the current instrument generates its sound in the browser.
