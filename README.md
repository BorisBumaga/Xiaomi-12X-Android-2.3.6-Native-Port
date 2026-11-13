# Android 2.3.6 Gingerbread — Xiaomi 12X

Experimental Android 2.3.6 Gingerbread for **Xiaomi 12X**.

## Screenshots

| About phone | Gingerbread Easter egg |
| --- | --- |
| ![Android 2.3.6](media/screenshots/01-about-phone.jpg) | ![Gingerbread Easter egg](media/screenshots/02-gingerbread-easter-egg.jpg) |

| Home screen | Lock screen |
| --- | --- |
| ![Home screen](media/screenshots/03-gingerbread-home-screen.jpg) | ![Lock screen](media/screenshots/04-gingerbread-lock-screen.jpg) |

## Boot

1. **Unlock the bootloader** of your Xiaomi 12X.
2. Download `boot.img` from this project's releases (once published).
3. Install Android Platform Tools, connect the phone and enter **fastboot** mode.
4. Run:

   ```bash
   fastboot devices
   fastboot boot boot.img
   ```

**No partition flashing is required:** `fastboot boot` temporarily boots the supplied image without writing it to a partition. The image must be compatible with your device. This does not guarantee that every device configuration will boot successfully.

> **Warning:** An unlocked bootloader is required. Unlocking may erase user data. You perform all actions **at your own risk**. Back up important data first.