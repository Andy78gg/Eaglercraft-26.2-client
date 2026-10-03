# Eaglercraft 26.2 Client

A browser-playable single-file client for **Eaglercraft 26.2**, compiled locally from the
[Eaglercraft-26.2-Workspace](https://github.com/CynTheSolveroftheabsolutefabric/Eaglercraft-26.2-Workspace)
(patched with `eaglercraft-26.2-java-cli 0.1.0-u1` / TeaVM `0.13.1-eagler`).

## Files

| File | Size | What it is |
| --- | --- | --- |
| `eaglercraft-26.2-client.html` | ~106 MB | The full client. Download and open it in any modern browser (Chrome / Edge recommended). Contains all 4,779 gameplay sound effects (from the official 26.2 asset index, transcoded to mono OGG). |
| `eaglercraft-26.2-optional-music.zip` | ~157 MB | Optional music resource pack: 92 background-music / record tracks (original OGG). Import it via the in-game resource pack menu, or ignore it. |

Both large files are stored with **Git LFS**.

## How to play

1. Download `eaglercraft-26.2-client.html`.
2. Double-click it (or serve it over HTTP). No server needed — single-player worlds work out of the box.
3. First load takes a while (~106 MB), that is normal.

Multiplayer requires a compatible Eaglercraft 26.2 server, which is **not** included here.

## Mods

Fullbright-style client mods are planned: the client is recompiled from source whenever a mod
is added, and the updated single-file HTML is pushed to this repository. Open an issue if you
would like a specific mod.

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
