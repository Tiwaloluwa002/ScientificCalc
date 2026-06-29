# Calculator App — SEN 104 & SEN 214 Assignment
🤖 Android App Download:
https://expo.dev/artifacts/eas/L8C-ZJkUQ_8lb8AYAcd6uHRDztq4h5TVmZimd5dyMjM.aab
## Overview
A mobile calculator app built with React Native (Expo) that supports basic arithmetic
and scientific/advanced operations for bonus marks.

## Tech Stack
- React Native with Expo
- TypeScript
- Single screen (no navigation needed)

## Core Features (Required)
- Addition, Subtraction, Multiplication, Division
- Clear (AC) button
- Delete last character button
- Decimal point support
- Display shows current input and result
- Handle divide by zero gracefully

## Bonus Features (All of these for max marks)
- Trigonometric: sin, cos, tan (in degrees)
- Inverse trig: sin⁻¹, cos⁻¹, tan⁻¹
- Hyperbolic: sinh, cosh, tanh
- Square root, x², xʸ (power), log, ln
- Permutations nPr and Combinations nCr
- Factorial (n!)
- Statistical: mean, variance, standard deviation (accepts comma-separated input)
- Constants: π and e buttons
- Toggle between Basic and Scientific mode

## UI Requirements
- Dark theme preferred
- Basic mode shows standard calculator layout (numbers + 4 operations)
- Scientific mode reveals extra function buttons above the basic layout
- Toggle button labeled "SCI / BASIC"
- Result display at top, input expression below it
- Buttons should have clear visual feedback on press

## Display Behavior
- Show full expression being typed (e.g. "sin(45) + 3 * 2")
- Show computed result live or on = press
- Error states: show "Error" for invalid operations

## Non-functional
- Runs on Android via Expo Go (physical device)
- No backend, fully client-side
- No external math libraries — use JavaScript Math object only

---

## Running locally (Android & iOS)

Prerequisites:
- Node.js (LTS or newer)
- Expo CLI (optional) and Expo Go app on your device

Install and start the dev server:

```bash
npm install
npx expo start -c
```

- Android: open the Expo Go app and scan the QR code, or press `a` in the dev server to open an emulator.
- iOS: scan the QR code with the Camera app (physical device) or press `i` to open the iOS simulator (macOS only).

---

## Building an APK for Android

To get a downloadable APK file for installation on Android devices:

### Prerequisites
- Expo CLI installed: `npm install -g expo-cli`
- An Expo account (free at https://expo.dev)

### Build using EAS Build

1. **Log in to Expo:**
   ```bash
   npx eas login
   ```

2. **Build the Android APK:**
   ```bash
   npx eas build --platform android --local
   ```
   Or use the cloud build (recommended):
   ```bash
   npx eas build --platform android
   ```

3. **Get the download link:**
   Once the build completes, EAS will provide a download link to the `.apk` file. You can also check your build status on the [Expo Dashboard](https://expo.dev/dashboard).

4. **Install on Android device:**
   - Download the APK from the link provided
   - Transfer to your Android device and tap to install, OR
   - Use ADB (Android Debug Bridge): `adb install path/to/app.apk`

For more info on EAS Build, see the [Expo EAS Build documentation](https://docs.expo.dev/build/setup/).
