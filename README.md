# Alturex Studio — Downloads

Official installers and the auto-update feed for **Alturex Studio**, a local-first RF link and
network topology planner.

This repository hosts the official Alturex Studio downloads and the update feed the installed
app checks for new versions. For the latest build with per-platform install instructions, see the
[downloads page](https://ayrical.github.io/alturex-studio-releases/), or browse every published
version on the [Releases tab](https://github.com/Ayrical/alturex-studio-releases/releases).

This repository contains **binaries only**. Alturex Studio is proprietary software; the source
code is developed in a private repository and is not available here. Issues and pull requests in
this repository are not monitored — contact Alturex through your normal support channel.

## Download

| Platform | Architecture | Package | Download |
| --- | --- | --- | --- |
| Windows 10/11 | x64 | `.exe`, `.msi` | [Installer (recommended)](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.1/Alturex.Studio_0.1.1_x64-setup.exe) · [MSI](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.1/Alturex.Studio_0.1.1_x64_en-US.msi) |
| macOS 12+ | Apple silicon (arm64) | `.dmg` | [Download](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.1/Alturex.Studio_0.1.1_aarch64.dmg) |
| Linux | x64 | `.AppImage`, `.deb`, `.rpm` | [AppImage](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.1/Alturex.Studio_0.1.1_amd64.AppImage) · [Debian / Ubuntu](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.1/Alturex.Studio_0.1.1_amd64.deb) · [Fedora / RHEL](https://github.com/Ayrical/alturex-studio-releases/releases/download/0.1.1/Alturex.Studio-0.1.1-1.x86_64.rpm) |

See the [0.1.1 release](https://github.com/Ayrical/alturex-studio-releases/releases/tag/0.1.1)
for release notes and supporting files.

### Platforms not currently supported

| Platform | Architecture | Status |
| --- | --- | --- |
| macOS | Intel (x64) | Not supported. Apple silicon Macs only. |
| Windows | arm64 | Not supported. |
| Linux | arm64 | Not supported. |

## Automatic updates

Alturex Studio checks this repository for new releases and asks before installing an update.
Updates are never installed while a project save is pending.

## License

Copyright © Alturex. All rights reserved.

The installers in this repository are provided for use of Alturex Studio by its intended users.
No rights to the source code are granted. Redistribution of modified binaries is not permitted.
