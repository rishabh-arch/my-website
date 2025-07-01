---
title: Remote File Synchronization
description: How to remotely manage and update content in Bharat Signage using ZIP files from an HTTP or FTP server.
sidebar_position: 2
---

With **Bharat Signage**, you can remotely update display content from any location — no need for physical access to the device or a shared local network. This is made possible by syncing a ZIP file from a publicly accessible HTTP or FTP server.

---

## ✅ Requirements

To enable remote content updates, ensure the following:

- Android device with **stable internet connectivity**
- **Bharat Signage** installed on the device
- Access to an **HTTP or FTP server** available over the internet
- A ZIP compression tool like **7-Zip**, **WinRAR**, or **WinZip**

---

## 🔧 Step-by-Step Guide

1. **Create a ZIP Archive**  
   Package all the content files (images, videos, etc.) you want to display into a `.zip` file.

2. **Upload to Your Server**  
   Upload the `.zip` file to your HTTP or FTP server. Ensure the file is accessible via a direct URL.

3. **Access the Web Interface**  
   Open **Bharat Signage**'s web interface from a browser on the same local network.

4. **Set Synchronization Interval**  
   Navigate to `Settings → Device Settings` and set the **Synchronization interval** (e.g., `3600` seconds = 1 hour).

5. **Add Synchronization Entry**  
   Go to `Tools → File Synchronization` and add a new sync entry:
   - **URL**: Provide the full link to your `.zip` file (must start with `http://`, `https://`, or `ftp://`)
   - **File name**: Use `file.zip` — the name must end in `.zip`

6. **Reload the Application**  
   Restart **Bharat Signage**. It will automatically download, extract, and begin displaying the contents of the ZIP file.

7. **Update Anytime**  
   To update content later, just replace the ZIP file on your server. The app will fetch and apply the updated content at the next interval.

---

## 🛠 Troubleshooting

If the device does not show new content:

- Check the log via `Information → Log` in the web interface
- Ensure the server URL is accessible from the Android device

---

## 🔐 Securing Your Server with Authentication

To restrict access to the ZIP file:

- Configure **Basic Authentication** on your HTTP or FTP server
- Include the username and password in the URL:

```text
Format: protocol://username:password@your-server.com
Example: http://admin:securepass@files.bharatsignage.com/file.zip
