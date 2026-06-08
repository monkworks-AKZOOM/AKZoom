Tested on Ancient Kingdoms v0.9.20.0

# AKZoom
AK Zoom v1.0 - Simple Camera Zoom for Ancient Kingdoms
# AK Zoom

A simple camera zoom mod for **Ancient Kingdoms** using MelonLoader.

AK Zoom lets you cycle between the game’s normal camera view, a closer gameplay view, and a photo-style close-up view.

## Controls

Press:

P


to cycle through zoom modes:


Normal View → Close View → Photo View → Normal View


## Zoom Modes

- **Normal View**: Uses the game’s current default camera zoom.
- **Close View**: Sets camera zoom to 6.
- **Photo View**: Sets camera zoom to 2.

The normal zoom is captured from the game at runtime, so if the developers adjust the default camera in a future update, AK Zoom should still return to the correct normal view.

## Requirements

- Ancient Kingdoms
- MelonLoader installed for Ancient Kingdoms
- AKZoom.dll

## Installation

1. Install MelonLoader for Ancient Kingdoms.
2. Open your Ancient Kingdoms install folder.

Usually:


C:\STEAM\steamapps\common\Ancient Kingdoms


3. Open the `Mods` folder.

C:\STEAM\steamapps\common\Ancient Kingdoms\Mods


4. Copy `AKZoom.dll` into the `Mods` folder.
5. Launch Ancient Kingdoms.
6. Load into the game world.
7. Press `P` to cycle zoom modes.

## Confirming It Loaded

After launching the game, check:

C:\STEAM\steamapps\common\Ancient Kingdoms\MelonLoader\Latest.log


You should see something like:


AK Zoom v3.2 loaded.
Normal zoom is captured from the game camera at runtime.
Captured game default zoom: X


## Troubleshooting

### The mod does not load

Make sure `AKZoom.dll` is directly inside:


Ancient Kingdoms\Mods


Not inside another nested folder.

Correct:


Ancient Kingdoms\Mods\AKZoom.dll


Incorrect:


Ancient Kingdoms\Mods\AKZoom\AKZoom.dll


### P does nothing

Check `Latest.log` and look for:


AK Zoom v3.2 loaded.


If that line is missing, MelonLoader did not load the mod.

Also make sure the game window is focused and you are loaded into the game world.

### The game updated and the mod stopped working

Ancient Kingdoms may have changed its camera system. Remove `AKZoom.dll` from the `Mods` folder and wait for an updated version.

## Notes

AK Zoom modifies the game’s Cinemachine virtual camera lens value at runtime. It does not replace sprites, scale the UI, or modify saved games.

## Uninstall

Delete:


Ancient Kingdoms\Mods\AKZoom.dll


## Version

AK Zoom v1.0  
Created by Monk
