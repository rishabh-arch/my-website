---
sidebar_position: 3
---

# Content and Playlist Management

With **Bharat Signage**, you can fully customize what’s displayed on screen using **content** and **playlists**. These features can be managed directly from the **web interface**.

---

## 📁 Content Types

Content refers to the media or data shown on your display. Below are the supported content types:

- **Single file** – Display one specific file stored in the internal storage.
- **Files alphabetically** – Play multiple files in alphabetical order. Grouping can be based on:
  - 📂 _Folder location_
  - 🏷️ _Filename prefix_
  - 🧩 _File extension_
- **Files randomly** – Random playback of multiple files with a smart shuffle algorithm.
- **Audio/Video stream** – Stream from a URL (e.g., webcam, internet radio).
- **Date/Time** – Show current date/time using the device’s system clock.
- **Weather** – Display weather data from an online source.
- **RSS messages** – Show live news and updates via RSS feeds.
- **Plain text** – Single-line, unformatted text display.
- **Nothing** – Only the background is shown; useful for custom layouts.
- **Today’s name day** – Displays today’s celebrated first name.
- **Video input** – Live preview from a connected camera or HDMI input.
- **YouTube video** – Play YouTube-hosted content.
- **Android widget** – Embed widgets from installed Android apps.

---

## 🗂️ Path Formats for File-Based Content

For **Files alphabetically** and **Files randomly**, the `Path` field supports the following formats:

- `image1.jpg` – Play a single file directly.  
  _Tip: Use **Files → Right-click → Create new content from here** to auto-fill this path._

- `folder1/*` – Play all files in a specific folder.  
  _Right-click a folder to auto-fill._

- `folder1/**` – Include all files in the folder and its subfolders.

- `**` – Play files from all folders and subfolders.

- `folder1/*:folder2/*` – Combine multiple folder paths using colons.

You can create and manage content via **📌 Menu → Content**.

---

## 📋 Playlists

A **playlist** is a sequence of content items played in a loop until manually changed or updated via a schedule. Each content entry resolves to a single file or stream, displayed for a defined duration.

- ⏹️ **Mute** – No audio playback.
- 🎬 **From video** – Audio plays only from video or stream content.
- 🎵 **Audio playlist** – Audio-only playback (not assignable to screen zones).

**Note:** When new content is created, a playlist is automatically generated. If your playlist includes only one content item, a separate playlist isn’t required.

Manage playlists using **📌 Menu → Playlists**.
