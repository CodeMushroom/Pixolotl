# Changelog

The section for a version becomes the "What's new" text of its release and of the in-app update notice.
Keep entries short and written for users.

## 0.2.0

Adjustments, filters, layer effects, retouching, Photoshop and GIMP files, and Image Trace.

- **Adjustment layers.** Effect > New Adjustment Layer adds Levels, Curves, Hue/Saturation,
  Brightness/Contrast, Color Balance, Black & White, Exposure, Vibrance, Selective Color, Channel Mixer,
  Invert, Threshold, Gradient Map, or Shadows/Highlights above the selected layer, with a mask (made from
  your selection, if you have one). Paint the mask to limit it; clip it to the layer below with one button.
- **Adjustments, filters, and layer effects on any layer.** Effect > Adjustments, Blur, Sharpen, Noise, and
  Layer Effects add them to the selected layer, shape, text, or group. They stay editable: turn each off
  and on with its eye, drag it to change the order, delete it, or reset it. On a pixel layer, Apply makes
  them part of the pixels.
- **An editor for every adjustment**, in Properties: Levels and Curves over a histogram of the picture,
  Hue/Saturation with its six color ranges, Color Balance, Selective Color, Channel Mixer, Gradient Map,
  and the rest. The picture changes as you drag, and each drag is one step to undo.
- **Layer Style.** Drop shadow, inner shadow, outer and inner glow, stroke, color and gradient overlay, and
  bevel and emboss, with Photoshop's settings, in the Properties panel.
- **Filters with a dialog.** Effect > Blur > Gaussian Blur…, Sharpen > Unsharp Mask…, and Noise > Add
  Noise… show the filter live while you set it, and can change the pixels for good if you ask.
- **Photoshop and GIMP files.** Open, place, or drop PSD, PSB, and XCF files, with their layers, groups,
  masks, adjustment layers, and layer styles. If something could not be kept, the report says what, and
  can open the file flattened instead.
- **Export to Photoshop.** Choose PSD in the Export panel (or `--format psd` on the command line), with
  adjustment layers kept editable or applied.
- **SVG and PDF keep the look of effects.** Layers with adjustments, filters, or effects are written as
  pictures, and the export report says which.
- **Image Trace** (Object > Image Trace…) turns a picture into filled paths in black and white, gray
  steps, or colors, with a live preview on the canvas. In gray and color, Ignore White leaves white areas
  out, so they stay transparent.
- **Import brushes** from Photoshop (ABR) and GIMP (GBR, GIH) brush files in the Brushes panel, or by
  dropping the file on the window. They are kept for next time.
- **Retouching tools**: the Spot Healing Brush, Healing Brush, and Patch tool (J), Dodge, Burn, and Sponge
  (O), and Blur and Sharpen, in the Paintbrush button's group. Healing blends in the background with its
  progress and a Cancel button in the status bar.
- **Free Transform** (Edit > Free Transform, Ctrl+T with a pixel layer selected) for pixel layers and
  selected pixels: drag the handles or type position, size, angle, and skew; Distort, Perspective, and
  Warp with a mesh. Enter applies it as one step, Esc cancels.
- **Select > Refine Edge…** refines a selection around hair and soft edges, with a live preview, into the
  selection or a layer mask.
- **Edit > Fill From Surroundings** replaces the selected pixels with texture from around them, in the
  background.
- **Copy, Paste, and Clear Layer Style** in the Effect menu and the Layers panel's context menu.
- **Effect colors use the color picker.** Clicking a layer effect's color opens the color picker; a drag
  in it is one step to undo.
- The status bar says when the canvas shows a quick preview of a large blur while you drag.
- **The selection's marching ants march again**, smoothly, as in Photoshop. They stop while the window
  is minimized and while you paint.

Known limits in this version:

- A glow, shadow, or stroke that reaches more than about 100 pixels on screen takes several seconds to
  draw the first time and after each zoom.
- Dragging a layer effect setting in a document with twenty or more styled layers can drop slightly below
  60 frames a second.
- Layer effects blend inside their own layer, so a glow set to Screen can look different from Photoshop,
  and the picture stored inside an exported PSD does not include effects (the layers do).
- Very large blurs show a quick preview while you drag and take longer to finish.
- Pixel layers in CMYK are not drawn yet.
- While a selection is active, the marching ants use about a quarter of one processor core.
- Image Trace can cut the sharp tips of thin spikes short and can lose lines thinner than about 1.5 pixels.
- Fill opacity, pattern overlays, Satin, and smart object sources in Photoshop files are not kept; the
  import report says so.
- In this version a feedback report is still saved as a file for you to pass on.

## 0.1.2

- **Edit > Paste in Back (Ctrl+B)** pastes right behind the selection, in the same place it was copied
  from, or at the back of the layer when nothing is selected.
- **Object > Lock > Others (Ctrl+Alt+Shift+2)** and **Object > Hide > Others (Ctrl+Alt+Shift+3)** lock or
  hide everything except what you have selected, in one step you can undo.
- **Object > Path > Average… (Ctrl+Alt+J)** lines up the selected anchor points horizontally, vertically,
  or moves them to one point, also on shapes.
- **Delete a segment with Direct Selection.** Click a segment to select just that segment (it is drawn
  thicker), Shift-click for more, then press Delete: the path opens there or splits in two.
- **Tool tooltips name the tool the button shows.** A button that holds several tools now describes the one
  it shows, with its key, and then how to open the others.
- **The Selection tool shows the move pointer** over a selected object.
- **The brush outline follows the pointer exactly.** For the painting tools, the outline of the brush is now
  the system pointer itself, up to a large size, so it no longer trails behind when you move quickly.

## 0.1.1

Fixes for the first things a tester found, and a way to tell us what goes wrong.

- **Direct Selection now works on shapes.** Rectangles, ellipses, polygons, stars and lines show their
  anchor points as soon as you select or hover them, and you can drag anchors, handles and segments
  straight away. Before, the tool ignored every shape made with the shape tools.
- **The pointer no longer lags or doubles.** Tool pointers (Direct Selection, Pen, Lasso, Type and others)
  are now real system cursors. Before, they were drawn a frame late and a second arrow could appear
  beside them after a click.
- **Pen tablets:** hovering with a pen now moves highlights and the pointer; before, they only moved on a
  press.
- **The Pen, Scissors, Pencil and anchor tools work on shapes too**, and Direct Selection and the Lasso can
  select text, images and pixel layers.
- **Tools say why nothing happened.** Clicking a locked object, or using a tool on something it cannot
  edit, now explains what to do in the status bar.
- **Snapping shows what it snapped to** ("anchor", "edge", "guide" and so on), and pulls a little less
  eagerly.
- **Anchors and handles are as easy to hit as they look** at every text size.
- **Help > Send Feedback.** Write what happened and save a report with a screenshot of the Pixolotl
  window, details of your computer, and your last actions, each of which you can leave out. You can see
  exactly what the report contains. Nothing is sent on its own. In this version the report is saved as a
  file for you to pass on.

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
