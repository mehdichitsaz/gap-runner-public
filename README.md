# Gap Runner public site

The public website for **Gap Runner: Space Arcade** (iOS): the home page, Support and the Privacy Policy that the App Store listing links to.

## Live pages

- Home: https://mehdichitsaz.com/gap-runner/
- Support: https://mehdichitsaz.com/gap-runner/support.html
- Privacy Policy: https://mehdichitsaz.com/gap-runner/privacy.html

mehdichitsaz.com serves this repository's GitHub Pages site (https://mehdichitsaz.github.io/gap-runner-public/) under `/gap-runner/`, so every path in the pages is relative. `support/` and `privacy/` only redirect to the `.html` pages.

## Structure

```text
.
├── index.html          # Home: how to play, modes, stars and hearts, unlocks, iPhone Duo, updates, FAQ
├── support.html        # Support (App Store Support URL)
├── privacy.html        # Privacy Policy (App Store Privacy Policy URL)
├── support/, privacy/  # Redirects to the pages above
├── assets/site.css     # Shared styles for all pages
├── assets/img/         # Screenshots, header art, icons, social card (WebP/PNG/JPG)
├── apple-touch-icon.png
├── favicon.ico
└── app-ads.txt         # AdMob app-ads.txt, keep as is
```

## Maintenance

- Contact email on every page: `info@mehdichitsaz.com`.
- Keep `support.html` and `privacy.html` stable: the App Store listing links to them.
- The App Store link is `https://apps.apple.com/app/id6761074765` (works in every country).
- Screenshots are 640 px wide WebP from the iPhone 17 simulator; the iPhone Duo shots come from the App Store Connect Duo set; the header art is the App Store product page header.
- No build step and no frameworks: plain HTML and one stylesheet.

## Local preview

```bash
python3 -m http.server 8080
```

Then open http://localhost:8080/.
