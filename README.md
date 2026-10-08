# StepFun 5 · 100 HTML Files

One hundred self-contained single-file HTML pages. Every page carries its CSS,
JavaScript and prompt inline — **no CDN, no web fonts, no images, no libraries**.
Open any of them offline by double-clicking.

`index.html` is the gallery: one card per page with a live screenshot, a link to the
page, and the exact prompt that produced it. Each page has a matching `.txt`
companion holding that prompt plus its design note.

## layout

```
index.html             the gallery
001-….html … 100-….html the 100 pages
001-….txt  … 100-….txt  the 100 prompt/design notes
shots/                 one JPEG screenshot per page
```

## verified

- 100 pages, 100 companion `.txt` files, continuous numbering, no orphans
- every page opened in a real browser with no uncaught script error and no failed request
- no external references of any kind (`src=`/`href=` to a host, `<script src=`, `@import`, `fetch`, `XMLHttpRequest`)
- every page carries a viewport meta and responsive CSS; no page overflows its viewport
- every page's script proven to have run by diffing the live DOM against the source
