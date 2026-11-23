<div align="center">

<img src="assets/pixolotl.svg" width="128" alt="Pixolotl logo: a golden axolotl with a pen nib" />

# Pixolotl

### Vector and raster design in one application

Drawing, type, colour for print, and pixels in the same document, so you do not need one program for
vectors and another for images. Free, with **no account, no telemetry and no AI**.<br />
Made by [CodeMushroom](https://github.com/CodeMushroom).

[![Latest release](https://img.shields.io/github/v/release/CodeMushroom/Pixolotl?label=latest&color=ffc24a)](https://github.com/CodeMushroom/Pixolotl/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/CodeMushroom/Pixolotl/total?color=2fc4b6)](https://github.com/CodeMushroom/Pixolotl/releases)
![Platforms](https://img.shields.io/badge/platforms-Windows-7a6bd6)
[![License: Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-ec5a2a)](LICENSE)

### [⬇ Download Pixolotl](https://github.com/CodeMushroom/Pixolotl/releases/latest)

</div>

> **This is an early test build.** Much of Pixolotl works today and some of it is not built yet (see
> [What is coming](#what-is-coming)). Keep copies of anything important, and please
> [report](#feedback) what goes wrong.

![Pixolotl with an app icon on the artboard and the Export panel showing two PNG sizes with a live preview and file size](assets/export.png)

## What it does today

### Draw with precision

Shapes that stay editable, the Pen, Pencil, Paintbrush and Width tools, Shape Builder, Pathfinder and live
boolean shapes, Offset Path, Outline Stroke and Simplify. Several artboards, rulers, guides, grids, smart
guides and snapping. Every field takes typed numbers, units and arithmetic, and nothing drifts when you
save and open again.

### Colour for screen and print

RGB, CMYK, grayscale, Lab and spot colours with ICC colour management. CMYK documents with soft proofing,
gamut warning and overprint preview. Swatches, linear, radial and conic gradients edited on the canvas,
patterns, blend modes, and opacity and clipping masks.

![Editing a radial gradient on the canvas, with the Gradient panel showing its stops](assets/gradient.png)

### Type

Point type, area type in any shape and type on a path, with character and paragraph controls, tabs,
OpenType features, variable fonts and styles. Arabic, Hebrew, Devanagari, Thai, Chinese, Japanese and
Korean are shaped and laid out properly, and colour fonts work.

![Arabic with Latin, Devanagari and Thai text in one text frame](assets/type.png)

### Pixels in the same document

Pixel layers sit next to vector layers. Select with marquees, lassos, the magic wand or colour range, refine
with feather, grow, shrink and quick mask, and paint on layers and masks with the Brush, Eraser, Smudge,
Clone Stamp, Paint Bucket and Gradient. The Brushes panel has pressure and tilt dynamics and a stabilizer.

![The Brushes panel editing a chalk brush over a painted landscape](assets/painting.png)

![The Clone Stamp copying the sun across a pixel layer](assets/pixels.png)

### Open and export the files you use

Opens SVG, PDF, Illustrator files saved with PDF content, PNG, JPEG, TIFF, WebP, and ASE, ACO and GPL
swatches. Exports SVG, PDF for print (CMYK, spot colours, bleed, crop marks and a preflight check), PNG,
JPEG, TIFF and WebP with a live preview and the exact file size. Every import tells you anything it could
not bring in. `pixolotl --export` converts files from the command line.

### Never lose work

Unlimited undo with a History panel, safe saving, and automatic recovery of unsaved work after a crash.
Dark and light themes, and interface text from 100% to 200%.

## What is coming

- Adjustments, filters, layer effects and retouching tools
- Photoshop (PSD) and GIMP (XCF) files, and brush imports
- Live effects, symbols, and EPS and DXF export
- Saved workspaces and preferences, a shortcut editor and a command palette
- **macOS and Linux** versions

The [changelog](CHANGELOG.md) lists what each version brings.

## Install

Open the **[latest release](https://github.com/CodeMushroom/Pixolotl/releases/latest)** and download the file
that ends in **`Windows-setup.exe`**. It installs for your Windows account only and needs no administrator
rights. Everything else attached to a release (`.sig`, `latest.json`) is for the built-in updater and can
be ignored.

The installer is not yet signed with a Windows certificate, so the first launch shows a warning. Choose
**More info → Run anyway**.

Uninstall from **Settings → Apps**. Your documents, brushes and fonts stay where they are.

## Updates

Pixolotl checks for a new version when it starts, and whenever you choose **Help → Check for Updates**.
When there is one, it tells you what is new and offers **Install and Restart**. Nothing is downloaded or
installed until you say so.

- **The update check is the only network request Pixolotl makes.** It reads one public file from this
  repository's latest release. Nothing about you, your computer or your documents is sent.
- **Every update is signed** by CodeMushroom and checked against a key built into Pixolotl before it is
  installed. A download that does not match is deleted.
- To stop the check at start, untick **Check for updates when Pixolotl starts** in **Help → About
  Pixolotl**.

## Feedback

Found a bug or want a feature? [Open an issue](https://github.com/CodeMushroom/Pixolotl/issues/new/choose).
Please say which version you have (Help → About Pixolotl) and what you did. If Pixolotl is useful to you,
a ⭐ on this repository helps other designers find it.

This repository holds Pixolotl's releases, release notes and issues.

---

<div align="center">

Pixolotl is made by **[CodeMushroom](https://github.com/CodeMushroom)**. Copyright © 2026 CodeMushroom.

Licensed under the [Apache License 2.0](LICENSE). Redistributions must keep the [NOTICE](NOTICE) crediting CodeMushroom.<br />
The Pixolotl name and axolotl logo are CodeMushroom trademarks: see [TRADEMARKS.md](TRADEMARKS.md).

</div>
