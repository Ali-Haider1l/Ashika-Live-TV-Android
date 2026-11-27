# Ashika Live TV for Android

A separate Android edition of Ashika Live TV.

- Package ID: `com.ashika.livetv.android`
- Version: `1.2.0`
- Minimum Android: 6.0 (API 23)
- Android wrapper: Java + Android WebView
- The playlist/player web files were copied from the separate webOS project when this Android repository was initialized.
- Android-specific code and advertising integration live in this repository only.
- The webOS IPK repository is not modified by this project.

## Android features

- M3U/M3U8 URL and local-file playlist import
- Multiple playlists, favourites, recent channels, search and sorting
- TV Guide/XMLTV support
- Quality, audio, subtitle, speed and sleep-timer controls where supported by the stream
- Fullscreen landscape playback and Picture-in-Picture
- Local backup and restore
- Parental PIN option
- Server diagnostics
- Responsive Android-specific midnight/teal visual theme

## Advertising

The Android project includes Google Mobile Ads (AdMob) and Google User Messaging Platform (UMP) consent handling. **Only Google's sample test App ID and banner unit ID are configured.** These are for development testing and do not earn revenue.

Before production:
1. Create and verify the app in your own AdMob account.
2. Replace the sample App ID in `AndroidManifest.xml` and sample banner unit ID in `MainActivity.java` with your own IDs.
3. Configure UMP privacy messages and any required regional consent choices in AdMob.
4. Complete and publish the privacy policy, replacing the publisher-contact placeholder.
5. Only monetize streams and content for which you have the necessary distribution and advertising rights.
6. Verify Google Play and AdMob policies for the intended audience and countries.

Ads are shown in a reserved bottom banner area, not over the video or playback controls. The app does not use forced interstitials or rewarded ads in this version.

## Build

GitHub Actions builds a debug APK on pushes to `main` and on manual workflow dispatch. Download the APK from the workflow run's Artifacts section.

## Privacy

See [PRIVACY_POLICY.md](PRIVACY_POLICY.md) and the in-app [privacy policy page](privacy-policy.html). The policy is a draft and must be reviewed and completed before public distribution.

## Important notes

Playback depends on Android System WebView, supported codecs, network connectivity, playlist CORS settings and the stream provider. The app does not create or guarantee channel URLs. Use only playlists and streams you are authorized to access.
