# ACAN Emergency Green Corridor — HTTPS/PWA package

## Deploy as a separate GitHub Pages site
Do not upload these files into the existing `ident-xray-app` repository; that would replace the iDent app.

1. On GitHub, create a **new public repository** named `acan-green-corridor`.
2. Upload these four files to the repository root: `index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`.
3. Open **Settings → Pages**.
4. Choose **Deploy from a branch**, branch `main`, folder `/(root)`, then Save.
5. Wait for GitHub Pages to publish the site. Its address will be:
   `https://YOUR-GITHUB-USERNAME.github.io/acan-green-corridor/`
6. Open that HTTPS address in Chrome on Android.
7. When Chrome asks for location permission, choose **Allow while using the app**.
8. To install it, use Chrome menu → **Install app** (or **Add to Home screen**, depending on Chrome version).

## GPS notes
- Device location is requested only after the user taps the GPS button.
- HTTPS is required for browser geolocation on a hosted site.
- Android Location must be enabled, and Chrome must have location permission.
- If permission was previously denied, open the site's lock/tune icon → Site settings → Location → Allow, then reload.
- Location accuracy varies. The app's distance is straight-line only, not a road distance or ETA.

## Important safety boundary
This is a prototype. It does not send missions to a dispatcher, contact emergency services, or control traffic signals. Do not use it for real emergency operations. Live deployment requires agency agreements, secure backend services, approved traffic-system interfaces, safety engineering and operational testing.
