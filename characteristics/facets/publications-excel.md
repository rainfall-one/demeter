---
tags: [facet, export, excel]
---

# Excel Export Facet

## Library

- **Library Name**: `exceljs`
- **Description**: A library for reading, writing, and manipulating Excel files.
- **Compatibility**: Fully compatible with Node.js and TypeScript.
- **Installation**:
  ```bash
  npm install exceljs
  ```
- **Usage**:
  ```typescript
  import ExcelJS from 'exceljs';
  const workbook = new ExcelJS.Workbook();
  const sheet = workbook.addWorksheet('PaperClip Data');
  sheet.addRow(['Name', 'Value']);
  sheet.addRow(['PaperClip', 42]);
  await workbook.xlsx.writeFile('output.xlsx');
  ```

## Features

- Supports reading and writing Excel files.
- Allows styling and formatting of cells.
- Lightweight and fast.
