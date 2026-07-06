# First — Interactive Love Letter (إيتيشري)

An interactive, animated HTML "love letter" web page by Aayush (أيوش). Open the page in a browser to see an animated envelope, a typewriter message, background music, a bouquet animation, and small interactive touches.

## Preview
Open `index.html` in your browser to view the page locally. The page includes audio and animations; some browsers may block autoplay — click "Open Letter" to start the experience.

## What’s included
- `index.html` — the entire interactive page (HTML, CSS, JavaScript).
- Images: `love.png`, `bg.png`, `bouquet.png`, `hand_drawn_bouquet-removebg-preview.png`.
- Small inline audio players load a soft piano track and chime sounds.

## How to run locally
Option 1 — quick (may work for most browsers):
- Double-click `index.html` to open it in your browser.

Option 2 — recommended (serves files from a local web server):
- With Python 3:
  - python3 -m http.server 8000
  - Open http://localhost:8000 in your browser
- Or with Node:
  - npx http-server
  - or npx live-server

Note: Serving over HTTP(S) reduces some autoplay restrictions on certain browsers.

## Customize the message and content
- Main message: edit the `customMessage` string inside `index.html` (JavaScript near the top). Keep newlines as `\n` or paste plain text.
- Signature: edit the signature element inside `index.html` (search for `<p class="signature handwritten">`).
- Title and header text: edit the `<title>` and `<h1 class="handwritten">` in `index.html`.
- Replace images: swap any of the image files in the repo (keep the same filenames referenced in `index.html`), or update the `src` attributes to new filenames.

Be careful when editing: the page mixes inline CSS, SVG, and JavaScript. If you change the filenames, update the references in `index.html`.

## Accessibility & behavior notes
- The page respects `prefers-reduced-motion`: animations and the typewriter effect are reduced where that preference is set.
- Audio playback may be prevented by browser autoplay policies; clicking the "Open Letter" button starts audio and animations.
- If you want the page to be fully accessible, consider adding:
  - ARIA labels where appropriate.
  - A control to mute/stop music.
  - Text-only fallback for screen readers.

## Suggested improvements (ideas)
- Add a small settings panel: toggle music, reduce motion, font size.
- Externalize the message into a separate JSON or markdown file for easier editing.
- Add a `screenshot.png` or animated GIF in the repo for quick previews on GitHub.
- Add a LICENSE file (MIT or other) if you plan to publish the project.

## Contributing
If you want me to:
- Update this README in the repo, say "Please commit README".
- Add a LICENSE, or create a screenshot/preview, tell me which license or which screenshot.

## License
No license specified. Add a `LICENSE` file if you want a specific open-source license (e.g., MIT).

## Contact
Created by Aayush (أيوش). For help or changes, open an issue or reply here.
