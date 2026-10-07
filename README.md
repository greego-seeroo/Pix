# Pix — download

**Pix** is a personal AI assistant for coding that runs entirely on your own computer, with an
open-source model (Qwen3.5). It works offline; when online it can search the web and collect
knowledge on topics you follow. Nothing you type leaves your machine.

## Download the latest version

| System | Download |
|---|---|
| macOS (Apple Silicon) | [Pix-mac-arm64.dmg](https://github.com/greego-seeroo/Pix/releases/latest/download/Pix-mac-arm64.dmg) |
| macOS (Intel) | [Pix-mac-x64.dmg](https://github.com/greego-seeroo/Pix/releases/latest/download/Pix-mac-x64.dmg) |
| Windows (64-bit) | [Pix-windows-x64.zip](https://github.com/greego-seeroo/Pix/releases/latest/download/Pix-windows-x64.zip) |
| Linux (64-bit) | [Pix-linux-x64.tar.gz](https://github.com/greego-seeroo/Pix/releases/latest/download/Pix-linux-x64.tar.gz) |

All versions: [Releases](https://github.com/greego-seeroo/Pix/releases).

On first run Pix downloads its AI model (about 3 GB) once; after that it works without internet.

### First launch

- **macOS 13.3+:** the app isn't signed with an Apple certificate. Drag Pix to Applications and open it; when
  macOS refuses, open *System Settings → Privacy & Security* and click **Open Anyway**, then open Pix again.
- **Windows:** if SmartScreen appears, click **More info** → **Run anyway**.
- **Linux (Ubuntu 22.04 or newer):** `tar xzf Pix-linux-x64.tar.gz && ./Pix/Pix`. Pix opens in your browser;
  quit it with *Settings → Quit Pix*.

## Requirements

8 GB of memory or more is recommended (4 GB works with the small model). Apple Silicon Macs use the GPU;
Windows and Linux use the CPU.

## How releases are made

This repository holds the download page, the releases, and the build workflow
(`.github/workflows/build.yml`). The workflow checks out the source code from a private repository with
a read-only key, builds Pix on macOS, Windows and Linux, tests each build with a small model, and
publishes the packages here. Each release lists SHA-256 checksums in `SHA256SUMS.txt`.
