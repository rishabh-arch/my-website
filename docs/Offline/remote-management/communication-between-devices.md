---
title: Multi-Device Communication
description: Learn how Bharat Signage devices can connect and synchronize with each other over LAN or the internet.
sidebar_position: 3
---

**Bharat Signage** supports seamless interaction between multiple screens running the app. Using a proprietary communication protocol, devices can exchange data for basic monitoring, control, and synchronized playback — making it ideal for multi-screen digital signage setups.

---

## 🧩 Group-Based Device Linking

To allow devices to connect and collaborate, they must be assigned the **same Group Code**. Only devices with matching codes can see and interact with each other.

---

## 🌐 Modes of Connectivity

### 📶 Local Network (LAN)

When devices are on the **same local network**, they can discover each other automatically using **UDP multicast**.

- ✅ Recommended: Wired Ethernet for best results.
- ⚠️ Note: Some Wi-Fi networks and routers may block multicast traffic, preventing discovery.

### 🌍 Internet (WAN)

Devices on **different networks** can connect over the internet in some cases. This depends on network configuration:

- 🔄 Enable **“Device discovery on the internet”** in Bharat Signage settings.
- 🔧 Requires router support for **UPnP (Universal Plug and Play)**.
- ⚠️ May fail with **double NAT** setups or ISPs using **Carrier-grade NAT (CGNAT)**.

---

## 🔒 Security Considerations

- Your **Group Code** also acts as a security key. Keep it private.
- If you’ve used the "Nearby Devices" feature previously, update the Group Code from the default `DEFAULT_GROUP_CODE` before enabling internet-based discovery.
- Strongly recommended: Change the default **admin credentials** for the web interface if enabling discovery over the internet.

---

## 📺 Managing Connected Devices

Access a list of all discovered devices from the Bharat Signage web interface:

- Navigate to `Settings → Other Devices`
- View connected players along with available remote actions

### 🌐 Tunnel to Remote Device

For devices **outside your network**, Bharat Signage provides a **Tunnel Web Interface**:

- Click the **Tunnel** button to open the web interface of another player in a new browser tab.
- Useful for accessing remote players across different networks.
- ⚠️ Only **one tunnel** session can be active at a time.
- 🚨 Note: Tunnel speed is slower than standard LAN performance due to additional routing.

---

## 📘 Summary

Multi-device communication in **Bharat Signage** enables:

- Real-time sync between players
- Remote access across networks
- Flexible scaling for video walls or networked signage grids

Make sure to configure your network and security settings carefully for the best experience.
