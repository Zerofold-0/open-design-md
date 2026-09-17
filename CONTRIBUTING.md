# Contributing

Thank you for helping maintain Open DESIGN.md. This repository focuses on reusable, actionable design rules rather than reproducing page copy or brand assets.

## Add a Design System

1. Create a lowercase kebab-case directory under `design-md/`, such as `design-md/example-product/`.
2. Name its entry file `DESIGN.md`.
3. Include a clear `version`, `name`, colors, typography, radii, spacing, and component tokens in the YAML front matter.
4. Use the Markdown body to describe the visual theme, key components, layout principles, interaction states, and design do's and don'ts.
5. Remove personal information, page-specific copy, URLs, logos, and non-reusable marketing content.
6. Add a relative link and a one-line description to the appropriate category in `README.md`.

## Update an Existing Document

- Validate colors, type sizes, spacing, and interaction rules against the current public interface.
- Prefer semantic tokens instead of repeating hard-coded visual values in component definitions.
- Express interaction states as sibling variants rather than nesting them inside base components.
- Keep each document independently understandable without requiring other repository files.
- If a visual language has distinct light and dark variants, they may use separate directories with the variant identified in each name.

## Pre-Submission Checklist

- The file path follows `design-md/<slug>/DESIGN.md`.
- The YAML front matter is enclosed by a pair of `---` delimiters.
- `name` identifies the design system and does not contain placeholder text.
- All README links work and the collection count is current.
- The document contains no personal data, credentials, or restricted assets.
