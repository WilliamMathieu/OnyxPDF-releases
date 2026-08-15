# Onyx PDF

A small, fast, native PDF reader and annotator for Windows. No installer, no
account, no telemetry — two files in a folder, about 4 MB.

**[Download the latest release →](https://github.com/WilliamMathieu/OnyxPDF-releases/releases/latest)**

Free to use for any purpose, personal or commercial, on as many machines as you
like. See [LICENSE](LICENSE).

---

## What it does

**Read** — multi-page scrolling with momentum, zoom to cursor, fit
width/height/page, page thumbnails, document outline, find, and tabs for
several documents at once.

**Annotate** — highlight, strikethrough, sticky notes, rectangles, ellipses,
lines, free text, and signatures (drawn freehand or from an image). Everything
you place can be selected, moved, resized, restyled or deleted, with undo.

**Review** — attach a comment to a highlight or strikethrough, and open a
column beside the page that lists every note level with the text it marks.

**Fill forms** — type into AcroForm fields, copy out of them, and save.

**Redact** — properly. The covered text is removed from the file, not painted
over, so it cannot be recovered by selecting or extracting.

**Manage pages** — rotate, delete, reorder by dragging, insert blank pages or
pages from another PDF, extract a selection to a new file.

Plus printing with preview, save flattened or compressed, and four themes.

## Installing

Unzip anywhere and run `OnyxPDF.exe`. Keep `pdfium.dll` beside it. There is no
installer, nothing is written to the registry, and no admin rights are needed —
a USB stick works fine. To uninstall, delete the folder (settings live in
`%APPDATA%\onyxprojects`).

**Requirements:** Windows 10 or 11, 64-bit. No Visual C++ redistributable —
the runtime is linked statically.

### "Windows protected your PC"

The download is not code-signed, so SmartScreen warns the first time you run
it. Click **More info**, then **Run anyway**; Windows remembers the choice.

If you would rather check before trusting it, each release lists the SHA-256 of
its zip. Verify with:

```powershell
Get-FileHash OnyxPDF-0.1.0-win-x64.zip -Algorithm SHA256
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
