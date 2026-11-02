# Millwork Submittal Support — downloads

Windows desktop app that turns construction schedules into submittal packages:

- **Reads schedules** (hardware, plumbing, equipment, appliance, material, finish) from PDFs or images using Google Gemini's free tier.
- **Finds spec sheets** in this order: manufacturer website, then distributor copies (build.com, fergusonhome.com, …). As a last resort, and only when you ask, it generates an AI summary sheet clearly flagged for verification.
- **Exports** one stapled PDF with bookmarks and a tag stamp on every page, or individual stamped PDFs.

## Install

1. Open **[Releases](../../releases)** and download `MillworkSubmittalSupport-Setup-<version>.exe` from the newest release.
2. Run it. The installer isn't code-signed yet, so Windows may show **"Windows protected your PC"**. Click **More info → Run anyway**.
3. Start the app, open **Settings → AI**, and paste a free Gemini API key from <https://aistudio.google.com/apikey>.

## Updates

Each time the app starts, it checks this page for a newer version and asks before installing it.
Alpha builds (versions like `0.1.0-alpha.1`) also receive newer alpha builds.

## Alpha notice

This is early software. Check every spec sheet before submitting, especially sheets marked **AI – verify**.
To report a problem, open an [issue](../../issues) with a screenshot and the schedule type you were reading.

---
This repository only hosts installers. The source code is kept private.
