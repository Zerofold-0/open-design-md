---
version: "alpha"
name: "Mobbin Design System"
colors:
  primary: "#141414"
  on-primary: "#FFFFFF"
  primary-hover: "#2E2E2E"
  background: "#FFFFFF"
  foreground: "#141414"
  muted: "#666666"
  surface: "#F5F5F5"
  on-surface: "#141414"
  border: "#DEDEDE"
  accent: "#4D46E8"
  on-accent: "#FFFFFF"
typography:
  heading:
    fontFamily: "M Saans 652"
    fontSize: "80px"
    fontWeight: "652"
    lineHeight: "1"
    letterSpacing: "-2px"
  body:
    fontFamily: "sans-serif"
    fontSize: "32px"
    fontWeight: "400"
    lineHeight: "1.3"
    letterSpacing: "-0.5px"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "32px"
    fontWeight: "600"
    lineHeight: "1.2"
    letterSpacing: "-0.5px"
  button:
    fontFamily: "sans-serif"
    fontSize: "28px"
    fontWeight: "600"
    lineHeight: "1.2"
    letterSpacing: "-0.5px"
  caption:
    fontFamily: "sans-serif"
    fontSize: "28px"
    fontWeight: "400"
    lineHeight: "1.3"
    letterSpacing: "-0.3px"
rounded:
  sm: "16px"
  md: "32px"
  lg: "60px"
  full: "999px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "40px"
  xl: "64px"
  xxl: "96px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  navigation:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.navigation}"
    rounded: "{rounded.lg}"
    padding: "{spacing.md}"
  navigation-mark:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.sm}"
  navigation-link:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.navigation}"
  hero:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    padding: "{spacing.xxl}"
  hero-icon-tile:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    accentColor: "{colors.accent}"
    accentTextColor: "{colors.on-accent}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  supporting-copy:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.body}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.full}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.full}"
    padding: "{spacing.md}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    typography: "{typography.button}"
    rounded: "{rounded.full}"
    padding: "{spacing.md}"
  trust-label:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.caption}"
  wordmark-row:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.body}"
  floating-avatar:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: "{spacing.xs}"
  border:
    backgroundColor: "{colors.border}"
    height: "1px"
---

## Overview

This design system describes a spacious, centered interface with a light canvas, a restrained monochrome palette, oversized display typography, pill-shaped controls, and a small saturated accent used for decorative illustration.

## Colors

- **Primary:** Near-black color for high-emphasis actions and marks.
- **On Primary:** White content placed on primary controls.
- **Primary Hover:** Slightly lighter near-black interaction state.
- **Background:** White page canvas.
- **Foreground:** Near-black primary text.
- **Muted:** Medium gray for supporting copy, labels, and subdued marks.
- **Surface:** Very light gray used for the navigation container and soft tiles.
- **On Surface:** Dark content placed on light surfaces.
- **Border:** Light gray outline for secondary controls.
- **Accent:** Saturated blue-violet used sparingly in decorative iconography.
- **On Accent:** White content placed over the accent color.

## Typography

Use the captured heavy sans-serif display style for the primary heading. Display text is very large, tightly tracked, and set with compact line height. Supporting copy uses a lighter sans-serif treatment with generous readability. Navigation and buttons use a bold sans-serif style with compact spacing.

## Layout

- Keep the page canvas white and organize the main content on a centered vertical axis.
- Use a wide, shallow navigation container near the top with generous horizontal padding.
- Provide substantial vertical separation between navigation, decorative hero imagery, heading, supporting copy, actions, and the lower trust area.
- Constrain the hero text to a readable centered measure while allowing the heading to span multiple lines.
- Place primary and secondary actions together in a centered horizontal group.
- Keep the lower logo or wordmark row centered and visually quieter than the hero.
- Allow the navigation and action group to wrap gracefully at smaller widths rather than forcing fixed page dimensions.

## Elevation & Depth

Depth is subtle and mostly expressed through pale surface fills, light borders, and small layered offsets behind the decorative hero tile. Avoid strong shadows or dramatic elevation; the page should remain visually flat and airy.

## Shapes

- Use full pill rounding for navigation containers and action buttons.
- Use a medium rounded rectangle for the decorative hero tile.
- Use a smaller radius for compact marks and internal elements.
- Use circular rounding for floating avatars.
- Keep outlines light and restrained on secondary controls.

## Components

- **navigation:** Wide, softly rounded light surface containing a compact mark and a horizontal set of links.
- **navigation-mark:** Small high-contrast graphic mark placed at the leading edge of the navigation.
- **navigation-link:** Bold, dark navigation item with generous spacing between items.
- **hero:** Centered vertical composition with large open space around the primary message.
- **hero-icon-tile:** Soft rounded tile with a saturated geometric accent and subtle layered backing shapes.
- **heading:** Oversized, near-black display heading with tight tracking and compact line height.
- **supporting-copy:** Centered muted explanatory text beneath the heading.
- **button-primary:** Dark pill-shaped primary action with white text.
- **button-primary-hover:** Separate lighter near-black hover state for the primary action.
- **button-secondary:** White pill-shaped secondary action with a light outline and dark text.
- **trust-label:** Centered muted label introducing a quieter credibility area.
- **wordmark-row:** Horizontal collection of subdued grayscale marks beneath the trust label.
- **floating-avatar:** Small circular utility element fixed near the outer edge of the viewport.
- **border:** One-pixel light structural separator or control outline.

## Do's and Don'ts

### Do

- Use tokens for every visual value, including component colors, typography, spacing, and radii.
- Preserve the strong contrast between the white canvas, dark heading, and dark primary action.
- Keep supporting text and lower-page marks visibly quieter than primary content.
- Use the blue-violet accent only for decorative emphasis.
- Maintain generous whitespace and a centered visual hierarchy.
- Keep interaction variants as separate flat component entries.

### Don't

- Do not introduce additional colors, heavy shadows, or dense layouts without a clear hierarchy need.
- Do not use the accent color for large text or primary action surfaces.
- Do not hardcode captured values inside component definitions.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not allow secondary controls to lose their light outline or dark readable text.
