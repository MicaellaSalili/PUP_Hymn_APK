# How to Run This Cordova App on Android

## Prerequisites

- [Node.js](https://nodejs.org/) installed
- [Java JDK 8 or 11](https://adoptopenjdk.net/) installed and `JAVA_HOME` set
- [Android Studio](https://developer.android.com/studio) (for Android SDK & emulator)
- [Apache Cordova CLI](https://cordova.apache.org/) installed globally:
  ```sh
  npm install -g cordova
  ```

## 1. Install Dependencies

From the project root, install npm dependencies:
```sh
npm install
```

## 2. Prepare the Android Platform

If not already present, add the Android platform:
```sh
cordova platform add android
```
> If `platforms/android` already exists, you can skip this step.

## 3. Build the App

```sh
cordova build android
```
- The APK will be generated in `platforms/android/app/build/outputs/apk/`.

## 4. Run on an Android Device or Emulator

- **To run on a connected device:**
  ```sh
  cordova run android
  ```
- **To run on an emulator:**
  ```sh
  cordova emulate android
  ```

## 5. Troubleshooting

- Make sure your device has USB debugging enabled.
- If you encounter SDK or Gradle errors, open the project in Android Studio and let it resolve dependencies.

## Project Structure

- `www/` — App source files (HTML, CSS, JS, assets)
- `config.xml` — Cordova configuration
- `platforms/` — Platform-specific code (auto-generated)
- `plugins/` — Cordova plugins

---

For more, see the [Cordova Documentation](https://cordova.apache.org/docs/en/latest/guide/cli/).
