# Biomechanics Lab (Android APK)

The game is a single HTML file (`www/index.html`) wrapped in an Android app with Capacitor.
GitHub builds the APK for you; nothing needs installing on your computer.

## How to get the APK
1. Create a new GitHub repository and upload everything in this folder
   (keep the `.github/workflows/build-apk.yml` path exactly as it is).
2. Open the **Actions** tab. The "Build APK" workflow runs on every push to `main`
   (or press **Run workflow** to start it by hand).
3. When it turns green (about 3-5 minutes), open the run and download
   **BiomechanicsLab-APK** from the *Artifacts* section. Unzip it to get `app-debug.apk`.
4. Copy the APK to your phone and install it (allow "install unknown apps" if asked).

## Updating the game
Replace `www/index.html` with the new version and push. A new APK is built automatically.

## Notes
- The app is locked to landscape and fullscreen.
- This is a debug-signed APK: fine for installing on your own phone, but not for the Play Store.
- Change the app name or id in `capacitor.config.json` (`appName`, `appId`) before the first build.
