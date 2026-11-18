# ALDA Librarian — Pixel installable PWA (experimental)

This package creates an ALDA icon on your Android home screen *when hosted on a stable HTTPS origin*. Do not open index.html from a Google Drive preview or a file:// download and expect a browser install prompt.

## Before install
1. Keep all five files together (index.html, manifest.webmanifest, sw.js, icon-192.png, icon-512.png); icon.svg is optional.
2. Host on a stable HTTPS origin you control, without adding private files to the website. A GitHub Pages repository would make the app shell publicly viewable; that requires Francine's authorization.
3. On Pixel, open the HTTPS URL in Chrome. Chrome ⋮ → Add to Home screen → Install (or Create shortcut if Install not offered). Confirm ALDA Librarian icon appears. Never assume install succeeded until the icon launches the same app origin.
4. Import a **fictional** text file, search for its contents, add notes, close the app completely, reopen from the icon, and verify the same file and notes persist. Then export a backup and confirm restore. Do not use sensitive files until this real-device acceptance passes.

## What it can do
Import chosen local files (≤15 MB each), organize into folders, search content of supported text files, add tags and notes, download original, and JSON backup+restore.

## Important limitations
Browser IndexedDB data can be cleared by users, browsers or storage pressure. Always export backups. No cloud sync, encryption, PDFs/DOCX full-text indexing, unsupervised folder access, background AI agents or production-grade tamper-evidence. PWA installability requires HTTPS and browser/platform support. This package was NOT deployed on Francine's phone; the icon is not yet verified on the phone.
