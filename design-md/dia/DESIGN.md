---
version: "alpha"
name: "Dia Design System"
omitted:
  - "Source-specific copy"
  - "Brand marks"
  - "Personal imagery and identifying content"
  - "URLs and page-specific navigation labels"
colors:
  primary: "#FFFFFF"
  on-primary: "#000000"
  primary-hover: "#E6E6E6"
  background: "#000000"
  foreground: "#FFFFFF"
  surface: "#24231F"
  on-surface: "#FFFFFF"
  muted: "#999999"
  border: "#333333"
typography:
  display:
    fontFamily: "Exposure Variable"
    fontSize: "56px"
    fontWeight: "300"
    lineHeight: "52px"
    letterSpacing: "-1.68px"
  heading:
    fontFamily: "Exposure Variable"
    fontSize: "24px"
    fontWeight: "400"
    lineHeight: "32px"
    letterSpacing: "-0.48px"
  body:
    fontFamily: "ABC Oracle"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0px"
  label:
    fontFamily: "ABC Oracle"
    fontSize: "14px"
    fontWeight: "400"
    lineHeight: "20px"
    letterSpacing: "0px"
rounded:
  sm: "16px"
  md: "24px"
  lg: "9999px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  2xl: "48px"
  3xl: "64px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  navigation:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  hero:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  display-mark:
    textColor: "{colors.foreground}"
    typography: "{typography.display}"
  hero-copy:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.heading}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  helper-text:
    textColor: "{colors.muted}"
    typography: "{typography.label}"
  media:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
  media-control:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.lg}"
    padding: "{spacing.sm}"
  support-control:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
  border:
    backgroundColor: "{colors.border}"

---

## Overview

This design system defines a high-contrast, dark landing-page composition with a centered hero, floating light navigation, prominent light action controls, and immersive media. It intentionally excludes source-specific copy, marks, imagery, and identifying details.

## Colors

- **Background:** Use near-black for the primary canvas and media backdrop.
- **Foreground:** Use white for high-emphasis text and display elements.
- **Primary:** Use white for prominent actions and floating navigation.
- **On Primary:** Use black for text and icons placed on primary controls.
- **Primary Hover:** Use a slightly darker white for light control hover states.
- **Surface:** Use a warm charcoal for media controls and compact overlays.
- **On Surface:** Use white for content placed on dark surfaces.
- **Muted:** Use accessible gray for supporting or secondary text.
- **Border:** Use dark gray for restrained structural separation.

## Typography

Use **Exposure Variable** for the oversized display mark and concise hero heading. Use **ABC Oracle** for navigation, body, labels, and controls. The hierarchy is compact, centered, and spacious, with tight display tracking and generous line spacing for supporting text.

## Layout

- Use a full-bleed dark canvas with a centered content column.
- Position the navigation as a floating pill near the top of the viewport.
- Keep the hero mark, supporting heading, primary action, and helper text vertically stacked and center aligned.
- Separate hero elements with the spacing scale rather than relying on arbitrary offsets.
- Allow immersive media to extend below the initial viewport while keeping its focal content centered.
- Keep compact controls centered over media or anchored to the viewport edge as floating overlays.
- Preserve responsive behavior by allowing the centered column and navigation pill to contract on narrow screens.

## Elevation & Depth

Use minimal elevation. Light floating navigation and action controls may use a restrained shadow or edge contrast against the dark canvas, while dark media controls should rely primarily on surface contrast and rounded silhouettes. Avoid layered cards or strong decorative shadows.

## Shapes

- Use rounded rectangular pills for navigation, primary actions, and compact media controls.
- Use the medium radius for large light controls and floating navigation.
- Use the full radius for compact circular or capsule-shaped overlays.
- Keep corners smooth and consistent across controls; avoid sharp card-like geometry.

## Components

- **navigation:** Floating light navigation using {colors.primary} with {colors.on-primary} content, {rounded.md}, and {spacing.md} padding.
- **hero:** Centered dark hero region using {colors.background} and {colors.foreground}.
- **display-mark:** Oversized display treatment using {colors.foreground} and {typography.display}.
- **hero-copy:** Short centered heading using {colors.foreground} and {typography.heading}.
- **button-primary:** Large light call-to-action using {colors.primary} with {colors.on-primary} content, {rounded.md}, and {spacing.lg} padding.
- **button-primary-hover:** Independent hover state using {colors.primary-hover} with {colors.on-primary} content.
- **helper-text:** Low-emphasis supporting text using {colors.muted} and {typography.label}.
- **media:** Full-width dark media region using {colors.background} and {colors.foreground}.
- **media-control:** Dark capsule overlay using {colors.surface} with {colors.on-surface} content, {rounded.lg}, and {spacing.sm} padding.
- **support-control:** Compact floating support control using {colors.surface} with {colors.on-surface} content and {rounded.lg}.
- **border:** Subtle separator using {colors.border}.

## Do's and Don'ts

### Do

- Use {colors.background} as the dominant canvas color.
- Keep primary content centered and vertically sequenced.
- Use light controls with dark content for strong action contrast.
- Preserve the distinction between light floating controls and dark media overlays.
- Reference spacing, typography, colors, and radii through tokens.
- Maintain WCAG AA contrast for all text and interactive controls.

### Don't

- Do not introduce bright accent colors that compete with the monochrome hierarchy.
- Do not use dense grids or multiple competing content columns in the hero.
- Do not nest hover or other interaction variants under a base component.
- Do not hardcode captured values inside component definitions.
- Do not add source-specific copy, marks, imagery, or identifying details.
