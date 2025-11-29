---
id: auto-start
title: Auto Start Feature
description: Automatically start your digital signage application on device boot-up using the Auto Start feature.
sidebar_label: Auto Start Feature
sidebar_position: 3
---

supported by the current version of **Bharat Signage Online** software.

## How to Enable

1. **Open Menu**
2. **Click on Basic Settings**
3. **Configure the Component**
4. Set the **Launcher** using **Open Launcher Setting**.
5. Enable the **Start App on Boot** option to ensure the Bharat Signage application launches automatically on device boot-up.
6. Click on **Set as Default Launcher** and select **Bharat Signage** from the list of available launchers. Then choose **Always** to confirm.
7. **Restart Device**:

## Note

- **If App is not directly launching on Boot**:  
 After enabling the Auto Start feature, if the Bharat Signage application does not launch automatically on device boot-up, then OS might be restricting the app from starting in the background. In such cases, please follow these additional steps:
  - Go to **Device Settings** -> **Apps** -> **Bharat Signage** -> **Battery Optimization**.
  - Select **Don't Optimize** to allow the app to run in the background without restrictions.
- **If app is taking time on launch on Boot**:
   Some devices may have slower boot times or background processes that delay app launch. If you experience delays, consider the following:
  - Ensure no other heavy applications are set to launch on boot.
  - Check for any device-specific settings that may affect startup performance.
  - Restart the device after making changes to see if performance improves.
- **If you want to revert back to previous launcher**:
   To revert back to the previous launcher after setting Bharat Signage as the default launcher, follow these steps:
  - Go to **Device Settings** -> **Apps** -> **Default Apps** -> **Home App**.
  - Select your previous launcher from the list to set it as the default again.
  - Restart the device to apply the changes.

## using ADB or Third-Party Apps

- **Disable System Launcher**:  
- If your device does not allow changing the default launcher through settings, you can use ADB commands or third-party apps to disable the system launcher.
- **Keep Bharat Signage as Launcher**:
- Ensure that Bharat Signage remains set as the default launcher to maintain the auto-start functionality.
