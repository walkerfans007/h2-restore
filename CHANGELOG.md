# Changes — WalkerFans H2 Tools

## Windows 0.3.1 Preview
- Added X1000 A108:1000 USB RAM rescue for three H2 hardware generations.
- Added verified bundled bootloaders and official libusb 1.0.30 x64 DLL, WinUSB setup guidance, and ten-language rescue UI.
- Stop before upload on an unexpected CPU; stop the boot sequence on incomplete transfers.
- 17 automated checks pass, including reference decompression hashes and boot protocol ordering. Not yet tested on Windows hardware; unsigned.

## Windows 0.3.0 Preview
- Initial native Windows wizard for stock recovery and Rockbox installation, FAT32/MBR checks, verified backup/copy, formatting and safe removal.

## macOS 0.2.2
- Fixed close/reopen: closing the last window exits the app; busy card operations finish before exit.

## macOS 0.2.1
- Added the H2 product icon; signed and notarized package.

## macOS 0.2.0
- Added standard Rockbox installation alongside factory restoration.
- Added ten languages, system-language selection and Arabic right-to-left layout.
- Bundled firmware and Rockbox files; verified writes, backup and cleanup.
- Fixed an extra-directory copy bug and added a regression check; retested the correct card-root layout.
