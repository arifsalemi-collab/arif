# Doc Scanner (Android)

Free document scanner: scan to PDF (auto-crop, filters, gallery import), save, open, share, rename, delete. One AdMob banner at the bottom of the main screen.

## Get the APK (no Android Studio needed)
1. Create a free GitHub account and a new repository (public is simplest).
2. Upload ALL files from this folder to the repository root (keep the folder structure).
   If the `.github` folder does not upload, create the file `.github/workflows/build-apk.yml`
   in GitHub's web editor and paste the contents of `WORKFLOW-copy-paste.txt`.
3. Open the repository's **Actions** tab -> **Build APK** -> wait ~5-10 minutes for the green check.
   (If it didn't start, click **Run workflow**.)
4. Open the finished run -> **Artifacts** -> download **DocScanner-APK** -> unzip -> `app-debug.apk`.
5. Copy the APK to your Android phone and install it (allow "install unknown apps" when asked).

## Before publishing to Google Play
- Replace the TEST AdMob IDs in `AndroidManifest.xml` and `MainActivity.kt` with your own (AdMob is free).
- Change `applicationId` / package name to your own.
- Build a signed release (AAB), add a privacy policy, fill in the Data safety form.
