# SheetHound — downloads

*(formerly Millwork Submittal Support)*

Windows desktop app that turns construction schedules into submittal packages:

- **Reads schedules** (hardware, plumbing, equipment, appliance, material, finish) from PDFs or images using Google Gemini's free tier.
- **Finds spec sheets** in this order: your own saved sheets, the manufacturer website, then distributor copies (build.com, fergusonhome.com, …). When a sheet can't be downloaded automatically, each item gets a link: click it, pick the PDF on the manufacturer's site, and it's attached. As a last resort, and only when you ask, it generates an AI summary sheet clearly flagged for verification.
- **Exports** one stapled PDF with bookmarks and a tag stamp on every page, or individual stamped PDFs.

## Install

1. Open **[Releases](../../releases)** and download `SheetHound-Setup-<version>.exe` from the newest release (versions up to 0.1.0-alpha.5 were named `MillworkSubmittalSupport-Setup-<version>.exe`).
2. Run it. The installer isn't code-signed yet, so Windows may show **"Windows protected your PC"**. Click **More info → Run anyway**.
3. Start the app, open **Settings → AI**, and paste a free Gemini API key from <https://aistudio.google.com/apikey>.

## Updates

The app checks this page at startup and every few hours. From 0.1.0-alpha.6 on, new versions download in the background and install themselves when the app is idle: SheetHound restarts, reopens your work, and shows *Updated to vX* in the status bar. To be asked first, untick **Settings → Updates → Install updates automatically**.
SheetHound is now in **beta** (from 0.2.0-beta.1). Alpha installs (`0.1.0-alpha.x`) update to the beta by themselves, and beta installs receive later betas and full releases, never an older alpha. Copies of *Millwork Submittal Support* update to SheetHound like any other version, keeping their settings, API key and spec library.

## Beta notice

SheetHound is feature-complete for day-to-day use and still being refined. Check every spec sheet before submitting, especially sheets marked **AI – verify**.
To report a problem, open an [issue](../../issues) with a screenshot and the schedule type you were reading.

---
This repository only hosts installers. The source code is kept private.
