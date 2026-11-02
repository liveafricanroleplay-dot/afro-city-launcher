# AFRO CITY LAUNCHER

Android SA-MP Mobile launcher rebrand for AFRO CITY RP.

## Branding scope
This project is based on the supplied Alyn SA-MP Mobile v17.x source snapshot. The intended changes are limited to launcher identity (app label, icon, splash/launcher artwork, and AFRO CITY RP community links). The original package/namespace and native SA-MP client integration are retained to protect Java/JNI compatibility.

## Build requirements
- JDK 17
- Android SDK 35
- Android NDK 25.1.8937393
- CMake
- Gradle wrapper included in source

## Source import required
The repository currently contains the build workflow but not the Android source tree. Upload and extract the contents of `AFRO_CITY_RP_Launcher_Source_Modified.zip` into the repository root so that `settings.gradle`, `gradlew`, and `app/build.gradle` are at the root / expected paths. Do not upload the ZIP as a replacement for the source tree.

## Build
Use the **Android APK Build** workflow under Actions. The workflow builds debug and release APK variants. The release APK is signed with Android's debug key for testing; create and configure a private release signing key before distributing a production APK.

## Important compatibility notes
- Package ID remains `ro.alynsampmobile.launcher`; changing it can break native/JNI integration.
- The source snapshot targets GTA: San Andreas Android 2.10.
- Existing Alyn-hosted update/server-list endpoints may remain dependencies until replaced with AFRO CITY RP-compatible services.
- Do not redistribute proprietary GTA assets or third-party assets without permission.
