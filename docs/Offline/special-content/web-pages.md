---
title: Displaying Web Pages
description: Learn how Bharat Signage displays websites and HTML content using the WebView component.
sidebar_position: 1
---

**Bharat Signage** offers the flexibility to show live websites, dashboards, and even custom HTML content directly on your screen using Android’s **WebView** component. This enables seamless integration of online resources such as charts, news feeds, and more — right into your digital signage setup.

---

## ⚙️ WebView Engine and Updates

The rendering engine used for displaying web pages is Android's **WebView**, which functions like a lightweight browser embedded inside Bharat Signage.

- 📲 **Updatable independently** from the app and Android OS.
- 🔄 Keep it **updated via Google Play** (Android System WebView or Chrome).
- 🔧 You can switch the WebView provider from:
  > `Developer Options → WebView implementation`

---

## 🧾 Customizing the User-Agent

The **User-Agent** string used in HTTP requests can be configured:

- 🧠 Default: Automatically uses the best string based on the WebView version.
- ✏️ Optional: Customize it in the app settings under `User agent for HTTP requests`.

This is useful when you want web servers to serve specific content for Bharat Signage devices.

---

## 🌍 Showing a Website via `.url` Files

Bharat Signage can render full websites by detecting `.url` files in your content folder. These files contain the web address of the site to be displayed.

### ✅ Supported Formats

- A **plain text file** with a single line:  
  `https://example.com`
- A `.url` file **created or edited via Bharat Signage File Manager**.
- `.url` file **generated on Windows**.

> 🔗 The device must have **internet access** to load external websites.

---

## 🔐 Password-Protected Websites

Two methods are supported for loading secured pages:

1. **HTTP Basic Authentication**  
   Include credentials in the URL:  
   `https://username:password@domain.com`

   > Make sure special characters are **URL-encoded**.

2. **Login Form Authentication**  
   Use the `Enter web page` editor in File Manager:
   - Click `Scan page`, enter login details, then click `Save`.
   - ⚠️ Compatibility may vary depending on the site's login implementation.

---

## 🌐 Domain Restrictions

You can **restrict allowable domains** using the “Available domains” field in the `Enter web page` editor:

- Leave empty to allow **all** domains.
- Specify one or more domains (comma-separated) to restrict redirects.
- Subdomains are automatically included.
- External assets like **JavaScript, fonts, and CSS** are **not restricted**.

---

## 🧱 Displaying `.html` Files

You can also serve **custom HTML content**:

- Upload `.html` files to your device.
- Supports **HTML5**, **JavaScript**, **iframes**, and **CSS** (based on WebView version).
- Transparent background by default – to show overlays.

To set a solid background:

```html
<body style="background-color: white"></body>
```

## ✍️ Edit HTML in the Web Interface

You can edit HTML files directly in the Bharat Signage web interface:

- WYSIWYG (CKEditor) – Visual HTML editing
- Plain Text (TextArea)

Go to `File Manager → Right click on an HTML file → Edit file.`

## 💡 Example: Twitter Feed Widget

You can use HTML widgets such as Twitter timelines, weather feeds, etc. Below is an example of embedding a Twitter feed:

Example `twitter.html`

```html
<html>
  <style>
    body,
    html {
      margin: 0;
    }
  </style>
  <body>
    <a
      class="twitter-timeline"
      data-lang="en"
      data-width="960"
      data-height="1080"
      data-theme="dark"
      href="https://twitter.com/BharatSignage?ref_src=twsrc%5Etfw"
    >
      Tweets by BharatSignage
    </a>
    <script
      async
      src="https://platform.twitter.com/widgets.js"
      charset="utf-8"
    ></script>
  </body>
</html>
```

Save this file and add it to your layout. The Twitter feed will be live and interactive on your signage screen!
