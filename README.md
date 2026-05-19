# IWES LaTeX Templates

Official LaTeX templates from the **Institute of Wind Energy Systems (IWES)**,
Leibniz University Hannover.

## Templates

| Thesis (English) | Thesis (Deutsch) | Presentation | Poster | Gantt Chart |
|:---:|:---:|:---:|:---:|:---:|
| [![thesis-english](thesis-english/preview.png)](../../releases/latest/download/thesis-english.zip) | [![thesis-german](thesis-german/preview.png)](../../releases/latest/download/thesis-german.zip) | [![beamer](beamer/preview.png)](../../releases/latest/download/beamer.zip) | [![poster](poster/preview.png)](../../releases/latest/download/poster.zip) | [![gannt](gannt/preview.png)](../../releases/latest/download/gannt.zip) |
| [thesis-english.zip](../../releases/latest/download/thesis-english.zip) | [thesis-german.zip](../../releases/latest/download/thesis-german.zip) | [beamer.zip](../../releases/latest/download/beamer.zip) | [poster.zip](../../releases/latest/download/poster.zip) | [gannt.zip](../../releases/latest/download/gannt.zip) |

## Getting Started

We recommend using the **[LUH Overleaf service](https://tex.cloud.uni-hannover.de/saml/login)**
(login with your LUH account).

1. Download the zip for the template you need (links above)
2. In Overleaf: **New Project → Upload Project** → upload the zip
3. That's it — everything is ready to compile

Further instructions and usage notes are provided directly inside the template files.

## Building locally

All templates require **LuaLaTeX** (recommended) or XeLaTeX.

| Template | Command |
|---|---|
| thesis-english | `cd thesis-english && lualatex 00_main && biber 00_main && lualatex 00_main && lualatex 00_main` |
| thesis-german | `cd thesis-german && lualatex 00_main && biber 00_main && lualatex 00_main && lualatex 00_main` |
| beamer | `cd beamer && lualatex 00_main` |
| poster | `cd poster && lualatex 01_content` |
| gannt | `cd gannt && lualatex gantt_template` |

The thesis templates need three LuaLaTeX passes (plus one Biber pass) to resolve cross-references and the bibliography.

## Fonts

Templates can use **Rotis Sans Serif Std** (commercial license, not included).
The template compiles fine without it using a fallback font.
If you have the fonts, place the `.otf` files in the `font/` or `Rotis/` folder — see `FONTS.md` there.
Rotis requires a Unicode-aware compiler: **LuaLaTeX** or **XeLaTeX** (not pdflatex).

## License

Template code: [MIT](LICENSE) · Logos: property of LUH / IWES · Fonts: not included
