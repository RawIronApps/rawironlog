# RawIron Log

Static support/legal pages for RawIron Log, published as part of the RawManor website (see `../README.md`).

## Files

- `index.html` — public landing page, in the graphite product theme (`body.theme-graphite`, matching the app's dark mode)
- `privacy.html` — privacy policy
- `terms.html` — terms of use
- `support.html` — support/contact page
- `tips.html` — Tips & Features: what the app can do and where to find it; mirrors the app's Tips & Features page (`Pages/TipsPage.xaml.cs`), so update both together; also in the graphite product theme. Privacy, Terms and Support stay on the RawManor paper theme for long-form reading
- `styles.css` — shared styling: the RawManor palette plus the graphite product theme and steel phone frames (`.device`)
- `images/` — logo assets generated from `rawironlog-app-logo.png` (cropped to the artwork, then resized)
  - `logo-72.png` — header mark (shown at 36px, 30px on mobile)
  - `logo-144.png` — featured-app logo on the RawManor home page (shown at 96–120px)
  - `logo-480.png` — large logo (no longer shown in the hero, which now shows app screenshots)
  - `favicon-32.png` — browser tab icon
  - `apple-touch-icon.png` — 180×180 iOS home-screen icon, flattened onto the page background
  - `screens/` — app screenshots for the hero phone frames (iPhone 15 Pro simulator, 9:41 status bar, resized to 589×1278 JPEG). Currently the Welcome screen in light and dark mode; replace or add screens (Workouts, Sets, History) captured from a device with real data.

## Before publishing

1. Review the Privacy Policy against the final production build and App Store / Google Play privacy disclosures.
2. Review the Terms of Use for the final publisher identity (RawManor) and jurisdiction. The terms are a practical draft, not legal advice.
3. Verify the support instructions against the production build and the current store configuration.
4. When the store listings are live, replace the two "Coming soon" spans in the `index.html` hero with links to the App Store and Google Play listings (see the HTML comment there).
5. Once the site's public URL is known, add an absolute `og:image` meta tag to each page so link previews show the logo.
6. Replace the Welcome-screen screenshots in `images/screens/` with screens showing real workouts.
7. Publish with the rest of the RawManor site (see `../README.md`).
