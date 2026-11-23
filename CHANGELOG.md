# Changelog

The section for a version becomes the "What's new" text of its release and of the in-app update notice.
Keep entries short and written for users.

## 0.1.0

The first test build of Pixolotl, for Windows only. It is an early build: much of the application works,
some of it is not built yet, and no designer has used it for real work so far. Please keep copies of
anything important and report what goes wrong.

What you can do today:

- **Draw and edit vectors.** Rectangles, ellipses, polygons, stars, lines and arcs that stay editable; the
  Pen, Pencil, Paintbrush and Width tools; anchor editing with typed coordinates; Shape Builder, Pathfinder
  and live boolean shapes; Offset Path, Outline Stroke, Simplify, Knife, Scissors and Eraser; dashes,
  arrowheads and variable-width strokes.
- **Lay out pages.** Several artboards, rulers, guides, rectangular and isometric grids, snapping and smart
  guides. Every field takes typed numbers, units and arithmetic.
- **Work in colour and for print.** RGB, CMYK, grayscale, Lab and spot colours with ICC colour management;
  CMYK documents, soft proofing, gamut warning and overprint preview; swatches, linear, radial and conic
  gradients, patterns, blend modes, opacity masks and clipping masks.
- **Set type.** Point type, area type in any shape and type on a path; character and paragraph controls,
  tabs, OpenType features, variable fonts, character and paragraph styles; Arabic, Hebrew, Devanagari,
  Thai, Chinese, Japanese and Korean text; colour fonts; Create Outlines.
- **Import and export.** Opens Pixolotl documents, SVG, PDF, Illustrator files saved with PDF content, PNG,
  JPEG, TIFF and WebP, and ASE, ACO and GPL swatches. Exports SVG, PDF (CMYK, spot colours, bleed, crop
  marks and a preflight check), PNG, JPEG, TIFF and WebP, with a live preview and the exact file size.
  Every import lists anything it could not bring in. `pixolotl --export` converts files from the command
  line.
- **Edit pixels.** Pixel layers next to vector layers in one document; marquee, lasso, polygonal lasso,
  magic wand and colour range selections with feather, grow, shrink and quick mask; saved selections;
  raster masks; crop; and painting with the Brush, Eraser, Smudge, Clone Stamp, Paint Bucket and Gradient,
  with a Brushes panel, pressure and tilt dynamics and a stabilizer.
- **Never lose work.** Unlimited undo with a History panel, safe saving, and automatic recovery of unsaved
  work after a crash.
- **Choose how it looks.** Dark and light themes and interface text from 100% to 200%.
- **Stay up to date.** Pixolotl checks for a new version when it starts (you can turn this off in
  Help > About Pixolotl) and on Help > Check for Updates. Updates are signed and installed only when you say so.

Not built yet:

- Adjustments, filters, layer effects and retouching tools.
- Photoshop (PSD) and GIMP (XCF) files, and brush imports.
- Live effects, symbols, and EPS and DXF export.
- Saved workspaces and preferences (only the update setting is remembered), and a shortcut editor.
- macOS and Linux versions.

Known limits: the Windows installer is not code-signed, so Windows SmartScreen warns the first time you
run it. Illustrator and PDF import have been tested on open-source sample files; text in a font you do not
have installed is drawn in a substitute font.
