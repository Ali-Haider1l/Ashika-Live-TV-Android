# Ashika Live TV for Android

Separate Android application project for Ashika Live TV.

- Package ID: `com.ashika.livetv.android`
- Version: `1.0.0`
- Minimum Android: 6.0 (API 23)
- Android wrapper: Java + Android WebView
- The web player files at the repository root are copied byte-for-byte from the original `Ali-Haider1l/Ashika-webos` main branch when this project was initialized.
- Android-specific code and build configuration live only in `android/`.
- This repository does not modify or build the webOS IPK.

## Build

GitHub Actions builds a debug APK on pushes to `main` and on manual workflow dispatch. Download it from the workflow run's Artifacts section.

## Notes

Playback depends on the device's Android System WebView, codecs, network, playlist CORS policy, and stream provider. The app does not create or guarantee channel URLs. Use only playlists and streams you are authorized to access.
