# WalkerFans H2 Tools — macOS 0.2.2 & Windows 0.3.1 Preview

**WalkerFans for HIFIWALKER H2 Hi-Fi Player / DAP / MP3 Music Player — factory restore, Rockbox installer and USB rescue.**

**Tags:** #HIFIWALKER #HIFIWALKERH2 #Rockbox #DAP #MP3Player #HiFiPlayer #FirmwareRestore

Community tools for the HIFI WALKER H2: restore factory firmware, install standard Rockbox 4.0, and load the recovery menu over USB when the player won't start. The app is available in ten languages and needs no internet connection.

## What's new

**macOS 0.2.2**
- Fixed: the app could not be reopened after its window was closed.
- Closing the window during a card operation now waits for the operation to finish before quitting.
- Signed with Developer ID and notarized by Apple.

**Windows 0.3.1 Preview**
- First Windows release, with the same restore and install workflows as the Mac app.
- USB rescue for all three known H2 hardware generations (Help → Player won't start (rescue)…). The recovery menu is loaded into RAM only; nothing is written to flash.
- Device and CPU checks before rescue; transfers stop safely on any failure.

## Supported players

- Rockbox installation: H2 original firmware **V1.0–V2.3**.
- Factory recovery: **V2.3 only** for now. Other versions are blocked rather than given the wrong file.
- This installer ships standard Rockbox 4.0. The WalkerFans H2 Rockbox Bluetooth build is a separate download.

## Known limitations

- **Windows is a preview.** It passes 17 automated checks but has not yet been tested end to end on Windows hardware. It is not Authenticode-signed, so SmartScreen may warn about an unknown publisher. Try it first with a spare card that holds no important data.
- USB rescue on Windows may need the WinUSB driver the first time. Install it with Zadig **only** for USB ID A108:1000; see the manual.
- Formatting erases the whole card. The app backs it up first by default.
- Do not disconnect or power off the player while it is flashing.

## Downloads

| File | Description |
|---|---|
| `HIFIWALKER-Restore-mac-v0.2.2.zip` | macOS 13+, Apple Silicon and Intel |
| `HIFIWALKER-Restore-Windows-v0.3.1-preview.zip` | Windows 10/11 x64, .NET runtime included |
| `Walkerfans-H2-Tools-source.zip` | Complete source for both apps |
| `SHA256SUMS` | Checksums for all files |

See the [manual](https://github.com/walkerfans007/h2-restore/blob/main/MANUAL.en.md) and [changelog](https://github.com/walkerfans007/h2-restore/blob/main/CHANGELOG.md). Rockbox, its bootloaders, libusb and .NET keep their original copyright and license notices; see [THIRD-PARTY.md](https://github.com/walkerfans007/h2-restore/blob/main/THIRD-PARTY.md).

Maintained and released by **WalkerFans Team**. Not an official Rockbox release.

## Español

Herramientas comunitarias para el HIFIWALKER H2: restauración del firmware de fábrica (solo V2.3), instalación de Rockbox 4.0 (V1.0–V2.3) y rescate por USB cuando el reproductor no arranca. macOS 0.2.2 está firmada y notarizada; Windows 0.3.1 es una versión preliminar sin firma y aún no probada en hardware Windows real. Consulta el [README en español](https://github.com/walkerfans007/h2-restore/blob/main/README.es.md) y el [manual en español](https://github.com/walkerfans007/h2-restore/blob/main/MANUAL.es.md).

## Disclaimer

WalkerFans Team is a group of HIFIWALKER fans and geeks. This project is shared for development and community exchange only, and is non-commercial: we make no profit from it. It is not an official Rockbox project release. All trademarks and copyrights belong to their respective owners.

If any content here involves a copyright, patent or other right we are not aware of, please contact us at **walkerfans007@gmail.com** and we will remove it.

— **WalkerFans Team** · walkerfans007@gmail.com
