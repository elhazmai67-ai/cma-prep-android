# CMA Prep Android APK

This project wraps the existing `CMA Prep.html` app in an Android WebView using Capacitor and builds a debug APK using GitHub Actions.

## Build on GitHub
1. Create a public or private GitHub repository named `cma-prep-android`.
2. Add these files preserving the paths:
   - `www/index.html` (the existing HTML app)
   - `package.json`
   - `capacitor.config.json`
   - `.github/workflows/build-apk.yml`
3. Commit the files to the `main` branch.
4. Open the repository's **Actions** tab and open **Build CMA Prep Android APK**.
5. If it has not started automatically, choose **Run workflow**.
6. Wait for the run to finish with a green check mark.
7. Open the completed workflow run and download the `CMA-Prep-debug-APK` artifact. GitHub downloads the artifact as a ZIP; extract it to get `app-debug.apk`.
8. On your Android phone, tap `app-debug.apk` and follow Android's installation prompt. You may need to allow your browser or file manager to install unknown apps.

## Important
- This is a debug APK for personal installation/testing, not a Play Store release.
- The workflow artifact is retained for 14 days.
- The app stores its current progress in local storage on that device. Uninstalling the app or clearing its app data may erase saved progress.
- Keep your repository files private if you do not want the HTML source to be public.
