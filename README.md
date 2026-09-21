# Alturex Studio — Downloads

Standalone CLI/MCP downloads and archived **Alturex Studio** desktop installers.

**Desktop is deprecated and frozen. Version 0.1.3 is the final desktop release.**
Existing installers and project files remain available; there will be no 0.1.4 desktop release.
The CLI and local MCP server remain supported. Hosted Studio has dev and staging deployments;
production is not deployed. Cloud commands need an operator-provided server URL.

This repository hosts the official Alturex Studio downloads and the update feed the installed
app checks for new versions. For the final desktop build with per-platform install instructions, see the
[downloads page](https://ayrical.github.io/alturex-studio-releases/), or browse every published
version on the [Releases tab](https://github.com/Ayrical/alturex-studio-releases/releases).

This repository distributes release artifacts; it does not contain the application source tree.
Licensing differs by artifact; see [License](#license). Issues and pull requests in this repository
are not monitored — contact Alturex through your normal support channel.

## CLI and local MCP — 0.1.4 (not published yet)

**These are prepared links for the first standalone release. They become available only after
`cli-v0.1.4` is published and verified.** The local CLI and `alturex mcp` work with portable project
files without an account. This is not a desktop 0.1.4 release.

| Platform | Architecture | CLI | MCP extension |
| --- | --- | --- | --- |
| macOS | Apple silicon (arm64) | [CLI tarball](https://github.com/Ayrical/alturex-studio-releases/releases/download/cli-v0.1.4/alturex-cli-darwin-arm64.tgz) | [MCPB](https://github.com/Ayrical/alturex-studio-releases/releases/download/cli-v0.1.4/alturex-studio-0.1.4-darwin-arm64.mcpb) |
| Linux | x64 · glibc 2.35+ | [CLI tarball](https://github.com/Ayrical/alturex-studio-releases/releases/download/cli-v0.1.4/alturex-cli-linux-x64.tgz) | [MCPB](https://github.com/Ayrical/alturex-studio-releases/releases/download/cli-v0.1.4/alturex-studio-0.1.4-linux-x64.mcpb) |
| Windows | x64 | [CLI tarball](https://github.com/Ayrical/alturex-studio-releases/releases/download/cli-v0.1.4/alturex-cli-win32-x64.tgz) | [MCPB](https://github.com/Ayrical/alturex-studio-releases/releases/download/cli-v0.1.4/alturex-studio-0.1.4-win32-x64.mcpb) |

Prepared [release notes](https://github.com/Ayrical/alturex-studio-releases/releases/tag/cli-v0.1.4) and
[SHA256SUMS.txt](https://github.com/Ayrical/alturex-studio-releases/releases/download/cli-v0.1.4/SHA256SUMS.txt).
Always select `cli-v0.1.4` explicitly; GitHub's generic latest release remains desktop 0.1.3.

### Verify and install

The CLI requires **Node.js 22.17.1 through 22.x**, matching the package architecture.
Linux x64 requires glibc 2.35 or newer. Native ITM and dataset helpers are included; installing a
release package does not require Rust or the application source tree.

Download your tarball or MCPB plus `SHA256SUMS.txt` from that same release. Calculate the SHA-256
with one of these commands (replace the filename with your download):

```sh
# macOS
shasum -a 256 alturex-cli-darwin-arm64.tgz
# Linux
sha256sum alturex-cli-linux-x64.tgz
```

```powershell
Get-FileHash .\alturex-cli-win32-x64.tgz -Algorithm SHA256
```

Compare the complete result with the matching filename's line in `SHA256SUMS.txt`. **Do not install
if the hash differs or the filename is missing.** MCPB bundles also have matching `.mcpb.sha256`
sidecars; the same checksum procedure applies.

After verification, replace `<platform>` with `darwin-arm64`, `linux-x64` or `win32-x64`:

```sh
npm install --global ./alturex-cli-<platform>.tgz
alturex version
alturex mcp --help
```

MCPB requires a compatible MCP extension client and Node runtime; real-client installation can vary.
The installed CLI's `alturex mcp` command provides the local stdio alternative. The helpers do not
carry Apple Developer ID notarization or Windows Authenticode signatures; managed-device policies
may restrict execution.

## Archived desktop — 0.1.3

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

### Desktop platforms not supported

| Platform | Architecture | Status |
| --- | --- | --- |
| macOS | Intel (x64) | Not supported. Apple silicon Macs only. |
| Windows | arm64 | Not supported. |
| Linux | arm64 | Not supported. |

## Automatic updates

Older desktop installations can update to the final 0.1.3 release. No later desktop updates are
planned. The archived updater feed remains available.

## License

Each artifact is governed by its accompanying license and third-party notices. Standalone CLI/MCP
0.1.4 packages include an Apache License 2.0 `LICENSE`; the bundled NTIA ITM code has its separate
`NTIA-ITM-LICENSE.md` disclaimer and terms. Consult those included texts for the applicable rights
and obligations.

Archived desktop 0.1.3 installers retain their original accompanying terms. Adding the standalone
CLI/MCP packages does not relicense those older installers or grant rights to other artifacts.
