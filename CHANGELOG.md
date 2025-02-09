# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [1.8.3]

### Fixed

- Fixed an issue on Android where building the SDK would fail when depending on player SDK v5.x.

## [1.8.2]

### Fixed

- Fixed an issue on Android where building the SDK would fail when depending on player SDK v4.12.0.

## [1.8.1]

### Changed

- Restructured iOS bridge code to extensions based on features.

### Fixed

- Fixed an issue on Android where the system UI would not be restored when unmounting THEOplayerView with `fullscreen` enabled.
- Fixed an issue with the availability of the cast button and play buttons in the example application.
- Fixed an issue on iOS where the player was not destroyed correctly on the iOS bridge.
- Added support for `DRMConfig` through `SourceDescription` for SSAI sources on iOS.

## [1.8.0]

### Added

- Support for Chromecast and Airplay.

### Fixed

- Fixed an issue where moving the sender app to the background while playing a DAI source on an Airplay device, would pause playback.

### Changed

- Upgraded Web SDK to v4.6.0.
- Updated the custom build setup to support both iOS and tvOS.

## [1.7.2]

### Fixed

- Fixed an issue on tvOS where a feature flag was incorrectly used for ads-related code.

## [1.7.1]

### Fixed

- Fixed an issue on Android where the player would consider unusable custom drm integrations.
- Fixed missing kotlin classpath property on Android.

## [1.7.0]

### Added

- Support for content protection integration (DRM connectors).
- Support for subscribing to ad events.
- Support for Google DAI ads.
- Support for Google IMA ads.
- Support for ABR configuration on Android and Web.
- Support for video quality selection on Android and Web.

### Fixed

- Fixed an issue where the player would not be correctly released when destroying the view on Android.
- Fixed a warning during debugging when a stream would have duration INF or NaN.
- Fixed an issue in the example app where it would not be possible to select a specific text track.
- Fixed conflicting npm dependencies in the example app.

## [1.6.1]

### Added

- Improved source handling for iOS.

## [1.6.0]

### Fixed

- Fixed jitpack.io repository url for Android.
- Fixed an issue where play-out of HLS streams would fail on Android.

### Changed

- Excluded folders from bob build config.
- Upgraded gradle versions for Android.

## [1.5.0]

### Fixed

- Fixed disabling all debug logs for iOS/tvOS release builds.
- Fixed duration from seconds to milliseconds on iOS/tvOS.

### Added

- Support for DRM pre-integrations on Android.
- Support for additional source properties on Android: `liveOffset`, `hlsDateRange`, `timeServer` and `hls`.

## [1.4.0]

### Fixed

- Fixed an issue on iOS where subtitles upon disappearing would sometimes leave a thin black line on the image.
- Fixed an issue on iOS where the player would not be destroyed after going to fullscreen.

### Added

- Improved determination of the stream source type on Android.

## [1.3.0]

### Fixed

- Fixed an issue where the app would crash due to the configured Flipper version.
- Fixed duplicate classes issue for Android when having dependencies on local libs folder.
- Fixed documentation feature matrix.
- Fixed duration scale in loadedmetadata event properties for Web.

## [1.2.0]

### Fixed

- Fixed a crash when removing text tracks event listeners on iOS.
- Fixed a number of broken links in the documentation.
- Removed unused files.

## [1.1.0]

### Added

- Initial release.
