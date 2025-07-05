---
sidebar_position: 1
title: Auto-Start After Reboot
description: How to configure Bharat Signage to automatically start after device reboot for uninterrupted playback.
---

To ensure continuous playback on your Bharat Signage-powered screen. Especially in scenarios like power failures or scheduled restarts. It's essential to configure **Bharat Signage** to **launch automatically when the device boots**.

> 💡 **Only one method should be used at a time.** Avoid combining multiple auto-start methods to prevent unexpected behavior.

---

### 🏠 Method 1: Set Bharat Signage as the Android **Launcher / Home App** (Recommended)

The **Launcher** is the main interface Android loads immediately after booting up. If your Android device is dedicated to digital signage, setting Bharat Signage as the Launcher ensures **seamless and faster startup**, while also giving a more **professional appearance** (saving up to 15 seconds during boot).

### 🔧 How to Set

1. Launch the Bharat Signage app.
2. Navigate to:  
   `Basic Settings → Set Bharat Signage as Launcher / Home Application` at the bottom of the menu.

![Screen Menu](/img/offline-usb-images/automatic-startup/menu-open.jpg)
![Launcher Settings](/img/offline-usb-images/automatic-startup/set-as-launcher.jpg)

1. A system prompt will appear. Select **Bharat Signage** and choose **"Always"** if available.
2. On some devices, you may need to repeat steps 2 and 3 once more to confirm.
3. Reboot the device. Bharat Signage will now start immediately after the device powers on.

> 📝 When Bharat Signage is set as the Launcher, pressing the **Home** button on the remote or device will bring up the Bharat Signage screen.  
> To exit or open another app, select **Exit** from the app’s on-screen menu. You can revert this setting through `Basic Settings`.

---

## 🔁 Method 2: Enable **Start at System Boot**

If you prefer to keep your existing Launcher or are sharing the device for multiple purposes, you can enable Bharat Signage to **launch after the system boots** — without changing the Launcher.

1. Open Bharat Signage.
2. Go to:  
   `Settings → Enable "Start at System Boot"`

   ![Menu Settings](/img/offline-usb-images/automatic-startup/menu-settings.jpg)
   ![Start at system boot](/img/offline-usb-images/automatic-startup/start-at-system-boot.jpg)

3. Depending on your Android version, you may be asked to grant **"Display over other apps"** or **"Appear on top"** permission.
4. If prompted, the app will attempt to navigate you to the appropriate Android Settings screen.
   - If it fails, manually go to:  
     `Android Settings → Apps → Bharat Signage → Special Access / Permissions → Allow Display Over Other Apps`

> 🔔 Bharat Signage will now automatically open a few seconds after the device finishes booting.

---

## 📱 Method 3: Use Built-in Android Startup Settings (Device Dependent)

Some Android devices offer a built-in option to **launch apps automatically on boot** via the manufacturer's custom Android skin.

1. Locate Bharat Signage in your list of installed apps.
2. Long-press the icon or tap the app settings.
3. Look for an option like **“Auto-launch on boot”**, **“Start automatically”**, or **“Launch on startup”** and enable it.

> ❗ This option is **not available on all devices**. It depends on whether the device manufacturer included this feature in their Android version.

---

## ✅ Best Practice Recommendation

If your Android screen is solely dedicated to running Bharat Signage, using it as the **Launcher** is the most robust and elegant solution.  
For multi-purpose devices, **Start at System Boot** is the ideal fallback.

For further assistance, visit:  
👉 [https://bharatsignage.com/contact-us](https://bharatsignage.com/contact-us)
