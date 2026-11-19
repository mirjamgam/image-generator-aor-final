# Art of Research 2026 · LinkedIn image generator

A small web page where participants make an "I'm attending / presenting / volunteering at Art of Research 2026" image for LinkedIn.

- Upload a photo, drag and zoom it into the circle
- Add name, organisation or role, and an optional own line (for example "See you there!")
- Choose square (1200 × 1200) or landscape (1200 × 627)
- Download the PNG and copy the suggested post text

Photos are processed in the visitor's own browser and are not uploaded anywhere.

## Files

```
index.html            the page
css/style.css         styles
js/app.js             image drawing, photo upload and download
assets/aor-logo.png   Art of Research 2026 logo (white)
assets/aalto-logo.png Aalto University logo (white)
assets/voices-banner.jpg  Voices banner (the VOICES wordmark is cut from it)
```

## Publish with GitHub Pages

1. Create a new repository and upload all the files, keeping the folders.
2. In the repository, go to Settings → Pages.
3. Under "Build and deployment", choose "Deploy from a branch", select `main` and `/ (root)`, and save.
4. After a minute the page is live at `https://<your-username>.github.io/<repository-name>/`.

## Test locally

Open the page through a local web server rather than by double-clicking `index.html`. Some browsers block saving the image from a file opened directly from disk.

```
python3 -m http.server
```

Then open http://localhost:8000.

## Change the event details

The date, place, labels and post texts are at the top of `js/app.js` (`DATE`, `PLACE`, `LABEL`, `POST`). Colours are in `C` in the same file and as CSS variables at the top of `css/style.css`.
