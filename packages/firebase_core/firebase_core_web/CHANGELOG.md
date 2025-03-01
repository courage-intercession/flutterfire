## 1.6.6

 - **FIX**: bump `firebase_core_platform_interface` version to fix previous release. ([bea70ea5](https://github.com/firebase/flutterfire/commit/bea70ea5cbbb62cbfd2a7a74ae3a07cb12b3ee5a))

## 1.6.5

 - **REFACTOR**: use "firebase" instead of "FirebaseExtended" as organisation in all links for this repository (#8791). ([d90b8357](https://github.com/firebase/flutterfire/commit/d90b8357db01d65e753021358668f0b129713e6b))

## 1.6.4

 - Update a dependency to the latest release.

## 1.6.3

 - Update a dependency to the latest release.

## 1.6.2

 - **DOCS**: Fix typo in "firebase_core_web.dart" documentation. ([658c1db7](https://github.com/firebase/flutterfire/commit/658c1db71cc47b3eddec3a1f33d5d55d1a6ff98a))

## 1.6.1

 - **FIX**: update all Dart SDK version constraints to Dart >= 2.16.0 (#8184). ([df4a5bab](https://github.com/firebase/flutterfire/commit/df4a5bab3c029399b4f257a5dd658d302efe3908))

## 1.6.0

 - **FEAT**: Bump Firebase Web SDK version to 8.10.1 (CVE-2022-0235) for security patch purposes. (#8162). ([7624f777](https://github.com/firebase/flutterfire/commit/7624f7779f4a49f2353f3f593b31be9139197028))

## 1.5.4

 - Update a dependency to the latest release.

## 1.5.3

 - Update a dependency to the latest release.

## 1.5.2

 - **FIX**: correctly detect `not-initialized` errors and provide a better error message. ([0578423e](https://github.com/firebase/flutterfire/commit/0578423e9868352556bfdd326eef1cca8dbe04aa))

## 1.5.1

 - Update a dependency to the latest release.

## 1.5.0

 - **FEAT**: initial Firebase Installations release (#7377).

## 1.4.0

 - **FEAT**: bump Firebase JS SDK to `8.10.0` (#7460).

## 1.3.0

 - **FEAT**: automatically inject Firebase JS SDKs (#7359).
 - **FEAT**: auto inject Firebase scripts (#7358).

## 1.2.0

 - **FEAT**: support initializing default `FirebaseApp` instances from Dart (#6549).

## 1.1.0

 - **FEAT**: detect the version of the Firebase JS SDK that is in use and warn if the version is incompatible with FlutterFire.
 - **FEAT**: upgrade Firebase JS SDK version to 8.6.1.

## 1.0.3

 - **DOCS**: Add missing homepage/repository links (#6054).
 - **CHORE**: publish packages.
 - **CHORE**: publish packages.
 - **CHORE**: publish packages.
 - **CHORE**: bump min Dart SDK constraint to 2.12.0 (#5430).
 - **CHORE**: publish packages (#5429).
 - **CHORE**: publish packages.

## 1.0.2

 - **FIX**: cannot store null values in firestore on the web (#5335).

## 1.0.1

 - **FIX**: Fix wrong cast (firebase#5050) (#5242).

## 1.0.0

 - Graduate package to a stable release. See pre-releases prior to this version for changelog entries.

## 1.0.0-1.0.nullsafety.0

 - Bump "firebase_core_web" to `1.0.0-1.0.nullsafety.0`.

## 0.3.0-1.0.nullsafety.1

 - **REFACTOR**: pubspec & dependency updates (#4932).
 - **FIX**: Analysis error with firebase_core/web (#4836).
 - **CHORE**: update PromiseJsImpl resolve/reject to match expected types.

## 0.3.0-1.0.nullsafety.0

 - Bump "firebase_core_web" to `0.3.0-1.0.nullsafety.0`.

## 0.3.0-nullsafety.0

Major bump for the null-safety version to respect the versioning convention.

## 0.2.2-nullsafety.1

 - Bump `firebase_core` dependency version.

## 0.2.2-nullsafety.0

 - **REFACTOR**: Migrate to non-nullable types (#4656).

## 0.2.1+3

 - Update a dependency to the latest release.

## 0.2.1+2

 - Update a dependency to the latest release.

## 0.2.1+1

 - **REFACTOR**: ignore typedefs.
 - **FIX**: ensure list items are converted (#4076).

## 0.2.1

 - **FEAT**: migrate firebase interop files to local repository (#3973).
 - **CHORE**: promote to stable version.
 - **CHORE**: remove android directory from web plugins (#3199).

## 0.2.0

* DEPRECATED: `FirebaseApp.configure` method is now deprecated in favor of the `Firebase.initializeApp` method.
* DEPRECATED: `FirebaseApp.allApps` method is now deprecated in favor of the `Firebase.apps` property.
  * Previously, `allApps` was asynchronous where it is now synchronous.
* DEPRECATED: `FirebaseApp.appNamed` method is now deprecated in favor of the `Firebase.app` method.
* BREAKING: `FirebaseApp.options` getter is now synchronous.

* `FirebaseOptions` has been reworked to better match web property names:
  * DEPRECATED: `googleAppID` is now deprecated in favor of `appId`.
  * DEPRECATED: `projectID` is now deprecated in favor of `projectId`.
  * DEPRECATED: `bundleID` is now deprecated in favor of `bundleId`.
  * DEPRECATED: `clientID` is now deprecated in favor of `androidClientId`.
  * DEPRECATED: `trackingID` is now deprecated in favor of `trackingId`.
  * DEPRECATED: `gcmSenderID` is now deprecated in favor of `messagingSenderId`.
  * Added support for `authDomain`.
  * Added support for `trackingId`.
  * Required properties are now `apiKey`, `appId`, `messagingSenderId` & `projectId`.

* Added support for deleting Firebase app instances via the `delete` method on `FirebaseApp`.
* Added support for returning consistent error messages from `firebase-dart` plugin.
  * Any FlutterFire related errors now throw a `FirebaseException`.
* Added a `FirebaseException` class to handle all FlutterFire related errors.
  * Matching the web sdk, the exception returns a formatted "[plugin/code] message" message when thrown.

## 0.1.2

* Update lower bound of dart dependency to 2.0.0.

## 0.1.1+3

* Make the pedantic dev_dependency explicit.

## 0.1.1+2

* Update setup instructions in the README.

## 0.1.1+1

* Add an android/ folder with no-op implementation to workaround https://github.com/flutter/flutter/issues/46898

## 0.1.1

* Require Flutter SDK 1.12.13+hotfix.4 or greater.
* Fix homepage.

## 0.1.0+3

* Remove the deprecated `author:` field from pubspec.yaml
* Bump the minimum Flutter version to 1.10.0.

## 0.1.0+2

* Add documentation for initializing the default app.

## 0.1.0+1

* Use `package:firebase` for firebase functionality.

## 0.1.0

* Initial open-source release.
