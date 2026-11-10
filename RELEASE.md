# WalkerFans H2 Tools — macOS 0.2.2 & Windows 0.3.2 Preview

**WalkerFans for HIFIWALKER H2 Hi-Fi Player / DAP / MP3 Music Player — factory restore, Rockbox installer and USB rescue.**

**Tags:** #HIFIWALKER #HIFIWALKERH2 #Rockbox #DAP #MP3Player #HiFiPlayer #FirmwareRestore

> **Important — based on HIFIWALKER original firmware V2.3.** These tools were developed and tested on an H2 running the original HIFIWALKER firmware **V2.3**. Other firmware versions have not been tested on a real player and may not be compatible. If your player runs a different version, back up first and proceed at your own risk.

Community tools for the HIFI WALKER H2: restore factory firmware, install standard Rockbox 4.0, and load the recovery menu over USB when the player won't start. The app is available in ten languages and needs no internet connection.

## What's new

**macOS 0.2.2**
- Fixed: the app could not be reopened after its window was closed.
- Closing the window during a card operation now waits for the operation to finish before quitting.
- Signed with Developer ID and notarized by Apple.

**Windows 0.3.2 Preview** (replaces 0.3.1 — please update)
- Fixed: "Safely eject the card" failed with **error 23, 8** on some PCs, so the wizard stopped before the final step. The app now ejects the player's USB device the same way as the taskbar "Safely Remove Hardware" icon, stopping at the nearest removable device (USB hubs are never touched).
- If all files are written and verified but Windows still refuses automatic ejection, the app no longer reports an error: it asks you to use "Safely Remove Hardware" and continues to the next step.
- The "Finish on the player" page now shows numbered steps: **System Settings → Firmware Update → YES**, wait for the automatic restart, and what to do if "File not found" appears.
- Fixed unreadable characters in some error messages.
- Rockbox installation and safe ejection have now been tested on Windows hardware.

**Windows 0.3.1 Preview** (earlier)
- First Windows release, with the same restore and install workflows as the Mac app.
- USB rescue for all three known H2 hardware generations (Help → Player won't start (rescue)…). The recovery menu is loaded into RAM only; nothing is written to flash.
- Device and CPU checks before rescue; transfers stop safely on any failure.

## Supported players

- Rockbox installation: H2 original firmware **V1.0–V2.3**.
- Factory recovery: **V2.3 only** for now. Other versions are blocked rather than given the wrong file.
- This installer ships standard Rockbox 4.0. The WalkerFans H2 Rockbox Bluetooth build is a separate download.

## Installed the wrong version?

The app only copies files to the card; the player performs the update itself. It does **not** back up the player's internal firmware (it cannot read it), but most mistakes can be undone:

- **Rockbox does not replace the original system.** Hold **▶** while powering on to start the original firmware.
- **Wrong installer or Rockbox build, player still starts:** run the app again with the version shown in System Settings → Device Information → Version Information and install again. Hold **Volume +** while powering on for the recovery menu and **USB mode**.
- **Black screen / won't start:** **Help → Player won't start (rescue)…** loads the recovery menu into RAM over USB; choose **USB mode** and continue in the main wizard with the correct version.
- **Back to factory firmware:** **Restore factory firmware** (bundled for **V2.3 only**; for other versions, contact us with the diagnostics file from the Help menu).
- Replaced update files and card backups made before formatting are kept in **Documents → HIFIWALKER Backups** on Windows.

## Known limitations

- **Windows is a preview.** It passes 17 automated checks; Rockbox installation and safe ejection were tested on Windows hardware, but formatting and USB rescue have not yet been tested on Windows. It is not Authenticode-signed, so SmartScreen may warn about an unknown publisher. Try it first with a spare card that holds no important data.
- USB rescue on Windows may need the WinUSB driver the first time. Install it with Zadig **only** for USB ID A108:1000; see the manual.
- Formatting erases the whole card. The app backs it up first by default.
- Do not disconnect or power off the player while it is flashing.

## Downloads

| File | Description |
|---|---|
| `HIFIWALKER-Restore-mac-v0.2.2.zip` | macOS 13+, Apple Silicon and Intel |
| `HIFIWALKER-Restore-Windows-v0.3.2-preview.zip` | Windows 10/11 x64, .NET runtime included |
| `Walkerfans-H2-Tools-source.zip` | Complete source for both apps |
| `SHA256SUMS` | Checksums for all files |

See the [manual](https://github.com/walkerfans007/h2-restore/blob/main/MANUAL.en.md) and [changelog](https://github.com/walkerfans007/h2-restore/blob/main/CHANGELOG.md). Rockbox, its bootloaders, libusb and .NET keep their original copyright and license notices; see [THIRD-PARTY.md](https://github.com/walkerfans007/h2-restore/blob/main/THIRD-PARTY.md).

Maintained and released by **WalkerFans Team**. Not an official Rockbox release.

## Español

> **Importante — basado en el firmware original HIFIWALKER V2.3.** Estas herramientas se desarrollaron y probaron en un H2 con el firmware original HIFIWALKER **V2.3**. Otras versiones del firmware no se han probado en un reproductor real y podrían no ser compatibles. Si tu reproductor tiene otra versión, haz antes una copia de seguridad y continúa bajo tu propia responsabilidad.

Herramientas comunitarias para el HIFIWALKER H2: restauración del firmware de fábrica (solo V2.3), instalación de Rockbox 4.0 (V1.0–V2.3) y rescate por USB cuando el reproductor no arranca. macOS 0.2.2 está firmada y notarizada. Windows 0.3.2 es una versión preliminar sin firma: corrige el error 23, 8 al expulsar la tarjeta, y la instalación de Rockbox y la expulsión segura ya se han probado en hardware Windows real. Si instalaste una versión equivocada: Rockbox no borra el sistema original (mantén ▶ al encender), puedes reinstalar con la versión correcta, usar el rescate USB si la pantalla queda negra o restaurar el firmware de fábrica (solo V2.3). Consulta el [README en español](https://github.com/walkerfans007/h2-restore/blob/main/README.es.md) y el [manual en español](https://github.com/walkerfans007/h2-restore/blob/main/MANUAL.es.md).

## Disclaimer

WalkerFans Team is a group of HIFIWALKER fans and geeks. This project is shared for development and community exchange only, and is non-commercial: we make no profit from it. It is not an official Rockbox project release. All trademarks and copyrights belong to their respective owners.

If any content here involves a copyright, patent or other right we are not aware of, please contact us at **walkerfans007@gmail.com** and we will remove it.

— **WalkerFans Team** · walkerfans007@gmail.com
