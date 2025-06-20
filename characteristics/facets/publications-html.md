---
tags: [facet, export, html]
---

# HTML Export Facet

## Library

- **Library Name**: `jsdom`
- **Description**: A JavaScript implementation of the DOM and HTML standards.
- **Compatibility**: Fully compatible with Node.js and TypeScript.
- **Installation**:
  ```bash
  npm install jsdom
  ```
- **Usage**:
  ```typescript
  import { JSDOM } from 'jsdom';
  const dom = new JSDOM('<!DOCTYPE html><p>Hello, world!</p>');
  console.log(dom.window.document.querySelector('p').textContent);
  ```

## Features

- Allows manipulation and generation of HTML documents.
- Supports server-side rendering.
- Lightweight and fast.
