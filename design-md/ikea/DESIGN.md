---
version: "alpha"
name: "IKEA Design System"
omitted: []
colors:
  primary: "#FFDA00"
  on-primary: "#111111"
  primary-hover: "#F2C900"
  background: "#FFFEFB"
  foreground: "#111111"
  surface: "#D3A1F4"
  on-surface: "#111111"
  border: "#111111"
  overlay: "#000000"
  on-overlay: "#FFFFFF"
  control: "#FFFFFF"
  on-control: "#111111"
typography:
  display:
    fontFamily: "sans-serif"
    fontSize: "72px"
    fontWeight: "700"
    lineHeight: "0.98"
    letterSpacing: "-0.03em"
  heading:
    fontFamily: "sans-serif"
    fontSize: "40px"
    fontWeight: "700"
    lineHeight: "1.05"
    letterSpacing: "-0.02em"
  body:
    fontFamily: "sans-serif"
    fontSize: "20px"
    fontWeight: "400"
    lineHeight: "1.4"
    letterSpacing: "0em"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "32px"
    fontWeight: "400"
    lineHeight: "1.2"
    letterSpacing: "-0.01em"
rounded:
  sm: "8px"
  md: "16px"
  lg: "24px"
  full: "50%"
spacing:
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "32px"
  xl: "40px"
  xxl: "64px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  header:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.lg}"
  navigation:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    gap: "{spacing.xl}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  image-hero:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-overlay}"
    typography: "{typography.body}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  image-hero-heading:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.on-overlay}"
    typography: "{typography.display}"
  feature-panel:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.md}"
    padding: "{spacing.xxl}"
  feature-panel-heading:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.heading}"
  media-control:
    backgroundColor: "{colors.control}"
    textColor: "{colors.on-control}"
    rounded: "{rounded.full}"
    padding: "{spacing.md}"
  floating-control:
    backgroundColor: "{colors.control}"
    textColor: "{colors.on-control}"
    rounded: "{rounded.full}"
    padding: "{spacing.sm}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.xs}"

---

## Overview

This design system describes a spacious editorial interface with a warm off-white canvas, oversized imagery, bold typographic overlays, vivid accent controls, and a lavender feature section. Content is organized into wide horizontal compositions with generous gutters and rounded media containers.

## Colors

- **Primary:** Bright yellow used for prominent actions and navigation controls.
- **On Primary:** Near-black content placed on primary controls.
- **Primary Hover:** Slightly deeper yellow for interactive emphasis.
- **Background:** Warm off-white page canvas and header surface.
- **Foreground:** Near-black default text and navigation content.
- **Surface:** Light lavender used for a prominent feature panel.
- **On Surface:** Near-black text placed on lavender surfaces.
- **Border:** Near-black structural separator color.
- **Overlay:** Black image-overlay color that increases readability of text over photography.
- **On Overlay:** White text used over darkened imagery.
- **Control:** White used for circular media and utility controls.
- **On Control:** Near-black icons or labels used inside white controls.

## Typography

Use a clean sans-serif family throughout the interface. Navigation is large and lightly weighted, supporting text uses a comfortable reading size, and hero headings use a heavy weight with tight tracking and compact line height. Use display typography for short, high-emphasis image captions and heading typography for feature-panel titles.

## Layout

Use a wide responsive canvas with consistent horizontal gutters. Place large media cards in a two-column arrangement when space permits, with a substantial gap between cards. Keep text anchored near the lower edge of image cards with generous inset spacing. Feature panels use a split composition: text occupies one side while a large rounded image occupies the other. Collapse columns into a vertical flow at smaller widths while retaining the spacing hierarchy.

## Elevation & Depth

The interface relies primarily on image contrast, color blocking, and spacing rather than shadows. Use dark image overlays to separate text from photography. Circular controls may use a subtle boundary or minimal shadow only when needed to remain legible against an image.

## Shapes

Use rounded corners consistently on image cards and feature panels, with tighter rounding on buttons. Use fully circular geometry for media and floating utility controls. Keep corners soft and consistent rather than mixing sharp and highly rounded containers.

## Components

- **page:** Warm off-white canvas with near-black body content using {colors.background} and {colors.foreground}.
- **header:** Spacious page header using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **navigation:** Large horizontal navigation grouping with {colors.background} and {colors.foreground}.
- **button-primary:** High-emphasis yellow action using {colors.primary} and {colors.on-primary}.
- **button-primary-hover:** Independent hover state using {colors.primary-hover} and {colors.on-primary}.
- **image-hero:** Rounded, darkened image composition using {colors.overlay}, {colors.on-overlay}, and {rounded.md}.
- **image-hero-heading:** Large white image-overlay heading using {colors.overlay}, {colors.on-overlay}, and {typography.display}.
- **feature-panel:** Lavender editorial section using {colors.surface}, {colors.on-surface}, and {rounded.md}.
- **feature-panel-heading:** Bold dark heading on the lavender feature surface using {colors.surface}, {colors.on-surface}, and {typography.heading}.
- **media-control:** Circular white media control using {colors.control}, {colors.on-control}, and {rounded.full}.
- **floating-control:** Compact circular utility control using {colors.control}, {colors.on-control}, and {rounded.full}.
- **border:** Structural separator using {colors.border}.

## Do's and Don'ts

### Do

- Use token references such as {colors.primary} and {spacing.lg}.
- Preserve the wide, image-led composition and generous whitespace.
- Keep text over imagery inside a darkened overlay for legibility.
- Use large, concise headings with tight line height in prominent media areas.
- Maintain WCAG AA contrast for text and interactive controls.
- Keep hover and other interaction states as separate component entries.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not add heavy shadows where spacing and color blocking already establish hierarchy.
- Do not use sharp corners for the primary image and feature containers.
- Do not overcrowd the header or image captions with dense supporting content.
