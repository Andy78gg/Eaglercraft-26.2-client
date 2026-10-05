# Eaglercraft 26.2 Client — ruian client

A browser-playable single-file client for **Eaglercraft 26.2**, compiled locally from the
[Eaglercraft-26.2-Workspace](https://github.com/CynTheSolveroftheabsolutefabric/Eaglercraft-26.2-Workspace)
(patched with `eaglercraft-26.2-java-cli 0.1.0-u1` / TeaVM `0.13.1-eagler`).

This is a custom build: main menu title **"ruian client"**, custom main-menu background,
and 8 built-in client mods — no source mods to install, everything is compiled in.

## Files

| File | Size | What it is |
| --- | --- | --- |
| `index.html` | ~121 MB | The full custom client. Download and open it in any modern browser (Chrome / Edge recommended). Contains all 4,779 gameplay sound effects (from the official 26.2 asset index, transcoded to mono OGG). |

The large file is stored with **Git LFS**. Note: GitHub Pages does not resolve LFS
pointers, so `https://<user>.github.io/Eaglercraft-26.2-client/` will not render the
game — download the file and open it locally instead.

## How to play

1. Download `index.html` (use the **Download raw file** button, or clone the repo with Git LFS).
2. Double-click it (or serve it over HTTP). No server needed — single-player worlds work out of the box.
3. First load takes a while (~121 MB), that is normal.

Multiplayer requires a compatible Eaglercraft 26.2 server, which is **not** included here.

## Built-in mods

| Mod | Effect |
| --- | --- |
| Fullbright | World brightness maxed (gamma 1.0) — see in the dark |
| No particles | All particle effects disabled |
| No rain / snow | Weather rendering disabled |
| Zoom | Hold **C** to zoom ~5x |
| Toggle sprint | Sprint toggles on/off (no need to hold) |
| No hurt cam | No camera shake when taking damage |
| Small held item | Held items rendered at fixed 0.5x size |
| Autoclicker | Hold left/right click to auto-attack at fixed 12 CPS (toggle with **V**; skips blocks so mining stays normal) |

## Building from source

The workspace already contains the patched toolchain. On Windows you need JDK 25
(`JAVA_HOME` set explicitly), Node.js 22+, Git Bash on `PATH`, and the `wasm-toolchain`
scripts adapted for `gradlew.bat`. Follow the workspace's `GUIDE.md` for the upstream steps.

## Legal

Not affiliated with Mojang or Microsoft. *Minecraft* is a trademark of Mojang Synergies AB.
Eaglercraft is a community reimplementation of Minecraft for personal / educational use.

The sound files in this repository come from the official *Minecraft* 26.2 asset index and
belong to Mojang; publicly distributing them may be subject to DMCA takedown. This repository
exists for personal learning purposes.
