---
version: "alpha"
name: "Alo Design System"
omitted:
  - "Brand marks and logos"
  - "Source-specific labels, links, and marketing copy"
  - "Personal data and third-party widget content"
colors:
  primary: "#000000"
  on-primary: "#FFFFFF"
  primary-hover: "#000000"
  background: "#FFFFFF"
  foreground: "#000000"
  surface: "#000000"
  on-surface: "#FFFFFF"
  border: "#ECECEC"
  muted: "#777777"
  control: "#333333"
  on-control: "#FFFFFF"
typography:
  heading:
    fontFamily: "proxima-nova"
    fontSize: "32px"
    fontWeight: "600"
    lineHeight: "35.2px"
    letterSpacing: "-0.96px"
  body:
    fontFamily: "proxima-nova"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "1.5"
    letterSpacing: "0px"
  label:
    fontFamily: "proxima-nova"
    fontSize: "16px"
    fontWeight: "600"
    lineHeight: "24px"
    letterSpacing: "0px"
  navigation:
    fontFamily: "proxima-nova"
    fontSize: "18px"
    fontWeight: "600"
    lineHeight: "24px"
    letterSpacing: "0px"
rounded:
  sm: "4px"
  md: "8px"
  lg: "50%"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "48px"
  hairline: "1px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  header:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.xl}"
  navigation:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    gap: "{spacing.xl}"
  header-divider:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
  footer:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    padding: "{spacing.xxl}"
  footer-heading:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label}"
  footer-link:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    padding: "{spacing.xs}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.label}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  input:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    borderColor: "{colors.border}"
    padding: "{spacing.md}"
  input-placeholder:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.muted}"
    typography: "{typography.body}"
  submit-control:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.label}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  icon-button:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.lg}"
    padding: "{spacing.sm}"
  dark-icon-button:
    backgroundColor: "{colors.control}"
    textColor: "{colors.on-control}"
    rounded: "{rounded.lg}"
    padding: "{spacing.md}"
  heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
---

## Overview

This design system describes a monochrome interface with a spacious white header, strong black content surfaces, high-contrast typography, and compact line-based controls. It is intended for reusable navigation, grouped content, forms, links, and utility controls without source-specific content.

## Colors

- **Primary:** Black, used for high-emphasis actions and dark structural surfaces.
- **On Primary:** White content placed on primary controls.
- **Primary Hover:** The captured hover treatment remains black, preserving the monochrome emphasis.
- **Background:** White page and header canvas.
- **Foreground:** Black text and icons on light surfaces.
- **Surface:** Black grouped areas such as the footer.
- **On Surface:** White text and icons on dark surfaces.
- **Border:** Very light gray structural dividers and outlines.
- **Muted:** Medium gray supporting or placeholder text.
- **Control:** Dark gray circular utility-control background.
- **On Control:** White content placed on dark utility controls.

## Typography

Use **proxima-nova** throughout the hierarchy. Body text uses a regular 16px size with a 1.5 line height. Labels and section labels use a semibold weight. Navigation is semibold and slightly larger than body text. Headings use a 32px semibold style with a tight line height and negative tracking.

## Layout

Use a wide horizontal header with generous inline padding and separated navigation and utility-control groups. Keep navigation items in a single row on large screens with consistent gaps. Organize dark grouped content into multiple columns with aligned headings and link stacks. Place form controls in a horizontal field-and-submit arrangement when space permits, and allow the groups to stack responsively on narrower layouts. Use the spacing scale for column gaps, section gaps, link rhythm, and footer padding.

## Elevation & Depth

The interface is primarily flat, using contrast, spacing, and a strong color inversion rather than persistent shadows. Reserve subtle elevation for floating circular utility controls or transient overlays. Keep shadows soft and restrained so they do not compete with the black-and-white hierarchy.

## Shapes

Use small corner radii for fields, buttons, badges, and rectangular controls. Use the medium radius for grouped surfaces when separation from the page canvas is needed. Use circular geometry for icon-only utility controls and floating actions. Avoid decorative rounding on large structural regions.

## Components

- **header:** Light, spacious horizontal shell using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **navigation:** Semibold horizontal link group with consistent {spacing.xl} gaps.
- **header-divider:** Thin structural separator using {colors.border}.
- **footer:** Large dark multi-column region using {colors.surface} and {colors.on-surface}.
- **footer-heading:** Semibold high-contrast column heading on {colors.surface}.
- **footer-link:** Vertically spaced light link within the dark footer.
- **surface:** Grouped dark content area with {rounded.md} corners and internal padding.
- **button-primary:** High-emphasis black action with white text and compact rounded geometry.
- **button-primary-hover:** Separate hover state retaining the black primary treatment.
- **button-secondary:** Light action with black text for lower-emphasis contexts.
- **input:** Dark filled field with light text, a subtle border, and compact rounded corners.
- **input-placeholder:** Muted text treatment inside {input}.
- **submit-control:** High-contrast light submit segment paired with a dark field.
- **icon-button:** Light circular icon control for header and navigation utilities.
- **dark-icon-button:** Dark circular floating utility control with white icon content.
- **heading:** High-emphasis heading using {typography.heading} and {colors.foreground}.

## Do's and Don'ts

### Do

- Reference visual values through tokens such as {colors.primary}, {spacing.md}, and {rounded.sm}.
- Preserve the strong light-header and dark-footer contrast.
- Keep navigation, footer columns, and form controls aligned to a consistent spacing rhythm.
- Use separate flat entries for hover and other component states.
- Maintain WCAG AA contrast for all text and interactive controls.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not nest hover, active, pressed, or disabled variants inside a base component.
- Do not use excessive shadows or decorative radius where spacing and contrast provide the hierarchy.
- Do not add source-specific copy, logos, or page content to reusable component rules.
