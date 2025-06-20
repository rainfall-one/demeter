---
tags: [facet, editor, docs, wysiwyg]
---

# Editor for Documents Facet

## Library

- **Library Name**: `tiptap`
- **Description**: A modern WYSIWYG editor built on ProseMirror.
- **Compatibility**: Fully compatible with Svelte, TypeScript, and JavaScript.
- **Installation**:
  ```bash
  npm install @tiptap/core @tiptap/svelte
  ```
- **Usage**:
  ```typescript
  import { Editor } from '@tiptap/core';
  import StarterKit from '@tiptap/starter-kit';

  const editor = new Editor({
    extensions: [StarterKit],
    content: '<p>Hello, PaperClip!</p>',
  });
  ```

## Features

- Rich text editing with advanced formatting options.
- Extensible with plugins for additional features.
- Lightweight and fast.
