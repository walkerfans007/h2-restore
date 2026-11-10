# WalkerFans H2 Tool — Quick Manual

Back up your music/settings, record the original firmware version, and charge the player to at least 50%.

macOS: extract v0.2.2, move the app to Applications, then open it. Requires macOS 13 or later, Intel or Apple Silicon. Windows: extract the complete v0.3.1 preview, keep Assets beside the EXE, and approve its administrator prompt. The Windows runtime is included; Windows hardware acceptance and Authenticode signing remain outstanding.

Install: read System Settings → Device Information → Version Information on the original system. Choose Install Rockbox, select that exact version, connect the player/card reader, confirm the correct card and capacity, and follow the wizard. Formatting erases the card: use the verified backup option first. After copy/verification/eject, unplug, then choose System Settings → Firmware Update → YES on the player. Do not interrupt flashing. Reconnect and remove the installer when prompted. This installs standard Rockbox 4.0; the Bluetooth development package is a separate subsequent upgrade for supported hw4 devices.

Restore: bundled factory recovery is V2.3 ONLY. Power off, hold Volume + and press Power, choose USB mode, and use Restore factory firmware. After verified copy/eject, unplug, enter the menu again and choose HibyOS Recovery (Aigo Recovery on older menus). Wait for completion, boot normally, and clean up the installer. Advanced bootloader-only recovery instead uses Bootloader → Restore.

USB rescue: Help → rescue. Power off fully, connect the cable to the player, hold M while connecting it to the PC, then release M. The screen remains dark in boot ROM mode. Select the correct hardware generation (V1.0–V1.6 / V1.7–V1.8 / V1.9–V2.3). On Windows, first-time setup may require WinUSB via the official Zadig website: select ONLY USB ID A108:1000, never normal storage/input devices. Do not disable driver signature checks. Detect and load the recovery menu; this is a temporary RAM boot, not a flash restore. Confirm the player's screen yourself, choose USB mode and return to the main wizard. Save diagnostics if it remains dark.

Power normally for Rockbox; hold ▶ while powering on for the original system; hold Volume + while powering on for the recovery menu. Closing the window during a card operation defers exit until completion.

Maintenance and documentation: **WalkerFans Team**. Original Rockbox/libusb/.NET and firmware notices remain applicable.

Non-commercial community project by WalkerFans Team. If any content involves a copyright or patent we are not aware of, contact walkerfans007@gmail.com and we will remove it.
