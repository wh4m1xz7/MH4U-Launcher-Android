<div align="center">

# MH4U Launcher for Android

**Monster Hunter 4 Ultimate, with an interface built around playing on your phone.**

**0.1.4 · Public Beta · Android 10+ · ARM64**

Gesture movement and camera · Customizable controls · Android keyboard chat

[Download](#download) · [Installation](#installation) · [Controls](#controls) · [Requirements](#requirements) · [Report an Issue](#report-an-issue)

</div>

---

MH4U Launcher is an Android adaptation focused on comfortable mobile play: adjustable controls, a cleaner screen, and quick access to the game's features.

It combines **MH4UltimateDC**, its recompiled game code, and an **Azahar-based runtime** with an Android interface and touch controls adapted by **Mr.suilxz**.

> **This is a public beta.** Device compatibility, performance, and input behavior are still being tested. Stable 60 FPS and any particular rendering resolution are not guaranteed on every phone.

## Download

Open this repository's **Releases** page and download the **ARM64 APK** from the beta release. If you download the ZIP instead, extract the APK before installing it.

Android displays the app version as **0.1.4**. Check the release date and release notes to identify individual beta revisions.

The current APK's checksum is provided in [SHA256SUMS.txt](SHA256SUMS.txt).

## Features

- **Android Mode:** invisible movement controls on the left half and swipe camera controls on the right, with simultaneous multitouch input.
- **Traditional Mode:** visible, configurable virtual gamepad controls.
- **Free layout editing:** move and resize the main image, touch screen, and virtual controls.
- **Full-screen layout:** a large main image with a medium-sized floating touch screen by default.
- **In-game messages:** a compact talking-character shortcut, message window, history, and Android keyboard input.
- **Multiplayer:** room browsing and connections with compatible players.
- **Control customization:** button visibility, sensitivity, mapping, and layout options.
- **Launcher tools:** a mod catalog, FPS counter, image settings, and English and Spanish interfaces.

## Requirements

The APK requires **Android 10 or newer running a 64-bit ARM64 operating system**. A 64-bit processor with a 32-bit Android installation is not sufficient.

Graphics support requires **Vulkan 1.1 or OpenGL ES 3.2**, with compatible device drivers.

These are starting points for testing, **not certified hardware requirements**:

| Profile | Reference processor | Suggested physical RAM | Starting resolution |
|---|---|---|---|
| Baseline testing | Snapdragon 865 or similar performance | 6 GB | 1× |
| More performance headroom | Snapdragon 8 Gen 2 or newer | 8 GB or more | 2×; increase only if performance remains stable |

Less powerful devices may run the game, but require individual testing. Virtual or extended RAM does not replace physical RAM. Temperature, graphics drivers, and rendering resolution affect performance.

## Installation

You need your own compatible copy of **Monster Hunter 4 Ultimate USA** and **game update 1.3.0**.

1. Download and install the APK from **Releases**. If Android asks, allow installation from the app used to open the APK.
2. Open the launcher. Under **Keep your data here**, choose a folder for your progress, settings, and mods.
3. Under **Find your game**, select the folder containing your game.
4. Install update 1.3.0 using the app's **Install CIA file** option. Placing the update file next to the game does not install it.
5. Select **Play**. Start at **1× resolution** and adjust image quality after checking performance.

### Updating the beta

Install the new APK over the previous version and keep using the same data folder. Back up your progress before updating.

If Android refuses the update, record the exact installation message before uninstalling anything. Uninstalling or clearing app data may remove access to your existing configuration.

## Controls

| Action | How to use it |
|---|---|
| Move your character | Touch and drag in a free area on the left half of the screen. |
| Move the camera | Swipe in a free area on the right half. |
| Walk and look around together | Use both thumbs; each gesture keeps its own input. |
| Navigate menus, storage boxes, and lists | Enable **Menus** at the bottom left. Disable it to control character movement again. |
| Show or hide the secondary screen | Tap **Touch**. |
| Open messages | Tap the **talking-character icon**. |
| Move the message shortcut | Drag the character icon. |
| Expand the compact message history | Hold the character icon. Tap **—** to collapse the history. |
| Adjust the compact history | Drag its handle to move it; pinch with two fingers to resize it. |
| Select an item | Open the compact selector from the item button and use its arrows. **Use / sheathe** sends the game's original action. |
| Restore the recommended screen layout | Open **Options → Display**, then select **Recommended: full game + floating touch**. |

Buttons, the touch screen, and floating windows take priority over gestures that begin inside their own interactive areas. Button actions depend on the current context and equipped weapon.

## Beta Status

The current build passes **119 automated tests**, along with signature and library-alignment checks. These checks do not replace real gameplay testing on physical phones.

The main areas requiring further validation are:

- Accepting hunter and Palico names entered through the Android keyboard.
- Keyboard activation and message sending and receiving during multiplayer sessions.
- Simultaneous gestures, menu navigation, and physical controller behavior across devices.
- Stability, temperature, and performance during longer sessions.

The compact item selector uses the game's original inputs. **Read the selected item's name, icon, and quantity from the game's HUD.** The mobile selector does not display a separate inventory or directly select items by ID.

## Report an Issue

Open an **Issue** in this repository and include:

- Phone model, processor, physical RAM, and Android version.
- The downloaded APK filename or release date.
- Graphics backend, rendering resolution, and enabled mods.
- Steps to reproduce the problem, what you expected, and what happened.
- A screenshot, short video, or error log if available.

For multiplayer issues, also say whether you were hosting or joining a room and whether the players were on the same network. Do not post passwords or personal information.

## Credits and Technical Foundations

- **Android adaptation and interface:** Mr.suilxz.
- **Original project and static recompilation:** [MH4UltimateDC](https://github.com/CompaLarios18/MH4UltimateDC).
- **Runtime foundation:** [Azahar](https://github.com/azahar-emu/azahar) and its contributors.
- **Original game:** Monster Hunter 4 Ultimate by CAPCOM.

### Licensing

The Android adaptation follows **GNU GPLv3**. MH4UltimateDC publishes its project code under **GPL-3.0-or-later**, and Azahar publishes its foundation under **GPL-3.0**. Refer to the upstream projects for their original license files and copyright notices.

Distribution of the GPL-covered APK must also provide the corresponding source code, including modifications and the build files needed for that version, under the applicable license terms. An APK and README alone do not replace the corresponding source.

The original game remains the property of its respective rights holders. This is a community project with no affiliation with CAPCOM or Nintendo. You must provide your own compatible game files; this README does not provide downloads of the game or its update.
