---
title: Multiple Display Synchronization Guide
description: Learn how to Sync Multiple Bharat Signage Devices to Play in Perfect Harmony
sidebar_position: 3
---

### Sync Multiple Bharat Signage Devices to Play in Perfect Harmony

---

## 📌 Overview

This guide walks you through setting up **multiple Bharat Signage Android devices** to **play synchronized content**—starting at the **same timestamp**, frame-perfect, with optional **smooth playback**. This is ideal for installations like video walls, digital menu boards, or synchronized ads across screens.

![Example banner](/img/real-world-images/two-display-sync.png)

> 🔗 Required:  
> Visit the Bharat Signage CMS offline USB setup page:  
> **[https://cms.bharatsignage.com/offline-usb/](https://cms.bharatsignage.com/offline-usb/)**
> Use **version 4.9.16** or **4.10** for synchronization features.

---

## 🛠️ Step-by-Step Instructions

---

### 🧩 Step 1: Configuration Settings

In the **Configuration** tab of the CMS page:

1. **Go to** `Advanced Settings`
   - ✅ Click **Generate Communication Code**
     > This enables inter-device communication.
   - ✅ Enable **Communication Tracker**
     > This ensures timing consistency across displays.
   - ✅ _(Optional)_ Enable **Smooth Playback**
     > Improves playback sync and reduces visual jitter.

---

### 🧭 Step 2: Zone Sync Setup

Switch to the **Zone Setup** tab:

1. **Enter a Sync Code**

   > You can use any simple identifier (e.g., `hello`, `sync123`, or `zone1`).  
   > All devices using the same code will play in sync.

2. **Zone-Specific Playback**
   - To sync only one zone, use `zone1` as your sync code.
   - You can also sync other layouts like `zone2` or `zone3` for split screen scenarios.

---

### 💾 Step 3: Download Required Files

- Download both the:
  - ✅ **Template file**
  - ✅ **Setup file**

> These files contain your configuration and sync logic.

---

### 📁 Step 4: Prepare USB Pen Drive

1. Create a folder on your USB named:  
   **`bharatsignage`**

2. Place the following files into this folder:
   - ✅ **Bharat Signage APK file**
   - ✅ **configuration** file
   - ✅ **setup** file
   - ✅ **template** file

---

### 🗂️ Step 5: Folder Structure

Your pen drive should look like this:

```js
bharatsignage/
├── configuration.xml
├── setup.csv
├── zone1/
│ ├── video1.mp4
│ └── video2.mp4
├── zone2/
│ └── ...
├── zone3/
│ └── ...
```

- **`zone1/`** – Full-screen sync content
- **`zone2/`** – Split-screen (2-part) content
- **`zone3/`** – Split-screen (3-part) content
- **`configuration`** – Contains settings
- **`setup`** – Auto-connects Wi-Fi or other startup preferences

---

### 🔌 Step 6: Deploy to Android Devices

1. Plug the **USB pen drive** into your **Android TV or media player**.
2. Use the **remote control** to open the **File Browser**.
3. **Install the APK first.**
   > ⚠️ The APK must be installed before inserting the sync files to allow system-level modifications.
4. The app will automatically read configuration and enable synchronization.

---

### 🔌 Step 7: Reboot Device (Optional)

- After installation, you can reboot the device to ensure all settings are applied correctly.
- The app will automatically start syncing content based on the sync code provided.

---

## 🎯 Final Notes

- All devices must **use the same sync code** to stay in perfect sync.
- Ensure **date/time** settings are consistent across devices.
- If one display lags, it will automatically catch up during the next sync cycle.
- For smoothest results, keep **video files identical in format, bitrate, and resolution**.

---

## 🤝 Support

Need help with synchronization or setup?  
Reach out to the **Bharat Signage support team**:  
**[https://bharatsignage.com/contact-us/](https://bharatsignage.com/contact-us/)**
