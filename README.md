<p align="center">
	<img src="logo.png" width="376" height="128" alt="Winlator Logo" />
</p>

# Winlator MT5

This project builds on [Winlator](https://github.com/brunodev85/winlator) and its
[app source](https://github.com/brunodev85/winlator-app). It adds an optional
**Keep Windows running in background** setting for testing desktop MT5 and other
Windows programs on Android.

In **Settings**, enable **Background Protection**, then **Keep Windows running in
background**, and save. To continue with the screen locked, also enable the
wakelock option. The new option defaults to off. Android can still terminate the
app under memory pressure, and continuous MT5 bot operation needs device testing.

The **Build Android APK** workflow builds a debug APK on pushes to `main` or when
started manually from **Actions**. Download the `winlator-mt5-debug` artifact
from a successful run and extract the APK.

For a local build, use Java 17, Android SDK 35, NDK 24.0.8215888, CMake 3.22.1,
and `bash ./gradlew assembleDebug`. This build uses Winlator's package ID and a debug signing key. Installing it over the official APK requires
a matching signing key or uninstalling that APK first, which removes its app data.

Upstream source snapshot is commit `a030f552f452158a2db64fdb32b490fa19c0b48d`
from `brunodev85/winlator-app`. Upstream license and third-party credits are
retained below and in `LICENSE`.

# Upstream Winlator

Winlator is an Android application that lets you to run Windows (x86_64) applications with Wine and Box86/Box64.<br>
This repository stores the latest updates for the Winlator app source.<br>
For more information and releases, please visit the main repository: https://github.com/brunodev85/winlator

# Credits and Third-party apps

- GLIBC Patches by [Termux Pacman](https://github.com/termux-pacman/glibc-packages)
- Wine ([winehq.org](https://www.winehq.org/))
- Box86/Box64 by [ptitseb](https://github.com/ptitSeb)
- Mesa (Turnip/Zink/VirGL) ([mesa3d.org](https://www.mesa3d.org))
- DXVK ([github.com/doitsujin/dxvk](https://github.com/doitsujin/dxvk))
- VKD3D ([gitlab.winehq.org/wine/vkd3d](https://gitlab.winehq.org/wine/vkd3d))
- CNC DDraw ([github.com/FunkyFr3sh/cnc-ddraw](https://github.com/FunkyFr3sh/cnc-ddraw))

Special thanks to all the developers involved in these projects.<br>
Thank you to all the people who believe in this project.
