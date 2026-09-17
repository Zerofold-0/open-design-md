---
version: "alpha"
name: "The Verge Design System"
omitted:
  - source-specific copy
  - source-specific imagery
  - brand and product names
  - personal names and other proper nouns
  - URLs and domain references
colors:
  primary: "#5200FF"
  on-primary: "#FFFFFF"
  primary-hover: "#4400D6"
  background: "#FFFFFF"
  foreground: "#111111"
  surface: "#E9E9E9"
  on-surface: "#111111"
  muted: "#555555"
  border: "#E0E0E0"
typography:
  display:
    fontFamily: "ui-sans-serif"
    fontSize: "48px"
    fontWeight: "700"
    lineHeight: "52px"
    letterSpacing: "-1.44px"
  heading:
    fontFamily: "ui-sans-serif"
    fontSize: "32px"
    fontWeight: "700"
    lineHeight: "35.2px"
    letterSpacing: "-0.64px"
  card-heading:
    fontFamily: "ui-sans-serif"
    fontSize: "28px"
    fontWeight: "700"
    lineHeight: "30.8px"
    letterSpacing: "-0.56px"
  body:
    fontFamily: "ui-serif"
    fontSize: "24px"
    fontWeight: "400"
    lineHeight: "28.8px"
    letterSpacing: "0px"
  interface:
    fontFamily: "ui-sans-serif"
    fontSize: "14px"
    fontWeight: "500"
    lineHeight: "16.8px"
    letterSpacing: "1.4px"
rounded:
  sm: "3px"
  md: "50%"
spacing:
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
  content-column:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    padding: "{spacing.xxl}"
  right-rail:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    padding: "{spacing.lg}"
  top-rule:
    backgroundColor: "{colors.primary}"
    height: "4px"
  divider:
    backgroundColor: "{colors.border}"
    height: "1px"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
  tab-active:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.interface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  tab-inactive:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.muted}"
    typography: "{typography.interface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.interface}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  featured-story:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    gap: "{spacing.lg}"
  featured-story-heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.display}"
  story-list-item:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    padding: "{spacing.lg}"
    gap: "{spacing.md}"
  story-list-heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.card-heading}"
  story-summary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.body}"
  metadata:
    backgroundColor: "{colors.background}"
    textColor: "{colors.primary}"
    typography: "{typography.interface}"
  metadata-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.interface}"
  image-score:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    padding: "{spacing.sm}"
  ad-placeholder:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.interface}"
  icon-control:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    rounded: "{rounded.md}"

---

## Overview

This system describes an editorial interface with a spacious white canvas, a strong purple interaction accent, a multi-column desktop layout, bold sans-serif headlines, and large serif summaries. Content is organized into a featured story, compact story rows, and a separated secondary rail.

## Colors

- **Primary:** Saturated purple used for the top rule, active navigation, score treatment, and metadata accents.
- **On Primary:** White content placed on the primary purple.
- **Primary Hover:** Darker purple for interactive hover feedback.
- **Background:** White page and content canvas.
- **Foreground:** Near-black text for headlines and high-emphasis content.
- **Surface:** Light gray background for inactive segmented controls and grouped UI.
- **On Surface:** Dark text used on light gray surfaces.
- **Muted:** Medium gray for summaries, timestamps, utility labels, and inactive controls.
- **Border:** Very light gray for dividers and column separation.

## Typography

Use a heavy geometric sans-serif treatment for display and card headlines. The largest editorial headline has generous scale and tight tracking, while smaller story headlines remain bold and compact.

Use a serif face for article summaries and longer editorial text. Use the sans-serif interface style for uppercase metadata, navigation labels, timestamps, and utility controls, with visible letter spacing for small uppercase labels.

## Layout

Use a wide desktop composition with a primary editorial column and a narrower secondary rail separated by a vertical divider. Keep substantial whitespace above the content area for advertising or reserved utility space.

Within the primary column, place a purple horizontal rule above the lead heading. Follow the lead heading with a large featured image and supporting story details. Arrange secondary stories as stacked rows with text content and a compact image aligned to the trailing edge.

Keep the secondary rail independently structured, with utility controls and segmented navigation at the top, a prominent story block below, and reserved advertising space separated by dividers.

Use the spacing scale to maintain clear separation between editorial groups while keeping metadata and related controls tightly grouped.

## Elevation & Depth

The interface is primarily flat, with hierarchy communicated through whitespace, dividers, image scale, and the saturated top rule rather than shadows. Use the purple rule as an inset or structural emphasis at the beginning of the main editorial content. Avoid adding drop shadows to ordinary story cards or rails.

## Shapes

Use mostly square editorial image and content edges. Apply the small radius to controls and compact score treatments. Use the medium circular value for pill-shaped segmented navigation and circular utility or avatar controls.

## Components

- **page:** White canvas with near-black default content.
- **content-column:** Spacious primary editorial region using the page canvas.
- **right-rail:** Narrow supporting region separated from the main content by a light divider.
- **top-rule:** Thin purple structural accent above the lead content.
- **divider:** One-pixel light gray separator between story groups and rail sections.
- **surface:** Light gray grouped background for inactive or secondary controls.
- **tab-active:** Purple pill-shaped active segment with white uppercase interface text.
- **tab-inactive:** Light gray pill-shaped inactive segment with muted uppercase interface text.
- **button-primary:** Purple high-emphasis control with white interface text.
- **button-primary-hover:** Darker purple independent hover state with white text.
- **featured-story:** Large lead editorial composition combining an image, display heading, and serif summary.
- **featured-story-heading:** Largest bold sans-serif editorial headline.
- **story-list-item:** Stacked secondary story row with text and a trailing thumbnail.
- **story-list-heading:** Bold compact story headline.
- **story-summary:** Serif supporting copy in muted gray.
- **metadata:** Purple uppercase author or category treatment.
- **metadata-secondary:** Muted interface treatment for time, counts, or utility information.
- **image-score:** High-contrast purple score badge over an editorial image.
- **ad-placeholder:** Reserved advertising area using small muted interface text.
- **icon-control:** Minimal circular utility control on the white canvas.

## Do's and Don'ts

### Do

- Use purple selectively for active states, structural emphasis, and metadata accents.
- Preserve the contrast between bold sans-serif headlines and serif editorial summaries.
- Use whitespace and thin dividers to establish hierarchy instead of card shadows.
- Keep active and inactive segmented controls visually distinct.
- Reference visual values through tokens such as `{colors.primary}` and `{spacing.lg}`.

### Don't

- Do not use the primary color for large amounts of body copy.
- Do not replace serif summaries with the headline style.
- Do not add heavy borders, card shadows, or excessive rounding to editorial content.
- Do not place page-specific copy, names, imagery, or source identifiers in reusable components.
- Do not hardcode captured colors or nest interaction states inside a base component.
