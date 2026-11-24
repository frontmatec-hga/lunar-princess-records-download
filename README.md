# Lunar Princess' Records

A session recorder and stats app for Elden Ring played with Seamless Co-op.

It keeps a record per character of deaths (and deaths by falling), damage taken, healing, runes lost, boss attempts with damage per player, and hands out titles after each session, ending with the Chosen Consort.

## Download

**[Download the latest version](../../releases/latest)** and pick `LunarPrincessRecords.exe` under "Assets".

It is one file. Nothing else needs installing. Windows may warn that it comes from an unknown publisher, because the file is not signed: choose "More info", then "Run anyway".

## What you need

- Elden Ring, version 2.7.2.0
- Seamless Co-op
- Mod Engine 2, with Seamless Co-op's `ersc.dll` in the `external_dlls` line of its `config_eldenring.toml`

## Install

1. Start `LunarPrincessRecords.exe` and open **Setup** (the cog, bottom left).
2. Click **Choose folder** and pick your Mod Engine 2 folder, the one with `launchmod_eldenring.bat` in it.
3. Check the line it shows, then click **Install the recorder**. The config file is backed up first.
4. Start the game with `launchmod_eldenring.bat`. Load a character and it appears in the app.

To undo it, click **Remove the recorder** on the same page.

## Good to know

- **Early version.** The recorder is new and may get things wrong or fail to load. If the game will not start, remove the recorder on the Setup page.
- **It only watches.** The recorder reads the game and writes down what happens. It changes nothing in the game.
- **Never use it with Easy Anti-Cheat active.** Play only through Seamless Co-op or offline.
- **Your recordings stay on your PC,** in `%LOCALAPPDATA%\ErCoopRecords\`. Nothing is uploaded anywhere. The Setup page can make a backup.

## About

A fan-made hobby project. It is not affiliated with or endorsed by FromSoftware or Bandai Namco, and uses none of the game's artwork. The source code is not published here.

The app is built with open-source components, each under its own licence: the .NET runtime (MIT), WPF-UI (MIT), CommunityToolkit.Mvvm (MIT), the Rust standard library (MIT or Apache-2.0), and the Rust crates fromsoftware-rs / eldenring, serde, serde_json, chrono, pelite and windows (MIT or Apache-2.0).