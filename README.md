# Alturex Planner — Downloads

Official installers and the auto-update feed for **Alturex Planner**, a local-first RF link and
network topology planner.

This repository hosts the official Alturex Planner downloads and the update feed the installed
app checks for new versions. For the latest build with per-platform install instructions, see the
[downloads page](https://ayrical.github.io/alturex-planner-releases/), or browse every published
version on the [Releases tab](https://github.com/Ayrical/alturex-planner-releases/releases).

This repository contains **binaries only**. Alturex Planner is proprietary software; the source
code is developed in a private repository and is not available here. Issues and pull requests in
this repository are not monitored — contact Alturex through your normal support channel.

## Download

No release has been published yet. The table below goes live with the first signed release.

| Platform | Architecture | Package | Download |
| --- | --- | --- | --- |
| Windows 10/11 | x64 | `.msi` | _pending first release_ |
| macOS 12+ | Apple silicon (arm64) | `.dmg` | _pending first release_ |
| Linux | x64 | `.AppImage`, `.deb`, `.rpm` | _pending first release_ |

Each release includes SHA-256 checksums and Sigstore provenance for every installer. Verify the
checksum of anything you download before installing it.

### Platforms not currently supported

| Platform | Architecture | Status |
| --- | --- | --- |
| macOS | Intel (x64) | Not supported. Apple silicon Macs only. |
| Windows | arm64 | Not supported. |
| Linux | arm64 | Not supported. |

## Automatic updates

Installed copies of Alturex Planner check this repository's releases for updates. Update metadata
(`latest.json`) and every update bundle are cryptographically signed; the app verifies the
signature against a key embedded at build time and will not install anything that fails
verification. Updates are never installed without your explicit confirmation, and never while a
project save is pending.

## License

Copyright © Alturex. All rights reserved.

The installers in this repository are provided for use of Alturex Planner by its intended users.
No rights to the source code are granted. Redistribution of modified binaries is not permitted.
