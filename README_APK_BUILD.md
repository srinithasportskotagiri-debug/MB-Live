# MB Live Android APK Build

This is the Android Studio project for MB Live.

## Build an installable APK using GitHub Actions

1. Create a GitHub repository.
2. Upload the contents of this folder to the repository root (`app`, `gradle`, `.github`, `build.gradle`, `settings.gradle`, `gradlew`, etc.).
3. Open the repository's **Actions** tab.
4. Select **Build MB_Live APK** and click **Run workflow** (or push a commit to trigger it).
5. After the workflow completes successfully, open the run and download the **MB_Live-apk** artifact.
6. Extract the artifact ZIP; `app-debug.apk` is the installable APK. Transfer it to the Android phone and open it to install. Android may ask you to allow installs from that source.

## Build locally with Android Studio

Open this folder in Android Studio, allow Gradle sync to finish, then choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**. The project targets SDK 35 and has minimum SDK 25.

**Important:** This archive contains project source, not a prebuilt APK. A build needs Android SDK components and internet access to download Gradle/dependencies. The current build environment could not download Gradle, so no APK was generated here.
