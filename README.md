# JSON ↔ TOON Converter

A robust, single-file web application for converting data between **JSON** (JavaScript Object Notation) and **TOON** (a concise, S-expression-like data format).

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Tech: HTML/JS/Tailwind](https://img.shields.io/badge/Tech-HTML%20%7C%20JS%20%7C%20Tailwind-blue.svg)
![Status: Active](https://img.shields.io/badge/Status-Functional-green.svg)

## 📖 What is TOON?

**TOON** is a custom, minimal data serialization format designed to be more human-readable than JSON by removing syntactic noise (commas, colons, and excessive quotes). It borrows syntax concepts from Lisp (S-expressions).

**Key Differences:**

| Feature | JSON | TOON |
| :--- | :--- | :--- |
| **Objects** | `{ "key": "value" }` | `(key "value")` |
| **Arrays** | `[ "a", "b" ]` | `[ "a" "b" ]` |
| **Separators** | Commas `,` required | Whitespace only |
| **Keys** | Must be quoted | Unquoted if alphanumeric |
| **Comments** | Not supported | Supports `# comments` |

### Syntax Comparison

**JSON:**
```json
{
  "name": "Project X",
  "isActive": true,
  "tags": ["dev", "web"],
  "meta": {
    "id": 101
  }
}
```
**TOON:**
```lisp
(
  name "Project X"
  isActive true
  tags [ "dev" "web" ]
  meta (
    id 101
  )
)
```

### Demo
https://swapnilgopale.github.io/json-to-toon-converter/
