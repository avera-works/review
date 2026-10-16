# AVERA Review Studio

A simple Arabic RTL review page that creates a shareable AVERA-branded PNG card in the browser.

## Features
- Arabic responsive form
- Star rating
- Generates a 1080x1350 PNG card locally in the browser
- Download PNG
- Uses native device sharing when supported
- Opens WhatsApp with a prefilled review summary

## GitHub Pages setup
1. Create a new GitHub repository, e.g. `avera-review-studio`.
2. Upload `index.html` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then Save.
6. Wait for GitHub Pages to publish the site.

## Configure WhatsApp
In `index.html`, find:
`const AVERA_WHATSAPP_NUMBER = "9665XXXXXXXX";`
Replace it with the AVERA WhatsApp number in international format, digits only (no `+`, spaces, or dashes).

## Important limitations
- This static GitHub Pages version does not store reviews in a database.
- It cannot automatically send an image to WhatsApp. It opens WhatsApp with review text; attach the downloaded PNG manually.
- Automatic image delivery and persistent review storage require a secure backend/database and the official WhatsApp Business Platform or an approved provider. Keep API tokens on the server, never in `index.html`.
- Publish customer reviews only with appropriate permission. Name is optional.
