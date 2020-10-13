# Flutter Dark Mode Minimal App

Default Flutter app, with just two line changes to support light/dark mode on Android and iOS devicess that supoort it.

- Android 10 and above devices that support light/dark mode:
- Light or dark theme set by Android in Settings or Quick Settings, automatically changes the app theme without doing anything in the app
- App state is maintained when the operating system changes theme

- iOS 13.x and above devices that support light/dark mode:
- Light or dark theme set by iOS in Settings, automatically changes the app theme
- App state is maintained when the operating system changes theme

On Android 9, lower power mode will set a dark mode, the app utomatically changes to this theme without doing anything in the app
On Android 8.x and iOS 12.x lower versions, there is no light/dark theme support, so the app defaults to th elight theme always.
