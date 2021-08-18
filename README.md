# ExpoSplashScreenRepro

This repository contains two projects that demonstrate the same issue in different ways.

## ExpoManagedSplashScreenRepro

An Expo Managed Workflow app that shows an alert while the splash screen is visible.

Created via `expo init` with the TypeScript template. The code in `App.tsx` is copied from the official Expo documentation with a call to `Alert.alert` added in.

To run:
1. Install packages: `yarn`
2. Start Metro: `yarn start`
3. Open the app in Expo Go on your iOS device

## ExpoBareSplashScreenRepo

An Expo Bare Workflow app that shows an alert from the Objective-C code while the splash screen is visible.

Created via `expo init` with the bare minimal template. Only the code in `didFinishLaunchingWithOptions` has been modified.

To run:
1. Install packages: `yarn`
2. Open in Xcode and select a Team for automatic signing.
3. Install pods: `cd ios && pod install`
4. Run on your iOS device: `yarn ios --device`

