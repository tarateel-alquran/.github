<p align="center">
  <img src="https://raw.githubusercontent.com/tarateel-alquran/.github/main/assets/org-header.png" alt="Tarateel AlQuran — ترتيل القرآن" width="100%">
</p>

<h1 align="center">Tarateel AlQuran · ترتيل القرآن</h1>

<p align="center">
  <em>Listen to the Quran, beautifully — 270+ reciters, offline downloads, playlists, and Siri, in English and Arabic.</em>
</p>

---

## What this is

**Tarateel AlQuran** is a Quran listening experience: stream or download recitations from more than 270 reciters across the major rewayat, build playlists, keep favorites, and control playback from the Lock Screen, Control Center, and Siri — fully localized in Arabic and English with first-class RTL support.

This organization is home to the product's whole ecosystem, rebuilt from the ground up on a modern stack:

| Repo | What it is |
|---|---|
| **[quran-api](https://github.com/tarateel-alquran/quran-api)** | High-performance Go backend (Fiber) serving the unified bilingual reciter catalog, suras, and portraits — OpenAPI 3.1, Docker, Cloud Run-ready. |
| *QuranKits* · coming | The Swift package collection powering the apps: nine layered kits (playback engine, downloads, playlists, design system, Siri intents, UI) consumable by any host app — full app or embedded mini app — on iOS, iPadOS, and macOS. |

## How it fits together

```
┌─────────────────────────────┐        ┌──────────────────────────────┐
│  QuranKits (Swift packages) │  ←──→  │  quran-api (Go · Cloud Run)  │
│  iOS · iPadOS · macOS       │        │  unified catalog · portraits │
│  full app + mini app modes  │        │  OpenAPI 3.1 · local-first   │
└─────────────────────────────┘        └──────────────────────────────┘
        streams audio from mp3quran.net's reciter library
```

The apps launch instantly from bundled data and refresh **local-first** from the API: content updates reach users without app releases, and the bundle remains the permanent offline safety net.

## Principles

- **Reverence in the details** — validated Arabic wording, proper RTL, and a design language drawn from the tradition it serves.
- **Fast is a feature** — instant launch, precomputed responses, offline-first everywhere.
- **One codebase, many surfaces** — the same packages ship the full app, an embeddable mini app, and native macOS.

---

<p align="center">
  Audio library by <a href="https://mp3quran.net">mp3quran.net</a> · Original app by FarouK
  <br><br>
  <em>اذكرونا بدعوة عن ظهر غيب</em>
</p>
