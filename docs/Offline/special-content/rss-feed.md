---
title: RSS Feed Display
sidebar_position: 2
---

You can configure **RSS feed display** in _Bharat Signage_ by creating a new content item of type **“RSS messages”** and adding it to your playlist. For a quicker setup, you may also use the predefined **"With side panels"** layout as a starting template.

## RSS Source Options

In the RSS content configuration, use the **“URL for RSS messages”** field to specify where the messages will be loaded from. You can choose one or more of the following types:

- **Online feed:** Enter the direct URL to the RSS XML file, for example:  
  `http://feeds.bbci.co.uk/news/rss.xml`
- **Local file:** Use the filename (e.g., `news.rss`) if it's been uploaded or transferred to the Bharat Signage device. It's recommended to use the `.rss` file extension.

- **Manual messages:** Enter `"local"` (without quotes) to use messages manually added via the web interface under  
  `Tools → RSS Messages`.

Multiple sources can be combined using a comma (`,`). Messages from all sources will play sequentially in a loop.

## Optional Settings

- **Remove unwanted tags:** If your RSS contains HTML/XML tags (e.g., `&nbsp;` or `<img ...>`), enable the **“Remove XML tags”** option in the Edit Content screen to clean them from display.

- **Test RSS file:** You can use this `Sample RSS Feed` to test your setup. It contains two simple example messages.

```xml
<?xml version="1.0" encoding="utf-8"?>
<rss version="2.0">
  <channel>
    <item>
      <title>Title of the first message</title>
      <description>This is first sample message for Bharat Signage application.</description>
    </item>
    <item>
      <title>Title of the second message</title>
      <description>This is another message, which can be used for testing. Feel free to edit the file.</description>
    </item>
  </channel>
</rss>
```

Save this XML content as `sample.rss` and upload it to your Bharat Signage device to see how it works.

- **Cloud Hosting:** If you're planning to host your RSS file online, services like [rss-hosting.com](https://www.rss-hosting.com) are suitable.

## Format Details

RSS is a plain-text **XML-based format**, making it easy to edit using any text editor. You can find format references on [Wikipedia](https://en.wikipedia.org/wiki/RSS) or [W3Schools](https://www.w3schools.com/xml/xml_rss.asp).

Bharat Signage reads the following tags from each RSS item:

- `<title>` → Displayed in **bold**
- `<description>`, `<summary>`, or `<content>` → Displayed in **regular font**

## Tools for Creating RSS Files

To author RSS files manually or with additional features, you can use:

- Basic text editors (Notepad, VS Code, etc.)
- GUI-based tools like **RSS Builder**

---

This setup allows your screens to dynamically show live updates, news, alerts, or custom messages — all synchronized with your playlist and layouts in Bharat Signage.
