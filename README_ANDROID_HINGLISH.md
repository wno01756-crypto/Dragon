# Dragon World 3D – Android APK packaging kit

This is a phone-friendly PWA wrapper around the current Dragon World HTML game.
It is **not yet an APK**. To produce an APK without a PC, publish this folder to an HTTPS website, then use PWABuilder's cloud packaging service.

## Important
- Game uses Three.js from jsDelivr and PeerJS from unpkg, so first launch and multiplayer require internet.
- This package does not add new GTA V assets or turn the game into native Unity. It wraps the current HTML game as an installable web app.
- APK packaging happens in the cloud after hosting; the APK is not generated inside this ZIP.

## Steps on your Android phone
1. Extract this ZIP using your phone's file manager / ZArchiver.
2. Upload the **contents** of this folder to a static HTTPS host (for example, a static-site hosting service). The published site must open `index.html` at an HTTPS URL.
3. Open https://www.pwabuilder.com in Chrome and paste that HTTPS URL.
4. Choose **Package for stores** → **Android** → **Generate Package**.
5. Choose a new signing key for a first test build, then download the package ZIP.
6. Extract the downloaded ZIP and install its `.apk` file on your phone. Android may ask you to allow Chrome / Files to install unknown apps.
7. Keep `signing.keystore` and its password details safe for future updates.

PWABuilder Android packaging requirements and steps:
https://github.com/pwa-builder/PWABuilder/blob/main/docs/builder/android.md

## Current game controls
Use the on-screen controls already in the game. Rotate the camera on the right side of the screen.
