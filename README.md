# Ten-Level Chinese — Flashcards (Level 1)

A clean, Anki-style flashcard web app for **beginner (Level 1) Chinese**, built
as a companion study tool for students of *拾级汉语 综合课本 第1级* (BLCU Press).
Same engine as the [Level 2 app](https://github.com/PeterVanPercson/chinese-flashcards),
in its own separate site so progress never mixes between levels.

**Lesson 1 — 您贵姓? (May I know your surname?)**
- 29 vocabulary words · 18 example sentences · 20 read-and-write characters
- Native-quality Mandarin audio on every card (one tap to play, or autoplay)
- Stroke-order writing practice (Hanzi Writer) — on characters *and* single-hanzi words
- Beginner option: **Chinese + pinyin on the front** as a reading scaffold

> The vocabulary and characters are the lesson's factual word list. The example
> sentences are **original**, written to drill the lesson's grammar — they are
> not the textbook's dialogues.

## Features
Flip cards (Chinese → pinyin + English), Again/Hard/Good/Easy grading with simple
spaced repetition, search, "Due / Weakest / Random" quick-study, dark mode,
adjustable card size, audio autoplay toggle, progress export/import, installable
PWA with offline support. All progress lives in your browser only.

## Run locally
Serve the folder over http (file:// blocks `fetch`):
```
python3 -m http.server 8000
```
then open http://localhost:8000.

## Files
```
index.html              app shell (home / study views, dialogs)
assets/app.js           hash router, deck builder, SRS, audio, search, writer
assets/styles.css       paper-aesthetic design system + dark mode
sw.js                   service worker (offline; L1-specific cache namespace)
manifest.json           PWA manifest
data/lessons.json       Lesson 1 content (vocab / sentences / characters)
assets/audio/           58 Mandarin clips + manifest.json (1:1 coverage)
assets/icons/           PWA icons
```

Built by [Husan Mavlonov](https://husanmavlonov.com).
