# Onyx PDF

A small, fast, native PDF reader and annotator for Windows. No account, no
telemetry, about 4 MB — install it, or run it from a folder.

**[Download the latest release →](https://github.com/WilliamMathieu/OnyxPDF-releases/releases/latest)**

Free to use for any purpose, personal or commercial, on as many machines as you
like. See [LICENSE](LICENSE).

---

## What it does

**Read** — smooth multi-page scrolling, zoom to cursor, fit
width/height/page, two-page spread, page thumbnails, document outline, find,
clickable links, and tabs for several documents at once. Open documents come
back the next time you start.

**Annotate** — highlight, strikethrough, sticky notes, rectangles, ellipses,
lines, free text, and signatures (drawn freehand or from an image). Everything
you place can be selected, moved, resized, restyled or deleted, with undo.

**Review** — attach a comment to a highlight or strikethrough, and open a
column beside the page that lists every note level with the text it marks.
Resolve comments as you deal with them, or delete them.

**Fill forms** — type into AcroForm fields, copy out of them, and save.

**Redact** — properly. The covered text is removed from the file, not painted
over, so it cannot be recovered by selecting or extracting.

**Manage pages** — rotate, delete, reorder by dragging, insert blank pages or
pages from another PDF, extract a selection to a new file.

**Recover** — unsaved changes are kept in the background, and offered back if
the app ever closes unexpectedly.

Plus printing with preview, save flattened or compressed, recent files, four
themes, and a Settings window — down to the look of the pan cursor.

## Installing

Each release comes two ways:

- **`OnyxPDF-<version>-setup.exe`** — an installer with a Start-menu shortcut,
  an optional "Open with" entry for PDFs, and an uninstaller under Settings →
  Apps. No admin rights needed.
- **`OnyxPDF-<version>-win-x64.zip`** — portable. Unzip anywhere and run
  `OnyxPDF.exe`, keeping `pdfium.dll` beside it. Nothing is written to the
  registry and a USB stick works fine. To uninstall, delete the folder.

Settings live in `%APPDATA%\onyxprojects` either way.

**Requirements:** Windows 10 or 11, 64-bit. No Visual C++ redistributable —
the runtime is linked statically.

### "Windows protected your PC"

The download is not code-signed, so SmartScreen warns the first time you run
it. Click **More info**, then **Run anyway**; Windows remembers the choice.

If you would rather check before trusting it, each release lists the SHA-256 of
its files. Verify with:

```powershell
Get-FileHash OnyxPDF-0.2.1-setup.exe -Algorithm SHA256
```

## Built on

[PDFium](https://pdfium.googlesource.com/pdfium/) for rendering, forms and
annotations (BSD 3-Clause), [FLTK](https://www.fltk.org/) for the interface
(LGPL v2 with a static-linking exception), and
[stb](https://github.com/nothings/stb) for image decoding (public domain).
Full notices are in the app under **Help → Third-Party Libraries**.

## Reporting a problem

Open an [issue](https://github.com/WilliamMathieu/OnyxPDF-releases/issues) —
what you did, what happened, and the PDF if you can share it.

This repository holds releases only; the source is not published.
