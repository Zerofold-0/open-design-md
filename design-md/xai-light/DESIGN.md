---
version: "alpha"
name: "xAI Light Design System"
colors:
  primary: "#0A0A0A"
  on-primary: "#FFFFFF"
  primary-hover: "#242424"
  background: "#FFFFFF"
  foreground: "#0A0A0A"
  surface: "#F9F8F6"
  on-surface: "#0A0A0A"
  border: "#D5D5D5"
  muted: "#737373"
  accent-violet: "#B34FE8"
  accent-coral: "#F06A78"
  accent-gold: "#E7B42C"
typography:
  heading:
    fontFamily: "universalSansDisplay"
    fontSize: "60px"
    fontWeight: "500"
    lineHeight: "60px"
    letterSpacing: "-1.5px"
  body:
    fontFamily: "universalSans"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0px"
  navigation:
    fontFamily: "universalSans"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0px"
  lead:
    fontFamily: "universalSans"
    fontSize: "20px"
    fontWeight: "400"
    lineHeight: "28px"
    letterSpacing: "0px"
  label:
    fontFamily: "universalSans"
    fontSize: "14px"
    fontWeight: "500"
    lineHeight: "20px"
    letterSpacing: "0px"
rounded:
  sm: "9999px"
  md: "16px"
  lg: "28px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "48px"
  xxxl: "80px"
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
    textColor: "{colors.muted}"
    typography: "{typography.navigation}"
    gap: "{spacing.xl}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
  showcase-card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xl}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.xs}"
  announcement:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  hero:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
    padding: "{spacing.xxxl}"
  hero-lead:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.lead}"
    marginTop: "{spacing.lg}"
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
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  muted-label:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.label}"
  accent-line:
    backgroundStartColor: "{colors.accent-violet}"
    backgroundMiddleColor: "{colors.accent-coral}"
    backgroundEndColor: "{colors.accent-gold}"
    height: "{spacing.xs}"
  floating-control:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.sm}"

---

## Overview

This design system defines a spacious, monochromatic interface with centered hero content, pill-shaped actions, restrained borders, and softly tinted content surfaces. It is intended for reusable landing-page and application-shell patterns without source-specific copy or identity.

## Colors

- **Primary:** Near-black fill for high-emphasis actions.
- **On Primary:** White content placed on primary controls.
- **Primary Hover:** Slightly lighter near-black interaction state.
- **Background:** White page canvas.
- **Foreground:** Near-black high-emphasis text.
- **Surface:** Warm off-white grouping and card background.
- **On Surface:** Near-black content placed on surfaces.
- **Border:** Light neutral outline and separator color.
- **Muted:** Medium gray for navigation and supporting text.
- **Accent Violet, Coral, and Gold:** Small multicolor decorative accents used together in a restrained horizontal highlight.

## Typography

Use the display face for large, centered headings with a compact line height and slightly negative tracking. Use the regular sans-serif face for navigation, body content, labels, and controls. Supporting text is larger than standard body copy but remains lighter and muted. Keep heading weight moderate rather than bold.

## Layout

Use a centered hero composition with generous vertical spacing between the announcement, heading, supporting text, and actions. Keep primary and secondary actions in a horizontal group on wide layouts and allow them to wrap or stack on narrow layouts. Use a wide multi-column content region below the hero, with consistent gaps and equal visual weight between adjacent cards. Maintain generous page-side margins and preserve the open white space around the main content.

## Elevation & Depth

Use minimal elevation. Grouped content is distinguished primarily through the warm surface color and a subtle neutral border rather than a pronounced shadow. Floating controls may use a thin outline or very soft shadow to remain visible without competing with the hero.

## Shapes

Use fully rounded pills for buttons, compact announcements, and floating controls. Use the medium radius for standard surfaces and a larger radius for prominent showcase cards. Keep borders thin and understated. Use the accent treatment as a short horizontal decorative line rather than a large filled region.

## Components

- **page:** White canvas with near-black default text using `{colors.background}` and `{colors.foreground}`.
- **header:** Spacious navigation shell using `{colors.background}` and `{colors.foreground}`.
- **navigation:** Low-emphasis navigation links using `{colors.background}` and `{colors.muted}`.
- **announcement:** Compact pill-shaped notice using `{colors.background}` and `{colors.foreground}`.
- **hero:** Large centered heading region using `{colors.background}` and `{colors.foreground}`.
- **hero-lead:** Supporting hero copy using `{colors.background}` and `{colors.muted}`.
- **surface:** Warm grouped content area using `{colors.surface}` and `{colors.on-surface}`.
- **showcase-card:** Large rounded content panel using `{colors.surface}` and `{colors.on-surface}`.
- **border:** Thin neutral structural separator using `{colors.border}`.
- **button-primary:** High-emphasis pill action using `{colors.primary}` and `{colors.on-primary}`.
- **button-primary-hover:** Independent hover state using `{colors.primary-hover}` and `{colors.on-primary}`.
- **button-secondary:** Outlined or lightly filled alternative action using `{colors.background}` and `{colors.foreground}`.
- **muted-label:** Supporting metadata using `{colors.background}` and `{colors.muted}`.
- **accent-line:** Short decorative highlight combining `{colors.accent-violet}`, `{colors.accent-coral}`, and `{colors.accent-gold}`.
- **floating-control:** Small circular or pill-shaped persistent control using `{colors.surface}` and `{colors.foreground}`.

## Do's and Don'ts

### Do

- Reference visual values through tokens such as `{colors.primary}` and `{spacing.lg}`.
- Preserve the strong contrast between white space, near-black type, and restrained warm surfaces.
- Keep hero content centered and vertically separated with generous spacing.
- Use pill shapes for actions and compact notices.
- Maintain WCAG AA contrast for all text and interactive controls.
- Use borders and surface color before adding shadows.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not use heavy shadows, dense layouts, or strong decorative fills.
- Do not use rounded corners inconsistently across controls and content surfaces.
- Do not introduce source-specific copy, names, logos, or page content into reusable patterns.
