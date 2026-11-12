<div align="center">

# MORVEX

### WALLPAPERS

**Make your screen feel alive.**

A sleek, lightweight Android experience for discovering, downloading, and applying animated video wallpapers.

<br />

![Platform](https://img.shields.io/badge/Platform-Android-10151D?style=for-the-badge&logo=android&logoColor=3DDC84)
![Kotlin](https://img.shields.io/badge/Kotlin-Planned-10151D?style=for-the-badge&logo=kotlin&logoColor=AA78FF)
![Status](https://img.shields.io/badge/Status-In%20Development-10151D?style=for-the-badge&logo=github&logoColor=white)
![License](https://img.shields.io/badge/License-Not%20Specified-10151D?style=for-the-badge)

<br />

**[Overview](#-overview) · [Features](#-planned-features) · [Architecture](#-architecture) · [Getting Started](#-getting-started)**

</div>

---

## ✦ Overview

**Morvex Wallpapers** is an Android live-wallpaper project focused on motion, atmosphere, and simplicity. Browse a curated collection of animated backgrounds, preview your favorites, and download only the wallpapers you want.

The goal is a smooth, distraction-free experience with a remotely updated catalog and offline access to downloaded wallpapers.

> **Project status:** Early development. The features and architecture below describe the current plan and may change.

## ✧ Planned Features

| | Feature | Description |
|:--:|---|---|
| ◈ | **Video wallpapers** | Bring your home screen to life with looping video backgrounds. |
| ⌕ | **Discover & search** | Browse wallpapers by category, style, and keywords. |
| ▣ | **Instant previews** | Explore a lightweight visual catalog before downloading. |
| ↓ | **On-demand downloads** | Keep the APK small by downloading videos separately. |
| ♡ | **Favorites** | Save your preferred wallpapers for easy access. |
| ◌ | **Offline playback** | Use previously downloaded wallpapers without an internet connection. |
| ↻ | **Fresh content** | Receive new catalog entries without reinstalling the app. |

## ⌘ Architecture

```text
                  MORVEX WALLPAPERS
                         │
                Android Application
                 Kotlin + Compose
                         │
              ┌──────────┴──────────┐
              │                     │
         Catalog API          Local Storage
         (static JSON)        (downloaded MP4)
              │                     │
        GitHub Pages         WallpaperService
              │                     │
       Wallpaper metadata      Live wallpaper
              │
        GitHub Releases
          Video files
```

**Proposed stack**

- **Android:** Kotlin, Jetpack Compose, Material 3
- **Playback:** AndroidX Media3 and Android `WallpaperService`
- **Networking:** OkHttp
- **Local data:** Room
- **Images:** Coil
- **Distribution:** GitHub Releases (APK and video assets)
- **Catalog:** Static JSON hosted on GitHub Pages

This architecture is intended for a small, personal distribution. Hosting limits and acceptable-use policies should be reviewed before scaling.

## ◇ Getting Started

Morvex is not yet available as a stable build.

Once an APK is published:

1. Open the repository's **Releases** section.
2. Download the latest Android APK.
3. Install it on your Android device.
4. Browse, download, and apply your favorite wallpaper.

> Only install APKs from sources you trust. Android may ask you to allow installation from your chosen browser or file manager.

## ▤ Repository Structure (Planned)

```text
morvex-wallpapers/
├── app/                 # Android application
├── catalog/             # Wallpaper metadata
├── scripts/             # Asset processing and catalog tools
├── docs/                # Project documentation
└── README.md
```

## ◈ Design Principles

**Minimal by default.** Content takes center stage, not interface clutter.

**Performance matters.** Efficient previews, local caching, and careful video playback.

**No unnecessary accounts.** Browse and download without signing up.

**Built to evolve.** A remotely maintained library that can grow independently of the APK.

## ⚖ License & Content

No software license has been specified yet. Unless a license is added, the source code is not automatically granted open-source reuse permissions.

Wallpaper media remains subject to the rights and licenses of its respective creators. Only content with appropriate distribution rights should be included.

---

<div align="center">

### MORVEX / WALLPAPERS

*Less static. More alive.*

<sub>Designed for Android · Currently in development</sub>

</div>
