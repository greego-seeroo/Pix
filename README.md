# Pix — download

**Pix** is a personal AI assistant for coding that runs entirely on your own computer, with an
open-source model (Qwen3.5). It works offline; when online it can search the web and collect
knowledge on topics you follow. Nothing you type leaves your machine.

## Download the latest version

| System | Download |
|---|---|
| macOS (Apple Silicon) | [Pix-mac-arm64.dmg](https://github.com/greego-seeroo/Pix/releases/latest/download/Pix-mac-arm64.dmg) |
| Windows (64-bit) | [Pix-windows-x64.zip](https://github.com/greego-seeroo/Pix/releases/latest/download/Pix-windows-x64.zip) |
| Linux (64-bit) | [Pix-linux-x64.tar.gz](https://github.com/greego-seeroo/Pix/releases/latest/download/Pix-linux-x64.tar.gz) |

All versions: [Releases](https://github.com/greego-seeroo/Pix/releases).

On first run Pix downloads its AI model (about 3 GB) once; after that it works without internet.

### First launch

- **macOS:** the app isn't signed with an Apple certificate yet. If macOS says it can't be opened,
  right-click **Pix** → **Open** → **Open**, or allow it under *System Settings → Privacy & Security*.
- **Windows:** if SmartScreen appears, click **More info** → **Run anyway**.
- **Linux:** unpack, then run `./Pix/Pix`. The app window needs WebKitGTK (`libwebkit2gtk-4.1`); without it,
  Pix opens in your browser instead.

## Requirements

8 GB of memory or more is recommended (4 GB works with the small model). Apple Silicon Macs use the GPU;
Windows and Linux use the CPU.

This repository holds the releases only. The source code is in a private repository.
