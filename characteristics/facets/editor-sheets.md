---
tags: [facet, editor, sheets, wysiwyg]
---

# Editor for Spreadsheets Facet

## Library

- **Library Name**: `handsontable`
- **Description**: A JavaScript library for creating interactive spreadsheets.
- **Compatibility**: Fully compatible with Svelte, TypeScript, and JavaScript.
- **Installation**:
  ```bash
  npm install handsontable
  ```
- **Usage**:
  ```typescript
  import Handsontable from 'handsontable';

  const container = document.getElementById('example');
  const hot = new Handsontable(container, {
    data: [
      ['Name', 'Value'],
      ['PaperClip', 42],
    ],
    colHeaders: true,
    rowHeaders: true,
  });
  ```

## Features

- Supports formulas, charts, and data manipulation.
- Extensible with plugins for additional features.
- Lightweight and fast.
