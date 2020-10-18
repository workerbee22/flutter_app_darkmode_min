# Flutter Dark Mode - Minimal App

Default Flutter app, with just two line changes to support light/dark mode on Android and iOS devicess that supoort it.

Two key lines changed in `MaterialApp()`are:
```
darkTheme: ThemeData.dark(),
themeMode: ThemeMode.system,
```

**Android 10** and above devices that support light/dark mode:
- Light or dark theme set by Android in Settings or Quick Settings, automatically changes the app theme without doing anything in the app
- App state is maintained when the operating system changes theme
- App uses the default Theme.light or Them.dark values

**iOS 13.x** and above devices that support light/dark mode:
- Light or dark theme set by iOS in Settings, automatically changes the app theme
- App state is maintained when the operating system changes theme

**Lower Versions of Android & iOS**
On Android 9, lower power mode will set a dark mode, the app utomatically changes to this theme without doing anything in the app
On Android 8.x and iOS 12.x lower versions, there is no light/dark theme support, so the app defaults to th elight theme always.

**macOS**
- macOS Catalina v10.15.7 and above tested and working correctly. 
- the app picks up the with the light/dark/auto Appearance as set in macOS in Settings / General.

**Windows 10**
There is an issues that is currently open preventing the Flutter app listening for the Windows app theme value or chnages to it. See issue here: https://github.com/flutter/flutter/issues/54612

