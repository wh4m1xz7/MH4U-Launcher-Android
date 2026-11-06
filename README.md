<div align="center">

# MH4U Beyond Mobile for Android

**Monster Hunter 4 Ultimate, with an interface built around playing on your phone.**

**0.1.13 · Public Beta · Android 10+ · ARM64**

Gesture movement and camera · Customizable controls · Android keyboard chat

[Download](#download) · [Installation](#installation) · [Controls](#controls) · [Requirements](#requirements) · [Report an Issue](#report-an-issue) · [Español](README.es.md)

</div>

---

MH4U Beyond Mobile is an Android adaptation focused on comfortable mobile play: adjustable controls, a cleaner screen, and quick access to the game's features.

It combines **MH4UltimateDC**, its recompiled game code, and an **Azahar-based runtime** with an Android interface and touch controls adapted by **Mr.suilxz**.

> **This is a public beta.** Device compatibility, performance, and input behavior are still being tested. Stable 60 FPS and any particular rendering resolution are not guaranteed on every phone.

## Download

| Edition | Download size | APK filename | Setup |
|---|---:|---|---|
| **Lite** | ~102 MB | `MH4U-Beyond-Mobile-Lite-v0.1.13-arm64.apk` | Select your own MH4U USA ROM folder and install update 1.3.0 (.cia) in the app. |
| **Full** | ~2.63 GB | `MH4U-Beyond-Mobile-v0.1.13-arm64.apk` | Install the APK and open it to start the game. |

Both editions have the same controls and features. Lite keeps future app downloads smaller because you supply the game files separately. The installed version appears under **by Mr.suilxz** in the in-game side menu.

Check the 0.1.13 announcement for download links. [Discord community](https://discord.gg/zTJ6uJHYy)

If you download a ZIP, extract the APK before installing. Verify your file against the published checksums. [SHA256SUMS.txt](SHA256SUMS.txt)

## What's new in 0.1.13

- Turn the camera while sprinting. Hold **Sprint** and drag the same finger, or use a second finger to look around.
- Move the target icon, weapon button, item arrows, **Use** button and quest shortcuts independently.
- The item selector shows how many units of the selected item you have left.
- Lite and Full are available as separate builds of the same version.

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

### Lite

1. Install the Lite APK and open the launcher. Follow the prompts for file access if Android asks.
2. Tap **Select ROM folder** and choose the folder with your own copy of **Monster Hunter 4 Ultimate USA**.
3. Tap **Install CIA update**, select the **1.3.0** CIA, and wait for installation to finish. If the launcher detects the update in the game folder, you can install it from there.
4. Select **Play**.

### Full

1. Install the Full APK.
2. Open the app to start the game.

Start at **1× resolution** in either edition. Adjust image quality after checking performance in an actual hunt.

### Updating or switching editions

Back up your progress, then install the APK over the previous version and keep using the same data folder. Lite and Full use the same app identity and signing certificate, so installing one replaces the other. If you switch to Lite for the first time, complete the ROM and CIA setup above.

## Controls

| Action | How to use it |
|---|---|
| Move your character | Touch and drag in a free area on the left half of the screen. |
| Move the camera | Swipe in a free area on the right half. |
| Move and look around together | Use both thumbs to move and look. While holding **Sprint**, you can also drag that finger to turn the camera. |
| Navigate menus, storage boxes, and lists | Enable **Menus** at the bottom left. Disable it to control character movement again. |
| Show or hide the secondary screen | Tap **Touch**. |
| Open messages | Tap the **talking-character icon**. |
| Move the message shortcut | Drag the character icon. |
| Expand the compact message history | Hold the character icon. Tap **—** to collapse the history. |
| Adjust the compact history | Drag its handle to move it; pinch with two fingers to resize it. |
| Select an item | Open the compact selector with **Item** and use its arrows. The selector shows the quantity of the selected item. |
| Restore the recommended screen layout | Open **Options → Display**, then select **Recommended: full game + floating touch**. |

Buttons, the touch screen, and floating windows take priority over gestures that begin inside their own interactive areas. Button actions depend on the current context and equipped weapon.

## Beta Status

Both 0.1.13 APKs passed **165 automated tests** per edition, plus signing and native-library checks. The Lite ROM and CIA import flow still needs testing on physical phones.

Please report issues with name entry, multiplayer chat, touch and controller input, or performance during longer hunts. FPS and image quality vary by device, graphics backend and resolution.

## Report an Issue

Open an **Issue** in this repository and include:

- Phone model, processor, physical RAM, and Android version.
- Whether you use Lite or Full and the downloaded APK filename.
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

The original game remains the property of its respective rights holders. This is a community project with no affiliation with CAPCOM or Nintendo. The Lite edition uses your own compatible game files.
