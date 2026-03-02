# VS Code LaTeX Settings

Preconfigured `settings.json` for **VS Code + LaTeX Workshop** to make LaTeX projects compile reliably with:

* Automatic `biber` support (`biblatex`)
* Dedicated `build/` directory for auxiliary files
* Clean PDF generation workflow

This repository exists primarily so I can sync my own LaTeX configuration across machines.

---

## What This Config Does

* Uses `latexmk` (recommended) or structured recipe workflow
* Runs `biber` automatically for `biblatex`
* Sends `.aux`, `.bcf`, `.bbl`, etc. to a `build/` directory
* Reduces manual compile steps

---

## Installation Guide

### 1️⃣ Install Required VS Code Extensions

From the VS Code Marketplace:

* **LaTeX Workshop** by James Yu
  [https://github.com/James-Yu/LaTeX-Workshop](https://github.com/James-Yu/LaTeX-Workshop)

* **LaTeX Utilities** by tecosaur *(optional, but useful for Zotero integration)*
  [https://github.com/tecosaur/LaTeX-Utilities](https://github.com/tecosaur/LaTeX-Utilities)

---

### 2️⃣ Install LaTeX Distribution

Make sure you have a full LaTeX distribution installed:

* **TeX Live** (Linux/macOS)
* **MiKTeX** (Windows)
* Ensure `pdflatex`, `latexmk`, and `biber` are available in your PATH.

Verify with:

```
pdflatex --version
biber --version
latexmk --version
```

---

### 3️⃣ Add the Settings File

Copy the provided `settings.json` into:

* **Workspace settings** (recommended):

  ```
  .vscode/settings.json
  ```

* OR your global VS Code user settings.

After that, LaTeX builds should:

* Use `biber` automatically
* Place auxiliary files in `build/`
* Generate PDFs without manual intervention

---

## Why This Exists

This repo is mainly a personal configuration backup so I can quickly reproduce my LaTeX setup on new machines.

If it works for you, great. If not, treat it as a starting point.

