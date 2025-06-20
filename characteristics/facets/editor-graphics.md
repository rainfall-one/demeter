---
tags: [facet, editor, graphics, wysiwyg]
---

# Editor for Graphics Facet

## Library

- **Library Name**: `fabric.js`
- **Description**: A powerful JavaScript library for vector and raster graphics editing.
- **Compatibility**: Fully compatible with Svelte, TypeScript, and JavaScript.
- **Installation**:
  ```bash
  npm install fabric
  ```
- **Usage**:
  ```typescript
  import { fabric } from 'fabric';

  const canvas = new fabric.Canvas('c');
  const rect = new fabric.Rect({
    left: 100,
    top: 100,
    fill: 'red',
    width: 50,
    height: 50,
  });
  canvas.add(rect);
  ```

## Features

- Supports layers, effects, and interactive graphics editing.
- Extensible with plugins for additional features.
- Lightweight and fast.
