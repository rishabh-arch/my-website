---
sidebar_position: 1
---

# Local Web & Remote Interfaces

**Bharat Signage Slideshow** can be managed from your **computer, phone, or tablet** if the Android device is connected to the **same local network (LAN)**.  
For **remote access**, use file synchronization via **HTTP/FTP**, **Google Drive**, or **Dropbox**.

---

## 💻 Web Interface

The **web interface** is the **primary management panel** for advanced features.

### 🔗 Accessing the Web Interface

- Open any browser on your computer or mobile device.
- Get the address from **on-screen menu → Help**.
- Common formats:
  - Rooted: `http://<device_ip>`
  - Non-rooted: `http://<device_ip>:8080`

> ⚠️ **Note:** If the device has multiple networks (e.g., Wi-Fi + 4G), ensure you're on the **same active network**. You may need to **disable unused interfaces** to resolve connectivity issues.

### 🔐 Login

- **Default username/password**: `bsadmin / 2024bsadmin##`
- Change credentials via:
  - `Settings → Users`
  - `Settings → Password change`
- Forgot password?
  - **Reset option** available **within 10 minutes** of device startup on the **login page**
  - Requires **physical access** to the device

### ⚙️ Configurable Port Numbers

You can customize port settings via:

- `Settings → Device settings → HTTP/HTTPS port number`
- `On-screen menu → Basic settings → HTTP port number`

> 🔒 Ports below 1024 require a **rooted device**.  
> Common ports:
>
> - HTTP: `8080`
> - HTTPS: `8443`

---

## 🔐 Web Interface via HTTPS

Bharat Signage Offline supports secure HTTPS access:

- Rooted: `https://<device_ip>`
- Non-rooted: `https://<device_ip>:8443`

### SSL Certificate

- By default, a **self-signed SSL certificate** is generated
- You can upload a **custom SSL certificate** (PKCS12 format) via:
  - `Settings → Device settings → Certificate for HTTPS`

---

## 📁 FTP Interface

Access uploaded files using an **FTP client** (e.g., WinSCP, Total Commander).

### FTP Settings

| Setting           | Value                             |
| ----------------- | --------------------------------- |
| IP Address        | Device’s LAN IP                   |
| Port (rooted)     | `21`                              |
| Port (non-rooted) | `8021`                            |
| Username/Password | Same as web login (`admin/admin`) |

- Check current port via: `On-screen menu → Help`
- Change port via: `Settings → Device settings → FTP port number`

> ⚠️ **FTP is not encrypted.** Avoid using it on **open or insecure Wi-Fi networks**.

---

## 🌐 WebDAV Interface

Access files using a **WebDAV client** (e.g., WinSCP).

### WebDAV Settings

| Setting           | Value                             |
| ----------------- | --------------------------------- |
| IP Address        | Device’s LAN IP                   |
| Port              | Same as HTTP/HTTPS                |
| Path              | `/webdav`                         |
| Username/Password | Same as web login (`admin/admin`) |

> ⚠️ Windows’ built-in WebDAV client is **not fully compatible** (due to lack of Basic Auth support).
