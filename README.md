# IWES LaTeX Templates

Official LaTeX templates from the **Institute of Wind Energy Systems (IWES)**,  
Leibniz University Hannover (LUH).

---

## Available Templates

| Template | Description | Main file |
|---|---|---|
| [thesis-english](thesis-english/) | Master's / Doctoral thesis (English) | `00_main.tex` |
| [thesis-german](thesis-german/) | Master's / Doctoral thesis (German) | `00_main.tex` |
| [beamer](beamer/) | Presentation slides (Beamer) | `00_main.tex` |
| [poster](poster/) | Scientific poster (A0 format) | `00_template.tex` |

---

## Quick Start

### Option A — Overleaf (recommended)

1. Go to the [Releases](../../releases/latest) page and download the desired `.zip`
2. In Overleaf: **New Project → Upload Project** → select the zip
3. Set the main file (`00_main.tex` or `00_template.tex` for poster) and compile

### Option B — Local installation

```bash
git clone git@github.com:IWES-LUH/IWES-Templates.git
cd IWES-Templates/thesis-english   # or whichever template
```

Compile with:

```bash
pdflatex 00_main.tex
biber 00_main
pdflatex 00_main.tex
pdflatex 00_main.tex
```

Or use a LaTeX IDE (TeXstudio, VS Code + LaTeX Workshop) that handles this automatically.

---

## Fonts — Rotis Sans Serif

The templates are designed for **Rotis Sans Serif Std** (commercially licensed).  
The fonts are **not included** in this repository.

- See the `FONTS.md` in each template's `font/` or `Rotis/` folder for instructions
- Templates will compile with a fallback font (Latin Modern) if Rotis is absent
- Layout and spacing will match the intended design only when the fonts are installed

---

## Repository Structure

```
IWES-Templates/
├── thesis-english/     English thesis template
│   ├── font/           Place Rotis .otf files here (see FONTS.md)
│   └── figures/        Logos and example figures
├── thesis-german/      German thesis template (Abschlussarbeit)
│   ├── font/
│   └── figures/
├── beamer/             Presentation template
│   └── Rotis/          Place Rotis .otf files here (see FONTS.md)
├── poster/             A0 scientific poster template
│   └── Rotis/          Place Rotis .otf files here (see FONTS.md)
└── .github/workflows/  Auto-release GitHub Action
```

---

## Releases

A new release is automatically created on every push to `main`.  
Each template is packaged as a separate `.zip` ready for Overleaf:

| File | Contents |
|---|---|
| `thesis-english.zip` | English thesis template |
| `thesis-german.zip` | German thesis template |
| `beamer.zip` | Beamer presentation template |
| `poster.zip` | A0 poster template |

---

## License

- Template structure and code: [MIT License](LICENSE)
- Logos (LUH, IWES): property of their respective institutions
- Rotis Sans Serif fonts: not included, subject to separate commercial licensing
