---
tags: [facet, export, markdown]
---

# Markdown Export Facet

## Library

- **Library Name**: `markdown-it`
- **Description**: A popular Markdown parser and renderer for Node.js.
- **Compatibility**: Fully compatible with Node.js and TypeScript.
- **Installation**:
  ```bash
  npm install markdown-it
  ```
- **Usage**:
  ```typescript
  import MarkdownIt from 'markdown-it';
  const md = new MarkdownIt();
  const result = md.render('# Markdown Example');
  ```

## Features

- Supports rendering Markdown to HTML.
- Extensible with plugins for additional features.
- Lightweight and fast.
