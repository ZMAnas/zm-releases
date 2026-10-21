# ZM Sensor releases

This public repository holds **only finished app files** for ZM Sensor (ZM Motorsport) and the small version files the app reads to check for updates. There is no source code, no keys and no user data here.

| Channel | Version file | Who gets it |
|---|---|---|
| main | `main.json` | the normal ZM Sensor Android app |
| test | `test.json` | ZM Sensor test builds |
| ethanol | `ethanol.json` | the ethanol-only build (no OBD adapter) |

How it works: when the Android app starts, it reads its channel's version file. If the `versionCode` there is higher than its own, it offers **Update**; the APK is downloaded from this repository's Releases, its SHA-256 is checked, and Android asks the user to install it. Android only accepts an update signed with the same key as the installed app, so nobody else can push an update.

Releases are made by Claude for Anas from the private repos; don't edit these files by hand.
