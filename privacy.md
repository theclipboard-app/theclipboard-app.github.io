---
title: TheClipboard — Privacy Policy
---

# TheClipboard — Privacy Policy

*Effective 14 November 2026* · [Česky](soukromi)

**In short:** everything TheClipboard saves stays on your computer. The developer receives none of it. There is no account, no cloud, no advertising and no analytics. The only thing the app ever sends over the network is the domain name of a website, to fetch that site's icon — described below.

## What the app reads

TheClipboard has two jobs, and each needs to read something:

- **Clipboard history.** When you copy something, the app keeps a copy: text, images and other clipboard content.
- **Automatic saving of text fields.** While you type in a text field in another application, the app saves the field's text so it can be recovered if the window closes or crashes. It reads the text through **Windows UI Automation**, the accessibility interface Windows provides for this purpose.

With each saved item the app also stores where it came from: the application's name and program path, the window title, the field's label, and — for web browsers — the address of the page.

## What the app does not read

- **No keystroke capture.** The app does not install keyboard hooks and does not record individual key presses. It reads only the text a field itself makes available.
- **Password fields are never read.** Fields that Windows marks as password fields are skipped entirely.
- **Short text is not saved.** Text below a minimum length (adjustable in the app) is ignored.
- **Blocked applications** you choose are never watched, and automatic saving can be paused or switched off at any time.

## Where your data is stored

Everything is stored on your computer, in your Windows user profile, in the folder `%LOCALAPPDATA%\CLIPBOARD`. This includes the database of saved items, stored images, local backups, website icons, settings, diagnostic logs and crash reports.

The database is not encrypted by the app; it is protected by your Windows user account like your other files. You can lock the library with **Windows Hello**, and the app's windows are hidden from screenshots, screen recording and screen sharing. These protect what is shown on screen; they do not protect the files from other programs running under your account.

## What leaves your computer

**Website icons.** The first time a website appears in your history, the app requests that site's icon from DuckDuckGo's public icon service (`icons.duckduckgo.com`). The request contains only the **domain name** — for example `example.com` — never the page address, the text, or anything else. Each domain is requested once; the icon is then kept on your computer. DuckDuckGo's handling of these requests is covered by [DuckDuckGo's privacy policy](https://duckduckgo.com/privacy).

**Nothing else.** The app does not send your clipboard history, your saved text, usage statistics or crash reports anywhere. If the app crashes, a report is written to your computer only; it is sent to the developer only if you choose to send it yourself.

## Your control

- Delete individual items, whole folders, or everything, from within the app.
- Pause or switch off automatic saving, change the minimum length, and block applications.
- **Uninstalling the app does not delete your data folder.** To remove everything, delete the folder `%LOCALAPPDATA%\CLIPBOARD` after uninstalling.

## Children

The app is a general-purpose productivity tool and is not directed at children.

## Changes

If this policy changes, the new version will be published at this address with a new date. Earlier versions remain in the public history of this site.

## Contact

Questions about privacy: [kafka.enterprise@gmail.com](mailto:kafka.enterprise@gmail.com)
