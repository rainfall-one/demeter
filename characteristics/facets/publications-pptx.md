---
tags: [facet, export, pptx]
---

# PowerPoint Export Facet

## Library

- **Library Name**: `pptxgenjs`
- **Description**: A library for creating PowerPoint presentations programmatically.
- **Compatibility**: Fully compatible with Node.js and TypeScript.
- **Installation**:
  ```bash
  npm install pptxgenjs
  ```
- **Usage**:
  ```typescript
  import PptxGenJS from 'pptxgenjs';
  const pptx = new PptxGenJS();
  const slide = pptx.addSlide();
  slide.addText('Hello, PaperClip!', { x: 1, y: 1, fontSize: 18 });
  pptx.writeFile('output.pptx');
  ```

## Features

- Create PowerPoint presentations programmatically.
- Supports text, images, and charts.
- Lightweight and fast.
