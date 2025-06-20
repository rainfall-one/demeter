---
tags: [facet, export, docx]
---

# DOCX Export Facet

## Library

- **Library Name**: `docxtemplater`
- **Description**: A library for creating DOCX files programmatically.
- **Compatibility**: Fully compatible with Node.js and TypeScript.
- **Installation**:
  ```bash
  npm install docxtemplater
  ```
- **Usage**:
  ```typescript
  import Docxtemplater from 'docxtemplater';
  import PizZip from 'pizzip';
  const zip = new PizZip();
  const doc = new Docxtemplater(zip);
  doc.setData({ name: 'PaperClip' });
  doc.render();
  const buffer = doc.getZip().generate({ type: 'nodebuffer' });
  ```

## Features

- Template-based DOCX generation.
- Supports dynamic content insertion.
- Easy integration with existing workflows.
