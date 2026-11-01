# Goodwalk PWA test

A no-account, static PWA prototype for trying dog-walk GPS recording on iPhone Safari and Android browsers.

Live at [Goodwalk test PWA](https://seamusmcbride.github.io/dog-walk-pwa-test/). See [DEPLOYMENT.md](DEPLOYMENT.md) for install steps and data-handling limits.

## What it does

- Starts GPS only after the user taps **Start a walk**.
- Shows a timer, distance estimate, GPS point count, and a schematic trace.
- Saves finished walks and their points in this browser's local storage.
- Pauses/resumes location explicitly; finishing stops GPS.
- Caches the app shell for offline reopening after the first visit.
- Includes a clearly labelled sample trail that is not a real route or navigation map.

## Limits

- It is a test, not a finished safety/navigation app.
- No account, server sync, social/group features, reminder delivery, or AI video generation.
- Location and history stay in browser storage on the device. Clearing site data removes them.
- GPS recording should be tested with Safari open. This prototype does not claim continuous tracking after the browser is backgrounded or the screen locks.
- No external map tiles, fonts, analytics, or location services are contacted by the app.

## iPhone use

Open the HTTPS site in Safari, tap Share, then **Add to Home Screen**. Open it from the Home Screen and allow location when prompted. Walks require an active internet-independent GPS fix; the app shell can reopen offline after first load.

## Local preview

Serve this folder over HTTP for visual preview. Browser geolocation generally requires HTTPS (or localhost), so GPS on a phone should be tried only on the HTTPS hosted build.
