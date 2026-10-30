# VDU — Video Discovery Universe

A free, mobile-friendly video discovery interface. Search uses community-run public Invidious instances (no API key); playback uses the official YouTube embedded player.

## VDU Plus features
- Search by pressing **Enter**; `/` focuses the search field.
- 10-second seek back/forward and playback speed controls.
- YouTube's own player controls quality selection; the official IFrame API no longer allows a website to force a resolution.
- Fullscreen and landscape lock where the browser supports it.
- Floating player where Document Picture-in-Picture is supported.
- Optional live location for the current device only, after permission.
- VDU visible-tab screen-time counter saved locally in this browser.
- Browser connection estimate and an external full speed test.
- Installable PWA shell and offline reopening of the interface.

## Publish / update on GitHub Pages
Upload the files from this package to the repository root and commit to `main`. GitHub Pages should remain configured for `main` and `/(root)`.

## Important limitations
- VDU itself does not inject ads or analytics. Ads inside YouTube's player are controlled by YouTube and cannot be blocked or skipped by VDU.
- A website/PWA cannot guarantee YouTube playback while Android is locked or force background execution. Browser, battery and YouTube policies control this.
- Geolocation is only for the current device and requires HTTPS plus permission. City/country reverse lookup sends coordinates to BigDataCloud; exact coordinates are not stored by VDU. Background location can be suspended by the OS.
- VDU's screen-time counter measures only visible VDU use, not total Android screen time or other apps.
- Connection details from the browser are estimates; Cloudflare provides the full speed test.
- Offline caching covers the VDU interface only. Video search and streaming require internet.
