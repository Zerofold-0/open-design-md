---
version: "alpha"
name: "Uber Design System"
colors:
  primary: "#000000"
  on-primary: "#FFFFFF"
  primary-hover: "#000000"
  background: "#FFFFFF"
  foreground: "#000000"
  surface: "#F3F3F3"
  on-surface: "#000000"
  border: "#D9D9D9"
  accent-muted: "#C47E6F"
typography:
  heading:
    fontFamily: "sans-serif"
    fontSize: "52px"
    fontWeight: "700"
    lineHeight: "1.08"
    letterSpacing: "-0.02em"
  body:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "1.5"
    letterSpacing: "0em"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "700"
    lineHeight: "1.5"
    letterSpacing: "0em"
rounded:
  sm: "16px"
  md: "999px"
spacing:
  xxs: "1px"
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "32px"
  xl: "64px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  header:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.navigation}"
    padding: "{spacing.md}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.xxs}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.navigation}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    rounded: "{rounded.md}"
    padding: "{spacing.sm}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  navigation:
    textColor: "{colors.on-primary}"
    typography: "{typography.navigation}"
  location-field:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  selector:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    rounded: "{rounded.md}"
    padding: "{spacing.sm}"
  secondary-link:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  media-panel:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.sm}"
  overlay-banner:
    backgroundColor: "{colors.accent-muted}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  card-grid:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  field-connector:
    backgroundColor: "{colors.foreground}"
    width: "{spacing.xxs}"

---

## Overview

This design system defines a high-contrast interface with a dark navigation band, a spacious white canvas, large bold headings, rounded controls, and light-gray content surfaces. Layouts use a two-column hero pattern followed by grouped cards.

## Colors

- **Primary:** Black, used for the navigation band and high-emphasis actions.
- **On Primary:** White, used for content on primary surfaces.
- **Background:** White page canvas.
- **Foreground:** Black primary text and icons.
- **Surface:** Light gray fill for fields, selectors, and content cards.
- **On Surface:** Black content placed on light-gray surfaces.
- **Border:** Subtle gray structural separator.
- **Accent Muted:** Warm muted accent used for an overlaid callout or status banner.

## Typography

Use a clean sans-serif family throughout. Large headings are bold, tightly tracked, and set with compact line height. Body text uses regular weight and generous line height. Navigation and control labels use bold text at the body scale.

## Layout

Use a centered content container with generous horizontal margins. The primary hero uses a wide two-column arrangement: form and messaging content on one side, with a large media panel on the other. Stack the columns responsively on narrower screens. Maintain clear vertical separation between the hero, subsequent section heading, and card grid.

Use compact spacing inside controls and fields, medium spacing between related groups, and large spacing between major sections. Align fields and actions to a consistent content column.

## Elevation & Depth

The interface relies primarily on contrast, spacing, and rounded surfaces rather than visible shadows. Use a muted accent overlay to establish hierarchy over media. Avoid strong elevation effects unless a floating element must be separated from its background.

## Shapes

Use a moderate rounded corner for fields, cards, media panels, and primary controls. Use a fully rounded pill shape for compact selectors and secondary actions. Keep separators and connector lines square-edged.

## Components

- **header:** Dark full-width navigation band with light navigation content and generous horizontal padding.
- **navigation:** Bold light navigation labels arranged horizontally with optional icon or disclosure affordances.
- **heading:** Large bold black heading with compact line height and slightly tight tracking.
- **selector:** Light-gray pill-shaped control for choosing a mode or timing option.
- **location-field:** Light-gray rounded field with a leading location marker, muted input text, and an optional trailing action icon.
- **field-connector:** Thin vertical black connector between related location fields.
- **button-primary:** Black rounded action with white bold text.
- **button-primary-hover:** Independent hover state retaining the black-and-white high-contrast treatment.
- **button-secondary:** White pill-shaped action with black bold text.
- **secondary-link:** Black underlined text action placed beside a primary button.
- **media-panel:** Large rounded visual panel that can contain an illustration or photographic asset.
- **overlay-banner:** Warm muted accent rounded banner positioned over media, using black text and an optional white secondary action.
- **card:** Light-gray rounded content block with black heading and body content.
- **card-grid:** Evenly spaced row of related cards that collapses into a vertical stack responsively.
- **surface:** Reusable light-gray grouping surface for fields and content areas.
- **border:** Thin gray structural separator.
- **page:** White canvas with black default text.

## Do's and Don'ts

### Do

- Reference visual values through tokens such as `{colors.primary}` and `{spacing.sm}`.
- Preserve the strong black-and-white contrast hierarchy.
- Use rounded pills for compact selectors and rounded corners for larger fields and cards.
- Keep hero content aligned to a clear column and give the adjacent media generous space.
- Maintain WCAG AA contrast for text and interactive controls.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not nest hover or other interaction variants inside a base component.
- Do not use heavy shadows or excessive decorative borders.
- Do not make every element pill-shaped; reserve the pill shape for compact controls.
- Do not introduce dense layouts that remove the generous spacing between major content groups.
