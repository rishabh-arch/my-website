---
sidebar_position: 2
---

# External Storage Support

By default, **Bharat Signage** stores all uploaded media files in the device's internal memory, specifically under the folder:

/BharatSignage/slideshow

---

## 🧠 Using SD Card or USB Flash Drive as Permanent Storage

If your device lacks sufficient internal space and includes an **SD/MicroSD card slot** or a **USB port**, you can shift media storage to these external drives. To do this, adjust the setting **`Storage for media`** through either:

- The **web interface**: _Settings → Device Settings_, or
- The **on-screen menu**: _Basic Settings_.

You can verify whether Bharat Signage detects your SD card or USB drive by navigating to:

**_Device Information → External Storages_**

### 📂 External Storage Folder Paths

Depending on the Android version, the app may store files in one of the following locations:

- `/BharatSignage`

⚠️ _Due to Android's security policies, folder locations may vary._

We recommend formatting your external storage using:

- **EXT4**
- **FAT32**

Support for other file systems may vary depending on your Android device.

> Note: _Only media files_ are stored externally. **Configuration files and logs** are always stored in **internal memory**.

After changing the **Storage for media** option, you must **manually re-upload** the media files — they are _not_ automatically copied between internal and external storage.

---

## 🔌 Using USB Flash Drive to Import Content

When a **USB Flash Drive** is inserted into your Android device (via USB host port), Bharat Signage can take one of several actions based on the **`Action on Flash Drive Insert`** setting:

### Available Options:

- **Do nothing**: The flash drive is ignored, and playback continues normally.
- **Copy files from flash drive**: Current playlist pauses. Files from the USB are copied into internal storage, overwriting existing files with the same name.
- **Delete and copy from flash drive**: Same as above, but **all existing files** are deleted first (_irreversible action!_).
- **Play directly from flash drive**: Main zone playlist pauses, and files from the USB are played in **alphabetical order**. Content in other zones is **not affected**.

### 📁 Folder Detection on Flash Drive

You can specify which folder Bharat Signage should look for on the flash drive using the setting:

**`Folder on Flash Drive`**

- If this setting is empty, all files (including hidden ones) in the **root folder** will be used.
- At least **one valid file** must be present in the specified folder for detection to work.

We recommend formatting USB drives to **EXT4** or **FAT32** for maximum compatibility across Android versions.

---

## ⚙️ Auto Setup via `setup.csv`

If you include a file named:

on the flash drive, **Bharat Signage** will automatically detect and process it **before copying any files**.

---
