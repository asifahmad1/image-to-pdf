# Image to PDF Generator — Convert Photos to PDF

Turn your photos into one clean PDF — **100% in your browser**. No uploads, no sign-up, no server: your images never leave your device.

**▶ Live on Asif SaaS Studio:** open the tools catalogue and choose *Image to PDF Generator* (slug `image-to-pdf`).

## What it does
1. **Add images** — up to 50 (PNG, JPEG, WebP, BMP, GIF or AVIF, ≤ 25 MB each) by drag-and-drop or browsing, in one or several batches.
2. **Arrange** — each image becomes one PDF page, in the order shown; reorder with ↑ ↓, remove with ✕.
3. **Set the page** — A4, Letter or Fit-to-image; orientation Auto / Portrait / Landscape; margins 0–25 mm; image quality 60–100; custom file name.
4. **Download** — a genuine PDF 1.4 document, assembled on your device by a small PDF engine written into the page (JPEG image streams, exact cross-reference table, title metadata). Transparency is flattened onto white.

Inputs are validated in plain language — wrong types, empty and corrupt files, oversize files and the 50-image cap each get a named, specific message.

## Use
Open `index.html` in any modern browser — or from this repo via any static host. No build step, no dependencies.

- Single file, **22.9 KB**, all CSS/JavaScript inline
- No localStorage, no service workers, no browser permissions, no parent-window access — safe in a sandboxed iframe
- Responsive layout in the Asif SaaS Studio emerald + lime branding

## Testing
25/25 automated tests passed (Node.js, executed against the shipped file's own PDF-engine core): page geometry, validation, and PDF structure — including exact cross-reference offsets — plus independent verification of a generated PDF with poppler (2 pages, correct sizes, metadata, renders cleanly). Full report: `image-to-pdf-test-report.md`. Complete documentation: `docs/image-to-pdf-docs.pdf`.

Created by Dr. Asif Ahmad · Asif SaaS Studio · v1.0
