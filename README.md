# Auralis: native app setup

Install Node.js (https://nodejs.org) and, for Android, Android Studio.

## Android (do this first)
1. `npm install`
2. `npx cap add android`
3. `npx cap sync`
4. `npx cap open android`, then press Run in Android Studio with your phone plugged in (USB debugging on).

## iPhone (needs a Mac with Xcode)
1. `npx cap add ios`
2. `npx cap sync`
3. `npx cap open ios`

## After editing www/index.html
Run `npx cap sync` again, then Run in the IDE.

## Features
- Background audio & lock screen media controls (play/pause from lock screen & notification shade).
- High-resolution app icons and splash screen.
- Haptic feedback for meditation intervals and breathing guide.
- Ambient sounds, noise colors, binaural beats, and custom mixes.

## Build the APK on GitHub (no Android Studio)
1. Create a new GitHub repository and upload everything in this folder (including the hidden .github folder).
2. Open the Actions tab, run "Build Android APK" (it also runs on every push to main).
3. When it finishes, open the run and download the "auralis-debug-apk" file, unzip it and install app-debug.apk on your phone.
