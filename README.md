# DevCodec

> Six everyday encode/decode tools — Base64, URL, JWT, hex, HTML entities, timestamps — on one page.

**[Live demo](https://su-devcodec.vercel.app)**

Decoding a JWT or Base64 string usually means reaching for whichever random site ranks first that day and pasting a token into it. DevCodec puts the six conversions developers reach for most into a single tabbed page that runs entirely client-side, so nothing you paste is transmitted anywhere. Each tool is a bidirectional pair of fields: edit either side and the other updates as you type, with invalid input handled rather than throwing.

## Features

- **Base64** — encode and decode, bidirectional as you type
- **URL** — percent-encode and decode
- **JWT** — decode a token into its header, payload, and signature, using Base64URL decoding (no verification; decode only)
- **Hex** — convert between plain strings and hex
- **HTML entities** — escape and unescape
- **Timestamp** — Unix seconds to human-readable UTC, local time, and a relative description ("3 hours ago"), with a Now button and a copy button on every field

## Stack

- Vanilla JavaScript — a single `index.html` with no framework or runtime dependencies
- Vite as the dev server and build tool
- Built on native browser APIs — `btoa`/`atob`, `encodeURIComponent`, `TextEncoder`/`TextDecoder`, and `toLocaleString` — with no external libraries

## Running locally

```bash
npm install
npm run dev
```

---

Part of a series of 91 small web apps. [Browse them all](https://su-slopmachine.vercel.app).
