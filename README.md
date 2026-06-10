# AKC ANUV — landing page

Static, single-page landing site for AKC ANUV. No build step, no dependencies —
just open `index.html` (or serve the folder) and it runs.

## Structure

```
index.html                              Landing page
assets/
  logo.png                              AKC ANUV logo (title-block mark)
  gaudi-mark.html                       GAUDI animated mark (embedded in the GAUDI box)
drawings/                               Engineering drawings the hero cycles through
  pier-cap.html                         Pier cap CP-774
  span-cross-section.html               56 m span — cross-section
  bridge-general-arrangement.html       Dhari Jhora bridge — general arrangement
icons/
  favicon.svg                           Favicon (scalable)
  favicon-32.png                        Favicon fallback (32×32)
  apple-touch-icon.png                  Apple touch icon (180×180)
```

The hero embeds the three drawings in an `<iframe>` and cycles through them.
Each drawing is self-contained (geometry data is inlined). Fonts load from Google Fonts.

## Run locally

Any static server works, e.g.:

```
python3 -m http.server 8000
# then open http://localhost:8000
```

Opening `index.html` directly via `file://` also works in most browsers.

## External links

- Studio  → https://studio.akcanuv.com
- GAUDI   → https://gaudi.engineer
