# Kaghaz PDF Viewer

**A privacy-first PDF reader for highlighting, drawing, and notes.**

Kaghaz is a browser-based PDF annotation workspace. It opens PDFs locally, keeps annotations in the browser, and exports an annotated PDF without sending documents to an application server.

## Features

- Open a PDF from the device or drag and drop it into the reader
- Render PDF pages in the browser with PDF.js
- Persian and Arabic friendly right-to-left interface
- Highlight by drawing a rectangle over a passage
- Freehand pen and drawing tool
- Add Persian, Arabic, or English notes at any page position
- Select and move any annotation
- Change annotation color and pen width
- Edit note text
- Delete one annotation or use the eraser
- Undo and redo
- Zoom, fit page, and page navigation
- Save and restore annotation projects as JSON
- Export a marked-up PDF
- Switch PDF font rendering modes for difficult embedded fonts
- Open the original PDF in the browser's native viewer
- Responsive layout for desktop and mobile screens

## Privacy

PDF files are processed locally in the browser. They are not uploaded to a backend. PDF.js and pdf-lib are loaded from public CDNs, so the first run needs an internet connection.

## Run locally

```bash
git clone https://github.com/DataMahmood/PDF-viewer.git
cd PDF-viewer
python -m http.server 8000
```

Open `http://localhost:8000` in a modern browser.

## GitHub Pages

This repository is a static site and can be published from the `main` branch root in **Settings → Pages**. The site address is:

https://datamahmood.github.io/PDF-viewer/

## Annotation workflow

1. Open a PDF.
2. Choose **هایلایت** and draw a rectangle over the required text.
3. Choose **قلم** to draw.
4. Choose **یادداشت** and click on the page.
5. Choose **ویرایش علامت** to move, recolor, edit, or delete an annotation.
6. Use **دریافت PDF** to export the annotated document.

## Browser support

A current Chromium-based browser is recommended. Firefox and Safari can run the core reader, but PDF font rendering and file download behavior may vary by browser.

## License

MIT. See `LICENSE`.