

This is a custom build: main menu title **"ruian client"**, custom main-menu background,
and built-in client mods — no source mods to install, everything is compiled in.

## ▶ Play online (GitHub Pages)

**https://andy78gg.github.io/Eaglercraft-26.2-client/**

Open that link in Chrome / Edge and press Play. The first load takes a while
(~100 MB), that is normal.

## Files

| File | Size | What it is |
| --- | --- | --- |
| `index.html` | ~79 KB | Entry page for the online (multifile) build, served by GitHub Pages |
| `classes.wasm` + `*.wasm` + `*.epk` | ~200 MB | The actual game binaries/assets for the online build |
| `eaglercraft-26.2-client.html` | ~121 MB | **Single-file offline build** — download and open in any browser; contains all 4,779 sound effects (from the official 26.2 asset index, transcoded to mono OGG) |

The large files are stored with **Git LFS**. GitHub's web "Download raw file" only
shows the LFS pointer as a `.txt` — to get the real single-file build use either:

- `git clone https://github.com/Andy78gg/Eaglercraft-26.2-client.git` then
  `git lfs pull`, or
- the **Releases** page if a release asset is attached.

## How to play offline

1. Get `eaglercraft-26.2-client.html` (clone with LFS, or Releases).
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
| Autoclicker | Hold left click to auto-attack; toggle with **V**, adjust CPS 1–20 with the `\` / `|` key (chat shows current CPS; skips blocks so mining stays normal) |

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
