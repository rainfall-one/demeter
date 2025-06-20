---
tags: [facet, export, png]
---

# PNG Export Facet

## Library

- **Library Name**: `sharp`
- **Description**: A high-performance image processing library.
- **Compatibility**: Fully compatible with Node.js and TypeScript.
- **Installation**:
  ```bash
  npm install sharp
  ```
- **Usage**:
  ```typescript
  import sharp from 'sharp';
  sharp('input.png')
    .resize(200, 200)
    .toFile('output.png');
  ```

## Features

- Supports image resizing, conversion, and manipulation.
- High-performance and efficient.
- Wide format support.
