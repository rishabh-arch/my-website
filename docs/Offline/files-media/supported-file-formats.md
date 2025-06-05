---
id: supported-file-formats
title: Supported File Types and Codecs
sidebar_position: 1
---

# Supported File Types and Codecs

Below is the list of file types, formats, and codecs supported by the current version of **Bharat Signage** software.

## Image

| **Type** | **File Extensions**                                               | **Supported Formats**                                             | **Notes**                                                                                                                                                                                                                                                                         |
| -------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Image    | `jpg`, `jpeg`, `png`, `bmp`, `gif`, `webp`, `svg`, `heic`, `heif` | JPEG, PNG, Bitmap, GIF, WebP, SVG, HEIC/HEIF (only on Android 9+) | See [Android image format support](https://developer.android.com/guide/topics/media/media-formats#image-formats).\\Images with resolution more than twice the size of the display zone are scaled down to save memory.\\Animated GIFs and WebPs are supported only on Android 9+. |

## Video

| **Type** | **File Extensions**                                                                               | **Supported Formats**                | **Notes**                                                                  |
| -------- | ------------------------------------------------------------------------------------------------- | ------------------------------------ | -------------------------------------------------------------------------- |
| Video    | `mpg`, `mpeg`, `avi`, `mp4`, `3gp`, `mkv`, `ts`, `flv`, `f4v`, `webm`, `wmv`, `m2v`, `m4v`, `mov` | Usually MPEG-2, MPEG-4, H.264, H.265 | Codec and bitrate support depends on the device hardware and manufacturer. |

## Audio

| **Type** | **File Extensions**                       | **Supported Formats**                  | **Notes**                                                                                                       |
| -------- | ----------------------------------------- | -------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| Audio    | `aac`, `flac`, `mp3`, `wav`, `ogg`, `mid` | AAC, FLAC, MP3, PCM/WAVE, Vorbis, MIDI | See [Android audio codec support](https://developer.android.com/guide/topics/media/media-formats#audio-codecs). |

## PDF

| **Type** | **File Extensions** | **Supported Formats** | **Notes**                                                                                                       |
| -------- | ------------------- | --------------------- | --------------------------------------------------------------------------------------------------------------- |
| PDF      | `pdf`               | –                     | Depending on the “Display PDF as scrollable” setting, pages may appear as one long scroll or one after another. |

## HTML

| **Type** | **File Extensions**    | **Supported Formats** | **Notes**                                                                            |
| -------- | ---------------------- | --------------------- | ------------------------------------------------------------------------------------ |
| HTML     | `html`, `htm`, `xhtml` | –                     | Supported HTML/CSS/JavaScript features depend on the Android System WebView version. |

## Excel

| **Type** | **File Extensions** | **Supported Formats**               | **Notes**                                                                                |
| -------- | ------------------- | ----------------------------------- | ---------------------------------------------------------------------------------------- |
| Excel    | `xls`, `xlsx`       | Excel 97–2003, Excel 2007 and newer | Table styling can be customized via: **Settings → Device settings → CSS style for XLS**. |

## Webpage Link

| **Type**     | **File Extensions** | **Supported Formats** | **Notes**                                                                                                                                                         |
| ------------ | ------------------- | --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Webpage Link | `url`               | –                     | URL shortcut file or plain text file with a single-line web address.\\Only successfully loaded pages are displayed.\\Rendering depends on Android System WebView. |

## Text

| **Type** | **File Extensions** | **Supported Formats** | **Notes**                           |
| -------- | ------------------- | --------------------- | ----------------------------------- |
| Text     | `txt`               | Plain text (UTF-8)    | Used for displaying as moving text. |

## RSS

| **Type** | **File Extensions** | **Supported Formats** | **Notes**                  |
| -------- | ------------------- | --------------------- | -------------------------- |
| RSS      | `rss`, `xml`        | RSS, Atom             | Must be in UTF-8 encoding. |

## Stream

| **Type** | **File Extensions** | **Supported Formats**             | **Notes**                                 |
| -------- | ------------------- | --------------------------------- | ----------------------------------------- |
| Stream   | –                   | HTTP/HTTPS/RTSP/RTMP live streams | Codec support depends on device hardware. |

## Archive

| **Type** | **File Extensions** | **Supported Formats**                    | **Notes**                                                                                                |
| -------- | ------------------- | ---------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| Archive  | `zip`, `tar`, `ar`  | ZIP (Store, Deflate, Deflate64), TAR, AR | Used for downloading/synchronizing multiple files.\\Archive files are unpacked immediately after upload. |

## Google Docs

| **Type**    | **File Extensions** | **Supported Formats**       | **Notes**                                                                                                                                   |
| ----------- | ------------------- | --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Google Docs | –                   | Google Docs, Sheets, Slides | Automatically converted to PDF when downloaded from Google Drive.\\Conversion settings can be adjusted in **Google Docs convert settings**. |

---

### ⚠️ Important Notes

- Bharat Signage distinguishes file types **only by file name extension**.
- File extensions are **case-insensitive** (`.jpg` = `.JPG`).
- If a file isn't displayed, make sure its extension is listed in the table above.
