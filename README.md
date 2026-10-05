# Pixel Weather — website

Static site: landing page, privacy policy, terms & conditions. No build step — drag this
whole folder into a GitHub repo and enable **GitHub Pages** (repo Settings → Pages → Deploy
from branch → `main` / root).

- `index.html` — landing page. The hero animation is the *real* pixel-art renderer
  (inlined in `index.html`), ported line-for-line from the app's own Swift code — same
  palettes, same drawing logic, same dither transition. It's not a video or GIF.
- `privacy.html`, `terms.html` — same content as `PRIVACY_POLICY.md` in the Xcode project,
  themed to match. Use the Privacy Policy URL (your GitHub Pages `privacy.html` link) in
  App Store Connect's App Privacy section.
- `assets/app-icon.png` — copied from the app's real icon; update it here if you regenerate
  the icon in Xcode.

## Before you publish

- The "Join the Beta" / "Request TestFlight Access" buttons currently open an email to
  `support.projectz@gmail.com`. Once you enable *external* TestFlight testing and get a
  public link (App Store Connect → your app → TestFlight → Public Link), swap those
  `mailto:` hrefs in `index.html` for that link instead.
- The eyebrow badge says "LIVE ON TESTFLIGHT SOON" — update or remove once you have a
  public link to point to.
- Copyright year / "Last updated" dates are set to 2026 — bump them whenever you actually
  update the pages.
