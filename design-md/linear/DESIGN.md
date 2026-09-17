---
version: "alpha"
name: "Linear Design System"
omitted:
  - source-specific copy
  - brand marks and names
  - URLs and domains
  - personal imagery and data
  - page-specific content
colors:
  primary: "#F2F2F2"
  on-primary: "#0B0C0D"
  primary-hover: "#FFFFFF"
  background: "#08090A"
  foreground: "#F5F5F5"
  muted: "#8D9098"
  surface: "#111214"
  on-surface: "#F1F1F2"
  border: "#282A2E"
  accent: "#F2C94C"
typography:
  heading:
    fontFamily: "Inter Variable"
    fontSize: "64px"
    fontWeight: "510"
    lineHeight: "64px"
    letterSpacing: "-1.408px"
  body:
    fontFamily: "Inter Variable"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "-0.16px"
  navigation:
    fontFamily: "Inter Variable"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "-0.16px"
  label:
    fontFamily: "Inter Variable"
    fontSize: "14px"
    fontWeight: "500"
    lineHeight: "20px"
    letterSpacing: "-0.14px"
rounded:
  sm: "2px"
  md: "6px"
  lg: "12px"
  pill: "999px"
spacing:
  hairline: "1px"
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "48px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  header:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.navigation}"
    padding: "{spacing.md}"
    borderColor: "{colors.border}"
  navigation-link:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.navigation}"
    padding: "{spacing.sm}"
    rounded: "{rounded.sm}"
  navigation-link-active:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.sm}"
    rounded: "{rounded.sm}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "{spacing.sm}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "{spacing.sm}"
  heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  body-copy:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.body}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    borderColor: "{colors.border}"
  app-preview:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    borderColor: "{colors.border}"
    padding: "{spacing.xl}"
  sidebar:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    padding: "{spacing.lg}"
  sidebar-item:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.muted}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  sidebar-item-active:
    backgroundColor: "{colors.border}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  metadata-panel:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    borderColor: "{colors.border}"
    padding: "{spacing.lg}"
  status-accent:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.accent}"
    typography: "{typography.label}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
  floating-help:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.pill}"
    borderColor: "{colors.border}"
---

## Overview

This design system describes a dark, spacious interface with a restrained monochrome palette, high-contrast typography, subtle panel separation, and compact utility controls. The composition uses a wide centered content area, a persistent top navigation bar, a large hero hierarchy, and a detailed application preview.

## Colors

- **Background:** Near-black page canvas used across the primary composition.
- **Foreground:** Near-white color for prominent headings and high-emphasis content.
- **Muted:** Cool gray for secondary copy, navigation, metadata, and supporting labels.
- **Surface:** Slightly lifted charcoal used for previews, panels, sidebars, and floating controls.
- **On Surface:** Light text used inside dark surfaces.
- **Border:** Low-contrast gray for thin separators and panel outlines.
- **Primary:** Light neutral fill for the highest-emphasis action.
- **On Primary:** Dark text used on the primary action.
- **Primary Hover:** Brighter neutral fill for the primary action hover state.
- **Accent:** Warm yellow used sparingly for status and attention indicators.

## Typography

Use **Inter Variable** throughout the interface. The main heading is exceptionally large, tightly tracked, and presented with a light-to-regular variable weight. Body and navigation text use a compact 16px rhythm, while labels and metadata use a smaller 14px style. Secondary copy is distinguished primarily through the muted color rather than dramatic changes in size.

## Layout

- Use a wide centered content region with consistent horizontal gutters.
- Keep the top navigation in a shallow full-width bar separated from the page by a fine border.
- Place the hero heading in the left portion of the content region and allow it to wrap across two lines.
- Position supporting copy below the heading with generous vertical separation.
- Keep secondary actions aligned toward the opposite side of the hero supporting row.
- Place the large application preview below the hero with a clear gap.
- Use a narrow vertical sidebar within the preview and a larger content area beside it.
- Organize detailed content into a primary reading region and a narrower metadata region.
- Preserve generous empty space around the hero rather than compressing the content toward the header.

## Elevation & Depth

Depth is communicated primarily through near-black surfaces, subtle one-pixel borders, and very restrained tonal differences. Use a soft, low-opacity dark shadow beneath floating or raised surfaces; avoid strong blur, glossy gradients, or pronounced drop shadows.

## Shapes

Use small radii for navigation items and compact controls. Use a medium-to-large radius for application previews, cards, and floating panels. Use pill-shaped geometry for the prominent light action. Keep borders thin and understated, with no decorative corner treatments.

## Components

- **header:** Full-width dark navigation bar using {colors.background}, {colors.muted}, and {colors.border}.
- **navigation-link:** Secondary navigation item using {colors.background} with {colors.muted} text.
- **navigation-link-active:** Emphasized navigation item using {colors.background} with {colors.foreground} text.
- **button-primary:** Pill-shaped high-emphasis action using {colors.primary} and {colors.on-primary}.
- **button-primary-hover:** Independent hover state using {colors.primary-hover} and {colors.on-primary}.
- **heading:** Large hero heading using {colors.foreground} and {typography.heading}.
- **body-copy:** Supporting copy using {colors.background}, {colors.muted}, and {typography.body}.
- **surface:** Reusable lifted region using {colors.surface}, {colors.on-surface}, and {colors.border}.
- **app-preview:** Large rounded interface preview using {colors.surface}, {colors.on-surface}, and {colors.border}.
- **sidebar:** Dark navigation column within a preview using {colors.surface} and {colors.on-surface}.
- **sidebar-item:** Inactive sidebar row using {colors.surface} and {colors.muted}.
- **sidebar-item-active:** Selected sidebar row using {colors.border} and {colors.on-surface}.
- **metadata-panel:** Secondary information region using {colors.surface}, {colors.on-surface}, and {colors.border}.
- **status-accent:** Sparse status indicator using {colors.surface} and {colors.accent}.
- **border:** One-pixel structural separator using {colors.border}.
- **floating-help:** Circular or pill-like floating utility using {colors.surface}, {colors.on-surface}, and {colors.border}.

## Do's and Don'ts

### Do

- Use the near-black background and charcoal surfaces to establish the visual hierarchy.
- Maintain strong contrast for headings, primary actions, and surface content.
- Use muted text for secondary information without reducing legibility.
- Keep borders subtle and consistently one pixel.
- Preserve the generous hero spacing and wide horizontal composition.
- Reference all visual values through tokens such as {colors.primary} and {spacing.lg}.
- Keep component states as separate flat entries.

### Don't

- Do not introduce bright multicolor backgrounds or heavy gradients.
- Do not use strong shadows or excessive elevation.
- Do not make every label high contrast; preserve the foreground and muted distinction.
- Do not replace the pill-shaped primary action with a sharp rectangular control.
- Do not hardcode captured colors inside component definitions.
- Do not nest hover, active, or selected variants inside a base component.
- Do not add source-specific copy, names, imagery, or content to reusable patterns.
