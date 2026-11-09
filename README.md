# rupianii – website to Android APK

Wraps https://www.rupianii.com/ in an Android app (Capacitor WebView) using your logo as the launcher icon.

## Use
1. Create a GitHub repo and push the contents of this folder.
2. Open **Actions → Build rupianii APK → Run workflow** (or just push).
3. Download the `rupianii-apks` artifact: `app-debug.apk` installs directly on a phone.

## Notes
- `app-release-unsigned.apk` cannot be installed or uploaded to Play until signed. For Google Play, create a keystore and sign it (I can add that step).
- The app loads the live site, so it needs internet and site updates appear instantly. Google Play may reject apps that are only a website wrapper; consider adding native value (push notifications, offline page).
- Change `app-id` before publishing if you want a different package name; it can't change after release.
- `build/index.html` is only a fallback splash that redirects to the site.
