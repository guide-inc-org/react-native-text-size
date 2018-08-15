# Changes

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

**WARNING**

_The package id has changed, you must uninstall the previous version before using this one._

### Added
- Adds flow typings (almost) working with Flow 0.61.x
- Enhancements to the example with RN 0.56 and Flow
- New functions `specsForTextStyles`, `fontFromSpecs`, and `fontFamilyNames`

### Changed
- Simplify anroid/build.gradle and adjust the configuration.
- `allowFontScaling` is handled in the native side, index.js was simplified a lot.
- Migration of example to RN 0.52 and Typescript, enhanced features.
- Minimum supported versions: RN 0.52.x, Android SDK 16, iOS 9.0
- New fformat of the CHANGELOG to follow the _Keep a Changelog_ recommendations.
- Package ID now is `com.github.amarcruz.rntextsize` for Android, and `RNTextSize` for iOS.
- Fixes to typings.

### Removed
- Drop support for iOS 8 and RN below 0.52

### Fixes
- Improved measurement on both platforms, accuracy is more than 5 decimals.
- The iOS API and behavior of `measure` now is the same as Android.
- Makes the example works.

## [1.0.0-beta.5] - 2018-07-11
_Unpublished_
- Preliminary implementation for iOS (thanks to @xuhom)
- The license is changed to BSD 2-Clause as [react-native-measure-text](https://github.com/airamrguez/react-native-measure-text), on which this library is based.

## [1.0.0-beta.4] - 2018-04-23
_Unpublished_
### Changed
- Now the SDK versions are compatible with global rootProject.ext for flexible configuration.

## [1.0.0-beta.3] - 2018-02-17

Published to npm, tested with Android SDK 21.

### Changed
- Updates compileSdkVersion, buildToolsVersion and targetSdkVersion.
- Gradle plugin to 2.3.3

## [1.0.0-beta.2] - 2018-03-06
_Unpublished_
### Fixes
- Correction to the default export in the index
### Changed
- Using ES6 for index.js

## [1.0.0-alpha.10] - 2018-02-20
_Unpublished_
### Changed
- compileSdkVersion 25, buildToolsVersion 25.0.3, targetSdkVersion 25

## [1.0.0-alpha.9] - 2018-02-19
_Unpublished_
### Changed
- Revision to README
- targetSdkVersion from 22 to 23.
### Fixes
- Fix error in android path
- Android package id is 'io.amarcruz.rnmeasuretext'

## [1.0.0-alpha.8] - 2018-01-29
_Unpublished_
### Added
- Suppport for `includeFontPadding`
### Changed
- Using gradle 2.2.3

## [1.0.0-alpha.7] - 2018-01-11
_Unpublished_
### Added
- Returned info includes `lineCount` with the number of lines and `lastLineWidth` with the last line width (Android).
- Uses scaled `fontSize` (with `allowFontScaling`, automatic).
### Changed
- Makes `width` property optional in parameters (Android).
- Minor fixes, now working.
- First commit, Android only.