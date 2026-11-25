# Changelog

The section for a version becomes the "What's new" text of its release and of the in-app update notice.
Keep entries short and written for users.

## 0.3.2

- **Panels that fold away, as in Illustrator.** The double arrow at the top of the panels (or Window >
  Collapse Panels to Icons) folds them into a narrow column of icons and names. Click a row and its panel
  opens beside the column; click it again or press Escape and it tucks away. Drag the column narrower for
  icons only. Panels you open from the Window menu join the column.
- **Workspaces.** Window > Workspace saves your panel layout under a name, switches between layouts, and
  resets one to how you saved it. Your layout is remembered the next time you start Pixolotl.
- **A selection box you can see on photos.** The box and its handles now have a dark and a light edge, so
  they show over any picture. Before, the thin blue line could vanish on a photo.
- **Image Trace no longer covers your artwork when its panel is hidden.** Its preview shows only while the
  panel is in front.

Known limits are those of 0.3.1. A panel opened from the column stays open when you click the canvas.

## 0.3.1

- **Smooth panning over blurred layers again.** Panning at 100 % over a layer with a medium blur had
  dropped below 60 frames a second in 0.3.0; it is back to full speed.
- **A clearer taskbar icon.** The small icon is redrawn so the face reads at taskbar and title bar size.

Known limits are those of 0.3.0, without the blur panning one.

## 0.3.0

More of Photoshop: patterns, new adjustments and layer effects, CMYK pixel layers, and many selection,
brush, and image commands.

- **Posterize, Photo Filter, and Color Lookup.** Three more adjustments, as layers or on a layer: Posterize
  (2 to 255 levels), Photo Filter (Photoshop's warming, cooling, and colored filters, or any color, with
  Density and Preserve Luminosity), and Color Lookup (load a 3D LUT from a .cube file; the table is kept in
  the document and offered to every other Color Lookup). They come in from Photoshop files and go back out.
- **Channel eyes and targets.** In the Channels panel each color channel has an eye that shows or hides it
  on the canvas (one channel alone shows as gray) and a brush that says whether painting, fills, and filters
  change it. A CMYK layer's four inks are listed too.
- Documents with Posterize, Photo Filter, Color Lookup, or channel targets need this version or later to
  open (format version 13).
- **Fill opacity.** Beside Opacity, Properties has Fill: it fades what a layer draws but not its layer
  effects, so a shape at Fill 0 % shows only its stroke or shadow, as in Photoshop. Photoshop files keep
  each layer's Fill both ways.
- **Layer effects blend with what is below.** A Screen glow, a colored Multiply shadow, and effects on a
  layer with its own blend mode now mix with the layers underneath, as Photoshop draws them.
- **Satin, contours, noise, and Global Light.** The Layer Style list has Satin. Shadows, glows, bevels, and
  satin have Photoshop's contours (Cone, Gaussian, Ring, and the rest), glows a Range, and shadows and glows
  Noise. Use Global Light ties the angle of shadows and bevels to the document's light: turn one dial and
  every effect that uses it follows. Contours and the light come in from Photoshop files and go back out.
- **Wide effects stay fast.** A stroke or glow hundreds of pixels wide is drawn by the graphics card instead
  of slowly by the processor.
- **Effects in exported Photoshop files' preview.** The flattened picture of an exported PSD now shows the
  layer effects, so programs that show only that picture show them too.
- Documents with fill opacity, the global light, satin, contours, or noise need this version or later to
  open (format version 11).
- **More of Photoshop's Select menu.** Select > Reselect (Shift+Ctrl+D) brings back the selection you just
  took away. Select > Modify > Border… turns a selection into a soft band along its edge, and Smooth… removes
  specks and gaps and rounds corners. Select > Similar adds every pixel in the colors of the selected ones,
  using the Magic Wand's tolerance.
- **Fixed Ratio and Fixed Size marquees.** The marquees' toolbar has a Style: drag a shape of a set
  proportion, or click to place a selection of an exact size in pixels.
- **Duplicate brushes.** Duplicate any brush in the Brushes panel, the built-in ones included, to change or
  rename your copy. Renaming a built-in brush saves a renamed copy and leaves the original as it is.
- **An eyedropper and a preview in Color Range.** Click the canvas to pick the color to select; the dialog
  shows what will be selected as you change the fuzziness. Add to Sample and Subtract from Sample (or
  Shift-click and Alt-click) add more colors or take colors out.
- **A press profile for CMYK.** New CMYK documents use the CGATS21 CRPC6 profile, now included with
  Pixolotl. Documents you already have keep their own profile.
- **Partly locked layers are marked.** A pixel layer with any of its three locks on shows a small lock in
  the Layers panel; point at it to see which.
- **Healing never gives up on a busy computer.** The Spot Healing Brush, the Healing Brush, the Patch tool,
  and Fill From Surroundings no longer stop after a few seconds and throw the stroke away when the computer
  is slow or busy: they take as long as they need, with the progress line and its Cancel button.
- **The Spot Healing Brush keeps up with the pen.** Its darkened preview is drawn in the background, so
  painting a large spot never makes the pen wait.
- **Changing Warp's grid keeps your warp.** Choosing more or fewer rows and columns while warping keeps the
  shape you dragged instead of starting again.
- **Free Transform shows the layer mask.** While you warp or distort a layer with a mask, the preview shows
  the mask bent with the layer, as the result will be.
- **Image Size keeps masks, guides, and effects in step.** Layer masks are resampled with their layers,
  guides move with the artwork, and with Scale Styles (on by default) layer effects grow and shrink with
  the image.
- **Faster brushes with color jitter.** Large brushes with color jitter, wet edges, and tapers keep up with
  the pen.
- **Layer locks.** A pixel layer's Properties have Photoshop's three locks: transparent pixels (painting,
  fills, and filters change colors only), image pixels, and position. Documents saved by this version
  need this version or later to open.
- **Image Size and Canvas Size.** File > Image Size… (Ctrl+Alt+I) scales the artboards and everything on
  them, resampling pixel layers with the method you choose; File > Canvas Size… (Ctrl+Alt+C) resizes the
  artboard around an anchor without moving the artwork.
- **Sample All Layers for the Paint Bucket.** The Paint Bucket can find the area to fill on every visible
  layer at once and fill it on the selected layer, as the Magic Wand already could.
- **Color jitter, wet edges, and tapered strokes.** The Brushes panel can vary each dab's hue, saturation,
  and brightness or mix it toward the other color, paint with watercolor-like wet edges, and taper a stroke
  at its start and end. Brushes you save keep these settings, and Photoshop brushes that use them import
  with them.
- **Magnetic Lasso.** A new lasso in the Lasso group snaps its outline to the edges in the picture as you
  move along them, with Photoshop's Width, Contrast, and Frequency.
- **Copied pixels reach other programs.** Copying pixels puts them on the system clipboard as a picture
  other programs can paste, and a picture copied elsewhere afterwards pastes here as itself.
- **Lighter marching ants.** A selection's marching ants move as smoothly as before and now use far less
  processor time while they march.
- **Pixel layers in CMYK documents.** A CMYK document's pixel layers are drawn in their inks, through the
  document's CMYK profile like its shapes, with their masks, clipping, blend modes, adjustments, filters,
  and adjustment layers. Paint them with the brushes, and lighten, darken, saturate, blur, or sharpen them
  with Dodge, Burn, Sponge, Blur, and Sharpen.
- **Selective Color's Black moves black ink.** In a CMYK document the Black sliders add or take away black
  ink itself, and pure black counts among the blacks.
- **Photoshop patterns.** Pattern fill layers, Pattern Overlay, and strokes filled with a pattern come in
  from Photoshop files with the file's patterns, draw as Photoshop draws them, and go back out. Layer Style
  has Pattern Overlay, with a menu of the document's patterns, Scale, Angle, Link with Layer, and Snap to
  Origin.
- **Gradient and pattern strokes.** A layer style's Stroke has Photoshop's Fill Type: a color, a gradient
  across the layer, or a pattern.
- **Scale Styles scales patterns too.** Image Size with Scale Styles scales a pattern overlay's and a
  pattern stroke's scale with the image.
- **Fill lines up with Opacity.** In Transparency, the Fill slider now starts where the Opacity slider does.
- Documents with raster patterns, pattern overlays, or gradient and pattern strokes need this version or
  later to open (format version 12).

Known limits in this version:

- A 1000-pixel brush with color jitter, wet edges, or tapers in a 16-bit document can lag slightly behind
  the pen.
- Panning at 100 % over a layer with a medium blur (about 20 pixels) can drop below 60 frames a second.
- A glow, shadow, or stroke that reaches about 250 pixels takes a second or two to draw the first time.
- Dragging a layer effect setting in a document with twenty or more styled layers can drop slightly below
  60 frames a second.
- Threshold, Black & White, Gradient Map, Exposure, Shadows/Highlights, and Color Lookup are not available
  in CMYK documents, and the healing tools do not work on CMYK pixel layers.
- Patterns come from Photoshop files only: there is no Define Pattern or pattern file import yet.
- Noise and diamond gradients are still approximated, a layer with both a vector and a pixel mask gets a
  group for the second mask, and smart object sources in Photoshop files are not kept.
- Copying pixels to other programs has not been tested on every Windows setup.
- Image Trace can still lose a thin light line drawn over a very different color.
- In this version a feedback report is still saved as a file for you to pass on.

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
