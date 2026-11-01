# Goodwalk PWA test deployment

- **Live test:** https://seamusmcbride.github.io/dog-walk-pwa-test/
- **Source:** https://github.com/seamusmcbride/dog-walk-pwa-test
- **Hosting:** GitHub Pages, static files, no paid Azure resources created.
- **Data flow:** the app has no API/backend. GPS points and saved walks stay in browser local storage on the device. The site host necessarily serves the static files and may process ordinary request metadata such as IP address; it receives no walk coordinates from this app.
- **Visibility:** source repository and site are public. The app contains no private case, family, or location records.

## Install on iPhone

1. Open the live link in **Safari**.
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. Open Goodwalk from the Home Screen.
4. Tap **Start a walk** and allow location when Safari asks.
5. Keep the app open during this test. This prototype does not claim to keep recording when iOS suspends it or the screen locks.

On Android, open the link in Chrome and use **Install app** or **Add to Home screen**.

## Test boundaries

This is a device test, not a public launch. It has no login, shared profiles, group walks, real mapped/safety-checked trails, server sync, reminder delivery, or AI video. It records GPS only after the user starts a walk and stores points only on that device. Clearing the browser's site data deletes saved walks. Do not use this for emergency navigation or depend on it for a complete route record.

GitHub Pages is a global static host, not an EU-region data-residency guarantee. It is suitable here only because the prototype sends no walk data to the host. Choose an EU region and review the processor terms before adding accounts, syncing routes, or storing user data in a hosted backend.
