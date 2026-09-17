# Open DESIGN.md

A collection of `DESIGN.md` documents for AI coding and design agents. Each document captures the visual language of a product or brand—including colors, typography, radii, spacing, component rules, and design guardrails—and can be placed directly in a project root for an agent to read.

This repository follows the organization of [VoltAgent/awesome-design-md](https://github.com/voltagent/awesome-design-md): all design systems live under `design-md/`, each system has its own directory, and every entry uses the standard `DESIGN.md` filename. Categories exist only in this index so that document links remain stable.

## How to Use

1. Choose a design direction from the collection below.
2. Copy its `DESIGN.md` into the root of your project.
3. Tell your AI agent: `Read DESIGN.md and implement the interface according to its design system.`

For example:

```bash
cp design-md/linear/DESIGN.md /path/to/your-project/DESIGN.md
```

`AGENTS.md` explains how to build the project. `DESIGN.md` explains how the interface should look and behave.

## Collection

The repository currently contains **28** design system documents.

### AI and Intelligent Products

- [Agentic Skills](design-md/agenticskills/DESIGN.md) — High-contrast monochrome, grid backgrounds, and terminal-inspired details
- [Claude](design-md/claude/DESIGN.md) — Warm paper surfaces, serif headings, and terracotta accents
- [ElevenLabs](design-md/elevenlabs/DESIGN.md) — Restrained monochrome UI, lightweight headings, and generous whitespace
- [OpenAI](design-md/openai/DESIGN.md) — Neutral black and white, clear typography, and soft violet accents
- [xAI Dark](design-md/xai-dark/DESIGN.md) — Dark minimalist surfaces with a high-contrast information hierarchy
- [xAI Light](design-md/xai-light/DESIGN.md) — Light minimalist surfaces with violet, coral, and gold accents

### Developer Tools and Browsers

- [Arc](design-md/arc/DESIGN.md) — Cream canvas, soft typography, and blue action elements
- [Cursor](design-md/cursor/DESIGN.md) — Warm-gray canvas, quiet hierarchy, and a code-tool aesthetic
- [Dia](design-md/dia/DESIGN.md) — Black canvas, editorial typography, and understated surface layers
- [Linear](design-md/linear/DESIGN.md) — Precise dark UI, compact typography, and subtle borders

### Design Resources and Systems

- [Material Design](design-md/material-design/DESIGN.md) — Dark surfaces, violet accents, and clear component hierarchy
- [Mobbin](design-md/mobbin/DESIGN.md) — Large product typography, monochrome structure, and indigo accents

### Productivity and SaaS

- [Slack](design-md/slack/DESIGN.md) — Signature purple, friendly typography, and bright content areas
- [Zapier](design-md/zapier/DESIGN.md) — Warm canvas, vivid orange, and editorial display type

### Fintech

- [Stripe](design-md/stripe/DESIGN.md) — Deep-blue text, violet actions, and refined light surfaces
- [Wise](design-md/wise/DESIGN.md) — Bright-green canvas, deep-green text, and strongly rounded forms

### E-commerce, Retail, and Lifestyle

- [Airbnb](design-md/airbnb/DESIGN.md) — Coral accents, card-based content, and friendly radii
- [Alo](design-md/alo/DESIGN.md) — Fashion-focused monochrome, restrained borders, and clear commerce hierarchy
- [IKEA](design-md/ikea/DESIGN.md) — Yellow primary color, playful color blocks, and spacious image-led layouts
- [Nike](design-md/nike/DESIGN.md) — Strong monochrome, oversized headings, and image-first composition
- [Shopify](design-md/shopify/DESIGN.md) — Cinematic dark canvas, light typography, and pill-shaped actions
- [Starbucks](design-md/starbucks/DESIGN.md) — Signature green, clear hierarchy, and rounded controls

### Consumer Technology, Media, and Mobility

- [Apple](design-md/apple/DESIGN.md) — Minimal monochrome, system typography, and image-led presentation
- [Meta](design-md/meta/DESIGN.md) — Bright canvas, Meta blue, and spacious information architecture
- [Spotify](design-md/spotify/DESIGN.md) — Dark music UI, vivid green, and oversized headings
- [The Verge](design-md/the-verge/DESIGN.md) — Editorial typography, violet accents, and high content density
- [Uber](design-md/uber/DESIGN.md) — Strong monochrome, urban typography, and functional layouts

### Automotive

- [Tesla](design-md/tesla/DESIGN.md) — Minimal UI, blue action elements, and image-driven presentation

## Document Conventions

Each `DESIGN.md` has two parts:

- YAML front matter containing reusable color, typography, radius, spacing, and component tokens.
- A Markdown body describing the visual theme, components, layout principles, interaction states, and design do's and don'ts.

Directory names use lowercase kebab-case, and every entry file is named `DESIGN.md`. Read [CONTRIBUTING.md](CONTRIBUTING.md) before adding or modifying a document.

## Disclaimer

These documents are derived from publicly visible interfaces and are intended for learning, prototyping, and helping AI agents generate visually consistent interfaces. All brand names and trademarks belong to their respective owners. These documents are not official design guidelines and do not imply endorsement by the referenced brands.
