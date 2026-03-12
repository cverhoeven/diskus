# Diskus

<p align="center">
  <img src="logo.png" alt="Diskus Logo" width="140" />
</p>

<p align="center">
  <strong>Cross-platform disk analyzer</strong> · Windows app, Mac & Linux coming soon
</p>

<p align="center">
  <a href="https://diskus-app.com/">diskus-app.com</a>
</p>

<p align="center">
  Visualize your disk usage with interactive sunburst diagrams.<br>
  Find large folders, search within directories, and move files to the trash with precision.<br>
  Filters, settings, and localization (DE/EN).
</p>

---

## Why I built Diskus

I was always looking for a **clean, easy-to-use** way to find what’s eating my disk space – without the clutter of old-school tools and without the dull experience of most analyzers. So I built Diskus: a tool that makes it **fun to explore your storage**, with clear visuals, smooth interactions, and a focus on great UX. Finding storage hogs should feel straightforward and even a bit enjoyable ❤️

---

<p align="center">
  <a href="https://github.com/cverhoeven/diskus/releases/latest"><img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download" /></a>
  <img src="https://img.shields.io/badge/platform-Windows-lightgrey?style=flat-square" alt="Platform" />
  <img src="https://img.shields.io/badge/macOS%20%26%20Linux-coming%20soon-orange?style=flat-square" alt="Coming soon" />
  <img src="https://img.shields.io/badge/license-Proprietary-red?style=flat-square" alt="License" />
</p>

---

## Download

**Find all releases on GitHub:**

👉 **[View & download releases](https://github.com/cverhoeven/diskus/releases)**

| Platform | Status | Format |
|----------|--------|--------|
| **Windows** | ✅ Available | Installer (.exe) or Portable (.exe) |
| **macOS** | 🔜 Coming soon | — |
| **Linux** | 🔜 Coming soon | — |

> The first scan of a large drive may take a few seconds.

---

## Tip

**Feel free to leave me a tip, if you like Diskus <3**

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/B0B11VPEWW)

## Features

- **Drive overview** – All scannable drives (hard disks, SSDs, USB) in tile or list view; capacity bars (yellow/red at 80%/95%)
- **Onboarding** – Short intro tour on first start (welcome, features, support); repeatable via the sparkles icon on the intro screen
- **Sunburst diagram** – Interactive rings by folder size; click to drill down, breadcrumbs and center to go back
- **File list** – Resizable list of the current folder with sizes; sort by name or size
- **Search** – Filter the current folder by name in real time (toggle via search icon)
- **Settings** – Min file size, hide hidden files, sunburst depth/limits, list colors, trash undo duration; saved for next scan
- **Trash collector** – Collect items via context menu or drag & drop, then move all to system trash in one go; optional short-time undo
- **Context menu** – Show in Explorer, open file / Quick Look (macOS), add to trash collector
- **Language** – German and English; switch on the intro screen

---

## User Guide

### 1. Start – Choose a drive

On first start, a short **onboarding** (welcome, features, support) is shown. You can run it again anytime via the sparkles icon on the intro screen.

On the intro screen you see all available drives in **tile or list view**. Click a drive to start the scan.

- **Tile / list view** – Switch via the layout icon; preference is saved
- **Capacity bar** – Yellow at 80%, red at 95% usage
- **USB sticks** – Highlighted with a distinct icon
- **Reload** – Refresh the drive list

### 2. Disk view – Explore the sunburst

- **Click a segment** – Zoom into the folder
- **Breadcrumb at top** – Navigate back to parent folders
- **File list** – Resizable list of the current folder; sort by name or size
- **Search** – Click the search icon to show/hide the filter field; type to filter the current folder
- **Switch drive** – Dropdown in the header
- **Settings** – Filters (min size, hidden files), sunburst depth/limits, list colors, trash undo duration

### 3. Remove files

- **Right-click** on file/folder → **Add to trash collector** (or open in Explorer / Quick Look). You can also **drag & drop** items into the trash collector.
- **Trash collector** – Collect several items (context menu or drag & drop), then move all to the system trash in one action
- **Short-time undo** – Restore items after moving (duration configurable in settings)

> Files go to the **system trash** and can be recovered until you empty it.

### 4. Open in Explorer & Quick Look

- **Right-click** → **Show in Explorer** – Opens the folder in Windows Explorer (or Finder on macOS).
- **Double-click a file** – Opens with the default app (Windows) or Quick Look (macOS).

---

## Tech Stack

| Area | Technology | Notes |
|------|------------|-------|
| **Desktop** | Electron 41 | Main process, IPC, shell commands |
| **Frontend** | Angular 21 | Clean UI/UX |
| **Visualization** | D3.js | Sunburst, Partition layout, arc segments |
| **Icons** | Lucide (lucide-angular) | — |
| **i18n** | Transloco (@jsverse/transloco) | DE/EN, language switch in runtime |
| **Language** | TypeScript 5.9, RxJS 7 | — |

---

## License

Proprietary. All rights reserved © Carlo Verhoeven

---

<p align="center">
  Made with ✨ & ❤️ in cologne
</p>
