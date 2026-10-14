# Pawify

A small dark-purple music PWA prototype for iPhone. It can:
- Search Internet Archive's public audio catalogue and stream audio files that are available.
- Save eligible audio into local browser storage for offline playback.
- Import audio files from the iPhone Files picker.
- Play, pause, seek, skip through the current result list, and continue playing while the page stays active.

## Important limitations
- Pawify is not Spotify and does not unlock Spotify Premium or provide Spotify's licensed catalogue.
- Internet Archive results vary; some are recordings, podcasts, or live sets. Downloading depends on source permissions and CORS availability.
- Offline music is stored in Safari website storage. iOS may clear website data, and downloads may fail for sources that block cross-origin access.
- This is a web app/PWA, not a compiled native IPA. iOS background audio behavior can be more limited than a native app, especially after the app is suspended.
- For a Home Screen install, host these files on an HTTPS static host such as GitHub Pages. Open the HTTPS URL in Safari, tap Share, then Add to Home Screen.
- No Mac/Xcode is required to try the web version. A native IPA requires an iOS build/signing workflow.

## Files
- `index.html` app UI and logic
- `manifest.json` PWA metadata
- `sw.js` caches the app shell for repeat/offline launch
