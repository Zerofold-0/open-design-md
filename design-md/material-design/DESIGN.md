---
version: "alpha"
name: "Material Design System"
colors:
  primary: "#9B7CFF"
  on-primary: "#21134F"
  primary-hover: "#A98EFF"
  background: "#111111"
  foreground: "#F5F1F4"
  surface: "#1C1C1E"
  on-surface: "#F5F1F4"
  sidebar: "#211F21"
  muted: "#C7C1C8"
  border: "#4B4850"
typography:
  display:
    fontFamily: "sans-serif"
    fontSize: "96px"
    fontWeight: "400"
    lineHeight: "96px"
    letterSpacing: "-0.03em"
  heading:
    fontFamily: "sans-serif"
    fontSize: "64px"
    fontWeight: "400"
    lineHeight: "72px"
    letterSpacing: "-0.02em"
  body:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0em"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0em"
rounded:
  sm: "12px"
  md: "24px"
  lg: "32px"
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
  sidebar:
    backgroundColor: "{colors.sidebar}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.md}"
  navigation-item:
    backgroundColor: "{colors.sidebar}"
    textColor: "{colors.muted}"
    typography: "{typography.navigation}"
    rounded: "{rounded.pill}"
    padding: "{spacing.sm}"
  navigation-item-active:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    rounded: "{rounded.pill}"
    padding: "{spacing.sm}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xl}"
  hero-panel:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xxl}"
  media-panel:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.lg}"
  display-heading:
    textColor: "{colors.foreground}"
    typography: "{typography.display}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  body-copy:
    textColor: "{colors.muted}"
    typography: "{typography.body}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "{spacing.md}"
  icon-button:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.pill}"
    padding: "{spacing.sm}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"

---

## Overview

This system uses a dark, spacious canvas with a persistent navigation rail, large typographic introductions, rounded content panels, and a vivid accent action. The composition balances a restrained interface shell with dense visual media areas.

## Colors

- **Background:** Near-black page canvas for the primary workspace.
- **Surface:** Slightly lighter charcoal for hero panels, grouped content, and controls.
- **Sidebar:** Deep charcoal used to distinguish persistent navigation from the main canvas.
- **Primary:** Bright lavender accent for prominent actions and selected emphasis.
- **On Primary:** Deep violet text chosen for readable content on the primary accent.
- **Foreground:** Soft near-white for headings and high-emphasis interface content.
- **Muted:** Light gray-lavender for supporting text and secondary navigation.
- **Border:** Low-contrast gray for thin structural separators.

## Typography

Use a clean sans-serif family throughout. The display style is exceptionally large, light in weight, and tightly tracked. Supporting copy remains compact with a 16px size and 24px line height. Navigation labels use the same body scale with restrained emphasis.

## Layout

Use a persistent narrow navigation rail along the left edge and a broad content region to its right. Organize the main region with generous outer margins, large rounded hero panels, and adjacent or stacked media panels. Preserve a spacious vertical rhythm between the introductory block, primary action, and subsequent sections. Allow the media area to use a dense collage or multi-column arrangement while retaining consistent gutters.

## Elevation & Depth

Use subtle separation rather than strong shadows. Recommended depth is a restrained shadow equivalent to `rgba(0, 0, 0, 0.30) 0px 1px 2px 0px, rgba(0, 0, 0, 0.15) 0px 1px 3px 1px`. Keep the dark surface steps and rounded edges as the main sources of hierarchy.

## Shapes

Use large radii for hero and media panels, pill shapes for prominent actions and selected navigation items, and smaller rounded shapes for compact controls. Keep corners consistently soft and avoid sharp rectangular controls unless they function as a structural divider.

## Components

- **page:** Full-screen dark canvas using `{colors.background}` with `{colors.foreground}` content.
- **sidebar:** Persistent navigation rail using `{colors.sidebar}` and `{colors.foreground}`.
- **navigation-item:** Low-emphasis navigation control using `{colors.sidebar}` with `{colors.muted}` text.
- **navigation-item-active:** Selected navigation control using `{colors.surface}` with `{colors.foreground}` text.
- **surface:** Rounded grouped region using `{colors.surface}` and `{colors.on-surface}`.
- **hero-panel:** Large introductory panel using `{colors.surface}` and `{colors.foreground}`.
- **media-panel:** Rounded visual-content region using `{colors.surface}` and `{colors.foreground}`.
- **display-heading:** Oversized introductory heading using `{colors.foreground}` and `{typography.display}`.
- **heading:** Section heading using `{colors.foreground}` and `{typography.heading}`.
- **body-copy:** Supporting copy using `{colors.muted}` and `{typography.body}`.
- **button-primary:** Pill-shaped high-emphasis action using `{colors.primary}` with `{colors.on-primary}` text.
- **button-primary-hover:** Independent hover state using `{colors.primary-hover}` with `{colors.on-primary}` text.
- **icon-button:** Compact rounded control using `{colors.surface}` with `{colors.foreground}` icon content.
- **border:** Thin structural separator using `{colors.border}`.

## Do's and Don'ts

### Do

- Use the dark canvas and charcoal surface contrast to establish hierarchy.
- Reserve the lavender accent for prominent actions and selected emphasis.
- Keep display headings large, airy, and visually dominant.
- Use generous spacing around major panels and introductory content.
- Maintain strong contrast for all text and interactive controls.
- Keep state variants as separate component entries.

### Don't

- Do not introduce bright backgrounds that compete with the dark interface shell.
- Do not use sharp corners for primary panels or prominent controls.
- Do not overuse the accent color for ordinary body text or large surfaces.
- Do not compress the navigation rail, hero panel, or primary spacing rhythm.
- Do not hardcode captured colors inside component definitions.
- Do not nest hover, active, or pressed variants inside a base component.
