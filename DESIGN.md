---
version: alpha
name: To Comment or Not To Comment
description: >-
  Accessible, colorblind-friendly presentation design built on RevealJS simple:
  clean white canvas, high-contrast dark typography, ColorBrewer purple/gold
  callout semantics, and optimized code tables.
colors:
  primary: "#1a1a1a"
  canvas: "#ffffff"
  text: "#222222"
  muted: "#666666"
  tip-purple: "#7570B3"
  tip-bg: "rgba(117, 112, 179, 0.15)"
  caution-gold: "#E6AB02"
  caution-bg: "rgba(230, 171, 2, 0.15)"
  code-bg: "#f8f9fa"
typography:
  display:
    fontFamily: Helvetica Neue, Helvetica, Arial, sans-serif
    fontSize: 2.1em
    fontWeight: 700
  heading:
    fontFamily: Helvetica Neue, Helvetica, Arial, sans-serif
    fontSize: 1.4em
    fontWeight: 700
  body:
    fontFamily: Helvetica Neue, Helvetica, Arial, sans-serif
    fontSize: 32px
    fontWeight: 400
  mono:
    fontFamily: monospace
rounded:
  sm: 4px
  md: 8px
components:
  page:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.text}"
  callout-tip:
    borderColor: "{colors.tip-purple}"
    backgroundColor: "{colors.tip-bg}"
  callout-caution:
    borderColor: "{colors.caution-gold}"
    backgroundColor: "{colors.caution-bg}"
---

# DESIGN.md

The visual design specification of the To Comment or Not To Comment presentation deck.

## Overview

The visual design is built on Quarto's RevealJS `simple` theme, optimized for clarity, accessibility, and colorblind friendliness. It employs a clean white canvas, high-contrast dark text, ColorBrewer Dark2-inspired callout accents (purple for good practices, gold for cautions), structured comparison tables, and SVG icons.

The theme format is Quarto RevealJS (`theme: simple`). Custom styles are defined in `style.css` and mirrored in the front matter above.

## Colours

- **Canvas & Text:**
  - `canvas` (`#ffffff`): Crisp white background.
  - `text` (`#222222`): High-contrast dark grey body copy and headings.
  - `muted` (`#666666`): Captions, footnotes, and citation text.
- **Colorblind-Friendly Semantic Accents:**
  - `tip-purple` (`#7570B3`): Purple accent for `.callout-tip` representing good commenting patterns and effective documentation. Background: `rgba(117, 112, 179, 0.15)`.
  - `caution-gold` (`#E6AB02`): Gold/amber accent for `.callout-caution` representing stale, redundant, or misleading comment warnings. Background: `rgba(230, 171, 2, 0.15)`.
- **Code Background:**
  - `code-bg` (`#f8f9fa`): Soft light grey backing for code blocks rendered inside tables and callouts.

## Typography

- **Headings & Body:** Default clean sans-serif stack (`Helvetica Neue`, `Helvetica`, `Arial`, `sans-serif`).
- **Code:** Monospace stack for inline code snippets, syntax examples, and comparison tables. Code font size is tuned for table cell density (`0.9em`) and callout readability.

## Layout & Components

- **Callouts:** `.callout-tip` and `.callout-caution` with accessible left accent borders and tint backings.
- **Code Comparison Tables:** `.smaller table` with code blocks styled on `#f8f9fa` backings for side-by-side good vs. bad commenting comparisons.
- **Icons:** SVG mask icons (`.deck-icon`) using Font Awesome Free paths rendered via CSS masks in `currentColor`.

## Do's and Don'ts

- **Do** use `.callout-tip` and `.callout-caution` for semantic highlighting.
- **Do** ensure code blocks inside tables maintain readability and responsive wrapping.
- **Don't** use red/green pairings for good vs. bad comparisons; preserve the colorblind-friendly purple/gold system.
- **Don't** hard-code ad-hoc colors directly in `index.qmd`.
