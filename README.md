# Oilizodiac

A lightweight static web app that pairs Western and Chinese zodiac signs to recommend a Peloponnesian extra virgin olive oil variety with playful Finnish descriptions.

## Features
- Horoscope pairing: Western × Chinese → curated olive oil variety
- Playful Finnish descriptions for every pairing
- Social sharing (Facebook, X/Twitter, Bluesky, LinkedIn)
  - Share text includes variety and clipped description
  - Open Graph/Twitter image: /assets/images/og_image.png
- Favicon set and header logo linking to https://oilishop.fi/
- Firebase Hosting deployment

## Project Structure
- index.html — Single-page app (HTML, CSS, JS)
- assets/
  - images/ — Logo, OG image
  - favicon/ — Favicon assets

## Local Development
This is a static site. You can:
- Open index.html directly in a browser, or
- Serve with a simple HTTP server (recommended for share links and relative paths):
  - Python 3: `python3 -m http.server 8080`
  - Node: `npx serve .`

Then open http://localhost:8080

## Deployment (Firebase Hosting)
Prereqs:
- Firebase CLI installed and logged in
- Project set to `oilizodiac`

Deploy:
```
firebase deploy --only hosting
```

## Analytics
Firebase Analytics is loaded via CDN ESM and enabled if supported by the browser.

## Social Metadata
Open Graph and Twitter tags are set in the <head> with `og_image.png`.

## License
MIT
