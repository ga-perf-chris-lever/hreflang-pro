# Hreflang Pro

**The all-in-one hreflang cluster health checker for Chrome.**

Hreflang Pro scans any webpage for hreflang annotations, fetches every page in the cluster, validates the entire set, and tells you exactly what's broken and how to fix it — all from a single click.

![Chrome Extension](https://img.shields.io/badge/Chrome-Extension-4285F4?logo=googlechrome&logoColor=white)
![Manifest V3](https://img.shields.io/badge/Manifest-V3-34A853)
![License](https://img.shields.io/badge/License-Proprietary-orange)

---

## What Is It For?

International SEO relies on hreflang tags to tell search engines which language and regional version of a page to show each user. Getting these tags wrong — missing return links, invalid codes, canonical conflicts — can cause the wrong page to rank or no page at all.

Hreflang Pro automates the entire audit process. Instead of manually checking every tag across every page, the extension builds a complete picture of your hreflang cluster in seconds.

![Screenshot](https://raw.githubusercontent.com/free-whiteboard-online/Free-Erasorio-Alternative-for-Collaborative-Design/1c38beeaa2c7579c0b06643c1c98d3a2327c3c2b/uploads/2026-03-09T20-43-40-176Z-od8379nwm.png)

---

## Key Feature: Cluster Matrix

The **Cluster Matrix** is the centrepiece of Hreflang Pro. It's a visual grid showing every page in your hreflang cluster and whether each page correctly references every other page.

- **Green dots** — Confirmed bidirectional link
- **Red dots** — Missing return tag (the target page doesn't link back)
- **Gold dots** — Self-referencing tag

At a glance, you can see exactly where your hreflang implementation breaks down. The matrix can be exported as a **PNG image** for reports and client deliverables.

![Whiteboard Screenshot](https://raw.githubusercontent.com/free-whiteboard-online/Free-Erasorio-Alternative-for-Collaborative-Design/9cc942d306b450b987e47cd1233d8e301d0e3656/uploads/2026-03-09T20-45-25-896Z-q3jprr4ns.png)
---

## How to Use

1. Navigate to any webpage you want to audit
2. Click the **Hreflang Pro** icon in your browser toolbar
3. The extension automatically scans the page and fetches all linked language versions
4. Review the **Cluster Health Score**, **Cluster Matrix**, **Issues**, and **Page Details**
5. Use **Export CSV** for a full actionable audit or **Export Matrix** for a visual snapshot

---

## Features

### Detection & Scanning
- **Multi-source detection** — Finds hreflang tags in HTML `<link>` tags, HTTP `Link` headers, and XML sitemaps
- **Full cluster crawl** — Fetches every page referenced in the hreflang set to verify return tags
- **Response time tracking** — Measures how long each page in the cluster takes to respond
- **Redirect detection** — Identifies pages that redirect (including geo-redirect detection)
- **Sitemap cross-referencing** — Checks if the XML sitemap contains matching hreflang entries

### Validation & Scoring
- **Cluster Health Score** (0–100) — Weighted score based on issue count and severity
- **16 validation checks** including:
  - Invalid hreflang codes (with ISO 639-1 / ISO 3166-1 validation)
  - Common typo detection (e.g. `en-uk` → `en-gb`)
  - Missing self-referencing tags
  - Missing return tags (broken bidirectional links)
  - Duplicate hreflang values
  - Canonical URL mismatches
  - `<html lang>` mismatches
  - Content-Language header mismatches
  - Noindex + hreflang conflicts
  - Inconsistent tag counts across pages
  - x-default validation (missing, redirecting, outside cluster)
  - Relative URL detection
  - Hreflang tags placed outside `<head>`
  - Mixed HTTP/HTTPS schemes
  - Sitemap vs HTML conflicts
  - Geo-redirect detection (distinguishes geo-redirects from real redirects)
- **Smart issue prioritisation** — Issues ranked by severity and impact, with "Fix This First" guidance

### Visual & Export
- **Cluster Matrix** — Interactive grid showing the full link graph between all language versions
- **Export Matrix as PNG** — Dark-themed visual export with flag icons, ideal for reports
- **Export CSV** — Detailed per-issue action list with fix instructions
- **Copy Fix Code** — One-click copy of corrected hreflang markup for any page

### UI & Usability
- **Flag emoji icons** — Visual country/language flags via Twemoji for cross-platform support
- **Dark mode** — Toggle with the header button or press `D`
- **Pop-out to full tab** — Expand the popup into a full browser tab for larger clusters
- **Keyboard shortcuts**:
  - `R` — Re-scan the current page
  - `D` — Toggle dark mode
  - `C` — Export CSV
  - `X` — Export Matrix as PNG
- **Detection source badges** — See at a glance whether hreflang was found in HTML, HTTP headers, or sitemap

---

## Installation (Developer Mode)

Hreflang Pro is not yet on the Chrome Web Store. To install it locally:

1. Download or clone this repository
2. Open Chrome and go to `chrome://extensions/`
3. Enable **Developer mode** (toggle in the top-right corner)
4. Click **Load unpacked**
5. Select the `hreflang-pro` folder
6. The Hreflang Pro icon will appear in your browser toolbar — click it on any page to start scanning

> **Tip:** Pin the extension to your toolbar for quick access — click the puzzle piece icon in Chrome and pin Hreflang Pro.

---

## Built By

**Chris Lever** — Head of Technical SEO at [Glass Atlas](https://www.glassatlas.com)

Planning to submit to the Chrome Web Store after extensive testing. If you encounter any bugs or have feedback, message me on [LinkedIn](https://www.linkedin.com/in/chris-lever-seo/).
