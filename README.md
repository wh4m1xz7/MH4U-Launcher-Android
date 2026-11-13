<div align="center">

# MH4U Beyond Mobile for Android

**Monster Hunter 4 Ultimate, with controls and menus adapted for phones.**

**v0.1.19 · Public Beta · Android 10+ · ARM64**

Gesture movement and camera · Customizable touch controls · Android keyboard chat · Skip cinematics

</div>

---

MH4U Beyond Mobile is an Android adaptation of MH4UltimateDC, using an Azahar-based runtime and a phone-focused interface. Android adaptation and interface by **Mr.suilxz**.

> **Public beta:** device compatibility, performance, game input, and multiplayer behavior still need testing. Performance depends on the phone, graphics drivers, resolution, and game scene. 60 FPS is not guaranteed.

## Download

This release is the **Lite edition**. It contains the app, not the commercial game files. Use your own compatible MH4U USA game file and update CIA.

- APK: `MH4U-Beyond-Mobile-Lite-v0.1.19-arm64.apk`
- ZIP containing only the APK: `MH4U-Beyond-Mobile-Lite-v0.1.19-arm64.zip`
- SHA-256 (APK): `E11E5EE7D5C4A84921FD241217D4907CB6125FEBC233A5B776070767F8714AB1`
- SHA-256 (ZIP): `CCDFCF297D17210911394074F4EB478085DFAD4DFBBEFE973AA8296DB9525CF5`

## What's new in 0.1.19

- **New button style.** Round buttons with a gold bezel, depth and a press effect, one caption size for all of them, and redrawn icons (combo, menu action, extra action).
- **Kick button.** A dedicated kick button in the same style.
- **Options is the game's START.** The Options button opens the game's own menu, in a hunt or out of it. The app's own menu still opens with the swipe from the side.
- **Skip cinematic.** A video is cut at once. A short scene runs through at full speed, silently, until it ends, then the game returns to normal speed. The speed-up is never used online. This is new and still in beta: report any scene or video where it does not work.
- **Redesigned chat.** A bigger panel by default, message bubbles, new icons, and a redrawn talking-hunter shortcut.
- **Stability.** Fixed several crashes: a graphics warning (an unimplemented gas effect) that closed the game on Android, and a false Java stack-overflow error caused by asking Java for the screen orientation while the game was running.
- **Touch controls no longer hide on some Xiaomi phones**, where a built-in key device was mistaken for a gamepad.
- **Performance for mid and low range phones.** The game thread gets a higher priority and is kept on the fast cores of big.LITTLE chips, the game's code library is read ahead in the background, and a first-run profile is chosen from the phone's memory and chip (lower frame rate, 1x resolution and fewer effects on weaker phones; nothing changes on powerful ones). These changes are not measured on low-end phones yet.
- The launcher shows its version, and its texts refer simply to the CIA.

## Installation

1. Install the APK. If you already have an earlier version, back up your progress and install this APK over it; do not uninstall first.
2. Open the launcher and select the folder containing your own MH4U USA game file.
3. Install your compatible USA update CIA.
4. Wait for installation to finish. After a successful CIA install, the app offers to restart so the update can be loaded. Choose **Restart now** or restart later.
5. Start the game. Begin at **1x resolution**, then increase it gradually if performance remains smooth.

## What's included

- **Android Mode:** swipe to move on the left and control the camera on the right, with multitouch.
- **Traditional Mode:** configurable virtual gamepad controls.
- Move and resize the game screens and touch controls.
- Mobile chat interface with Android keyboard input.
- Local multiplayer room tools, a mod catalog, FPS display, graphics options, and English and Spanish interfaces.
- Select and install a compatible game update CIA in the app.

## Requirements

- Android 10 or newer on a **64-bit ARM64** system.
- Compatible graphics drivers supporting Vulkan or OpenGL.
- Your own compatible **MH4U USA** game file and update CIA. The APK does not include them.
- Free storage for the app, game data, updates, and save data. The needed space depends on the files you import.

## Controls

- Touch and drag in a free area on the left side to move.
- Swipe in a free area on the right side to turn the camera.
- Use both thumbs to move and look at the same time.
- **Options** opens the game's START menu. Swipe in from the side to open the app's menu and adjust the touch controls and screen layout.
- **Skip cinematic** appears while a scene or video plays.
- Use the talking-character shortcut to open mobile chat and type with the Android keyboard.

Button actions may depend on the current game screen, equipped weapon, and installed update. If a text field does not open the phone keyboard, report the exact screen and game update you selected.

## Updating

Back up your progress before updating. Install the new APK over the existing app and keep the same app data. Uninstalling can remove app data and saves.

## Report an issue

Open an Issue in this repository and include your phone model, Android version, APK edition and filename, selected game update, graphics backend, resolution, and steps to reproduce the problem. Screenshots or a short video are useful. If the game closes, attach the `log/azahar_log.txt` from your data folder, copied before you reopen the game. Do not post passwords or personal information.

## Source code and license

This project is distributed under the GNU General Public License v3.0 (GPLv3). The corresponding source code, including the changes in this release, must be published alongside the APK in this repository.

## Credits and notice

Built on [MH4UltimateDC](https://github.com/CompaLarios18/MH4UltimateDC) and the [Azahar](https://github.com/azahar-emu/azahar) project. Credit belongs to their respective contributors. Monster Hunter 4 Ultimate is a CAPCOM game.

This is an unofficial community project and is not affiliated with CAPCOM or Nintendo. The game and update files remain the user's responsibility and are not included in this Lite APK.
