# Required Fonts

This template uses **Rotis Sans Serif Std** by Albert-Jan Pool / Adobe.
These fonts are **not included** because they are commercially licensed and cannot be redistributed.

## Required font files

Place the following `.otf` files in this folder:

| File | Variant |
|---|---|
| `RotisSansSerifStd-Regular.otf` | Regular |
| `RotisSansSerifStd-Bold.otf` | Bold |
| `RotisSansSerifStd-ExtraBold.otf` | Extra Bold |
| `RotisSansSerifStd-Light.otf` | Light |
| `RotisSansSerifStd-Italic.otf` | Italic |
| `RotisSansSerifStd-LightIt.otf` | Light Italic |

## Compiler requirement

Rotis fonts are OpenType (`.otf`) files and require a Unicode-aware compiler.
You **must** use **LuaLaTeX** or **XeLaTeX** — `pdflatex` cannot load these fonts.

In Overleaf: go to **Menu → Compiler** and select **LuaLaTeX** or **XeLaTeX**.

## Without fonts

The template will compile and fall back to a standard font (Latin Modern).
The layout and spacing will differ slightly from the intended design.
