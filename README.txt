# VDU Plus — free GitHub Pages package

## Files
- `index.html`: VDU web app.
- `manifest.webmanifest`: installable PWA metadata.
- `sw.js`: caches the app shell for offline reopening; it does not run continuously in the background.
- `vdu-icon-192.png`, `vdu-icon-512.png`: app icons.

## Update your existing GitHub repository
1. Open https://github.com/jitender30meena-sys/vdu-video
2. Choose **Add file → Upload files**.
3. Upload all five files from this folder to the repository root (not into a new folder).
4. Commit directly to `main` with message `Upgrade VDU Plus tools`.
5. GitHub Pages is already configured for `main` and `/(root)`, so the next commit should redeploy the site automatically.
6. Open https://jitender30meena-sys.github.io/vdu-video/ after the Pages deployment finishes. Refresh or clear the old site cache if the previous version remains.

## Feature and browser limitations
- Enter in the search field submits the search; `/` focuses search.
- 10-second seek and playback-speed controls use the official YouTube IFrame API.
- YouTube no longer exposes API methods to set/get resolution. Use the YouTube player's Settings → Quality menu; YouTube can choose Auto.
- YouTube ads inside its official player are controlled by YouTube. VDU itself does not inject ads or analytics.
- Background playback cannot be guaranteed by a website/PWA. Android/Chrome/YouTube control screen-off behaviour. Media Session actions are provided when supported.
- Document Picture-in-Picture works only in supported browsers (mostly desktop Chromium). If unavailable, use YouTube's own PiP feature where the browser offers it.
- Live location is for the current device only and requires HTTPS and explicit permission. Browser/OS may pause location updates in background. City/country reverse lookup sends coordinates to BigDataCloud; exact coordinates are not saved by VDU.
- Screen-time tracking counts only time when this VDU page is visible in this browser, not Android-wide usage.
- The Network Information API is only an estimate. The Cloudflare button opens a full external speed test.
- PWA offline support caches the VDU interface only. Video search and video streaming still require an internet connection.
