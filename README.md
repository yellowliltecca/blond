# BLOND — Android music app

BLOND is an Android music player prototype built with Kotlin and Jetpack Compose.

## Build and download the APK

Every push to `main` starts a GitHub Actions build. You can also start one manually:

1. Open the **Actions** tab.
2. Select **Build BLOND APK**.
3. Choose **Run workflow**.
4. When the run completes, open it and download the **BLOND-Android-debug** artifact.
5. Extract the downloaded ZIP and install `app-debug.apk` on your Android phone.

If Android blocks installation, allow your browser or file manager to install unknown apps in Android settings.

## Build locally

Open the repository in Android Studio and sync Gradle. The project uses JDK 17, Android SDK Platform 36, and Gradle 8.13.

On Windows, run `setup-gradle.bat` once to generate the Gradle wrapper, then run `build-debug.bat`.

## Source code

The Android Studio project is stored in `source/BLOND-Android-source.tar.gz`. Extract it to get the complete `BLOND-Android` project directory.

## Music catalog

The prototype uses public Audius catalog endpoints for discovery and search. Availability and playback depend on Audius API and track-level rights/availability. Audius API access is not a blanket commercial music licence.

## Build type

The workflow produces a **debug APK** for testing. It is not a signed production release.
