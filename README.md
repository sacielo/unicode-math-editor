# unicode-math-editor
A lightweight, browser-based editor for writing math using real Unicode characters.

[Live Demo](https://sacielo.github.io/unicode-math-editor/)

---

## Why

Most online math editors either produce LaTeX (which requires a renderer) or use "fake" superscripts and subscripts — Unicode lookalikes that break when you paste them into a terminal, code comment, chat message, or plain text document.

This editor only outputs real Unicode codepoints. What you copy is what you get, everywhere.

## Features

- **Real sub/superscripts** — ₐ ₁ ² ⁿ are proper Unicode, not styled HTML
- **500+ symbols** across categories: Superscripts, Subscripts, Operators, Vectors, Physics, and more
- **Keyboard shortcuts** — select any text, then `Ctrl+↑` to superscript or `Ctrl+↓` to subscript
- **Symbol search** — find symbols by name (`integral`, `theta`, `implies`, `partial`, …)
- **Zero dependencies** — single HTML file, works offline, no install

## Usage

Open `index.html` in any browser. No server, no build step.

```
e₀ = mc²         →  e₀ = mc²
∀ε > 0 ∃δ > 0   →  ∀ε > 0 ∃δ > 0
f: ℝⁿ → ℝ        →  f: ℝⁿ → ℝ
```

## Keyboard shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl+↑` (or `Cmd+↑`) | Toggle normal text and superscript |
| `Ctrl+↓` (or `Cmd+↓`) | Toggle normal text and subscript |
| `Ctrl+Z` | Undo |
| `Ctrl+B` | Toggle normal text and boldface (when in Unicode) |
| `Ctrl+I` | Toggle normal text and italics (when in Unicode) |

## Limitations

Unicode only defines superscript/subscript glyphs for a subset of characters. Digits (0–9), common letters, and arithmetic signs are covered. Characters without a Unicode equivalent are left unchanged during conversion.

## License

Apache 2.0
