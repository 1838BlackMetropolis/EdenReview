# Eden Cemetery — Transcription Validator

A small website for volunteers to check the transcribed burial records against the original scanned
pages, side by side. Pick a page, compare the scan to the records we pulled from it, and mark each one
**✓ Verified** or **✎ Needs fix** (with a correction). Reviewers can export their work as a CSV to send back.

## What's in this folder

- `index.html` — the whole app (data is built in; no server or internet needed).
- `images/` — the scanned pages (`page_01.jpg` … `page_95.jpg`).

## Try it locally first

Double-click `index.html` — it opens in your browser and works offline.

## Publish it free on GitHub Pages

1. Create a new GitHub repository (e.g. `eden-validator`).
2. Upload **`index.html`** and the **`images/`** folder to the repo (drag them into the repo's
   "Add file → Upload files" page, or `git push`).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source: Deploy from a branch**, **Branch: main** (folder `/root`), and Save.
5. Wait a minute, then your site is live at `https://<your-username>.github.io/eden-validator/`.
   Share that link with your reviewers.

Note: GitHub Pages sites are public. That's usually fine for a cemetery project, but anyone with the
link can view it.

## How reviewers send corrections back

Their progress autosaves in their own browser. When they're done (or partway), they click
**⬇ Export review (CSV)** to download a small file listing only the records they marked, with their
notes. They email/share that CSV with you. You can open all the CSVs in Excel to see every correction,
or load one back into the app with **⬆ Import CSV** to keep reviewing.

## Updating the data later

The records come from `Eden_Cemetery_Database.xlsx`. When that's corrected, the site can be rebuilt so
the app always shows the latest transcription.
