---
sidebar_position: 6
---

# Scheduled File Deletion

**Bharat Signage** allows you to schedule automatic file deletion based on date and time. This helps keep your internal storage clean and organized.

---

## ⏲️ How It Works

The system **periodically checks** file deletion dates and automatically removes files once their **scheduled time** has passed.

- ✅ Interval can be configured from:
  **Menu → Settings → Device settings → How often to check files**
- ⏰ File deletion relies on the **device’s system time** — ensure it's correctly set.

---

## 📌 Methods to Schedule File Deletion

### 1. Via File Manager (Web Interface)

You can set a deletion schedule directly from the **File Manager**:

- Go to **Menu → Files → File manager**
- **Right-click** a file → **Select "Schedule deletion"**
- Choose the desired **date and time**

To view the deletion schedule:

- Right-click the file → **Get info**
- Or, switch to **List view** and check the **"Delete date"** column

---

### 2. Via `setup.csv` File

When uploading files through:

- 📁 ZIP Archive
- 💾 USB Flash Drive
- ☁️ Google Drive or Dropbox

You can set the deletion schedule in the **`setup.csv`** file included in the upload.

---

### 3. Via File Name Format

Upload a file using a specific naming pattern, and Bharat Signage will automatically detect and assign a deletion schedule.

**Format:**

`{name}DEL{date}.{extension}`

**Supported Date Formats:**

| Format             | Example                          | Description                      |
| ------------------ | -------------------------------- | -------------------------------- |
| `yyyy-MM-dd`       | `image_DEL_2020-11-22.jpg`       | Delete on specific date          |
| `yyyy-MM-dd HH:mm` | `video_DEL_2020-11-22 21:00.mp4` | Delete on specific date and time |
| `dd.MM.yyyy`       | `banner_DEL_22.11.2020.jpg`      | Alternate date format            |
| `dd.MM.yyyy HH:mm` | `doc_DEL_07.12.2019 13:20.pdf`   | Alternate full format            |
| `xxD`              | `temp_DEL_7D.pdf`                | Delete after X days from upload  |
| `xxH`              | `alert_DEL_5H.png`               | Delete after X hours from upload |

⚠️ **Note:**  
File name is parsed **only when first uploaded**.  
Renaming the file later will **not** update the deletion schedule.  
To modify the date afterward, use the **File Manager**.
