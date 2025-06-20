---
tags: [facet, export, pdf]
---

# PDF Export Facet

## Library

- **Library Name**: `pdf-lib`
- **Description**: A library for creating and modifying PDF documents.
- **Compatibility**: Fully compatible with Node.js and TypeScript.
- **Installation**:
  ```bash
  npm install pdf-lib
  ```
- **Usage**:
  ```typescript
  import { PDFDocument } from 'pdf-lib';
  const pdfDoc = await PDFDocument.create();
  const page = pdfDoc.addPage([600, 400]);
  page.drawText('Hello, PaperClip!');
  const pdfBytes = await pdfDoc.save();
  ```

## Features

- Create and modify PDF documents.
- Supports embedding images and fonts.
- Lightweight and fast.
