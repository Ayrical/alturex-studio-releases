# Alturex Studio — Downloads

Archived installers and the auto-update feed for **Alturex Studio** desktop.

**Desktop is deprecated and frozen. Version 0.1.3 is the final desktop release.**
Existing installers and project files remain available; there will be no 0.1.4 desktop release.
The CLI and local MCP server remain supported. The graphical client is moving to a hosted web
app, which is not deployed yet.

This repository hosts the official Alturex Studio downloads and the update feed the installed
app checks for new versions. For the final desktop build with per-platform install instructions, see the
[downloads page](https://ayrical.github.io/alturex-studio-releases/), or browse every published
version on the [Releases tab](https://github.com/Ayrical/alturex-studio-releases/releases).

This repository contains **binaries only**. Alturex Studio is proprietary software; the source
code is developed in a private repository and is not available here. Issues and pull requests in
this repository are not monitored — contact Alturex through your normal support channel.

## Download

| Platform | Architecture | Package | Download |
| --- | --- | --- | --- |
| Windows 10/11 | x64 | `.exe`, `.msi` | [Installer (recommended)](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.3/Alturex.Studio_0.1.3_x64-setup.exe) · [MSI](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.3/Alturex.Studio_0.1.3_x64_en-US.msi) |
| macOS 12+ | Apple silicon (arm64) | `.dmg` | [Download](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.3/Alturex.Studio_0.1.3_aarch64.dmg) |
| Linux | x64 | `.AppImage`, `.deb`, `.rpm` | [AppImage](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.3/Alturex.Studio_0.1.3_amd64.AppImage) · [Debian / Ubuntu](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.3/Alturex.Studio_0.1.3_amd64.deb) · [Fedora / RHEL](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.3/Alturex.Studio-0.1.3-1.x86_64.rpm) |

See the [0.1.3 release](https://github.com/Ayrical/alturex-studio-releases/releases/tag/0.1.3)
for release notes and supporting files.

Windows setup works offline when the Microsoft Edge WebView2 Runtime is already installed. A fresh
Windows machine without WebView2 needs network access during setup so the embedded bootstrapper can
download the runtime; Alturex Studio works offline after installation.

### Platforms not currently supported

| Platform | Architecture | Status |
| --- | --- | --- |
| macOS | Intel (x64) | Not supported. Apple silicon Macs only. |
| Windows | arm64 | Not supported. |
| Linux | arm64 | Not supported. |

## Automatic updates

Older desktop installations can update to the final 0.1.3 release. No later desktop updates are
planned. The archived updater feed remains available.

## License

Copyright © Alturex. All rights reserved.

The installers in this repository are provided for use of Alturex Studio by its intended users.
No rights to the source code are granted. Redistribution of modified binaries is not permitted.
