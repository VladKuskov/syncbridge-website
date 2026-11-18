# SyncBridge Core – Project Website (Indy-1, CS 4850 Fall 2026)

Plain HTML + CSS. No JavaScript, no build step.

## Files

| File | What it is |
|---|---|
| `index.html` | Home page (project ID, title, team, course, links) |
| `srs.html` / `sdd.html` | PDF viewer + clickable section index |
| `video.html` | Final presentation video (YouTube embed) |
| `style.css` | All styling (KSU black and gold) |
| `docs/` | The SRS and SDD as PDFs |
| `images/` | Team photos |

## Run it locally

In this folder, run:

```
python3 -m http.server 8000      # macOS / Linux
py -m http.server 8000           # Windows
```

Then open http://localhost:8000. Press Ctrl+C to stop.

(Double-clicking `index.html` also works, except the YouTube video, because YouTube blocks embeds on pages opened as local files.)

## Common edits

- **Real video:** in `video.html`, replace `dQw4w9WgXcQ` (it appears twice) with your YouTube video ID, the part after `watch?v=`.
- **New version of a PDF:** replace the file in `docs/` and keep the same name. If the page numbers changed, update the `#page=N` and `?p=N` numbers in `srs.html` / `sdd.html`.
