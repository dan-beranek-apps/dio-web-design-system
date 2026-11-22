# DIO Web Design System

A small, versioned design foundation for the web properties and tools maintained in the DIO/ODI ecosystem.

The system is **shared at the foundation level, not as a universal page template**. It standardizes design tokens, semantic reading-text colors, typography and opt-in long-form content primitives while leaving each project's information architecture, layouts, diagrams and domain-specific components independent.

## Principles

- Preserve each site's established visual identity and information architecture.
- Keep body copy comfortably readable; reserve compact sizes for metadata, not substantive explanations.
- Use shared design tokens for color, type, spacing, borders and shape.
- Keep site-specific CSS in the consuming project.
- Vendor a pinned copy of the CSS into each site. A deployed site must not depend on this repository or GitHub being available at runtime.
- Make upgrades explicit and reviewable through versioned changes.

## Repository structure

- `src/tokens.css` — canonical design tokens.
- `src/prose.css` — optional long-form content primitives.
- `dist/dio-core.css` — ready-to-vendor stylesheet containing the foundation.
- `docs/typography.md` — typographic scale and usage guidance.
- `VERSION` — current source version.
- `CHANGELOG.md` — release history.

## Use in a project

1. Copy `dist/dio-core.css` into the project's own assets, for example `assets/design-system/dio-core.css`.
2. Load it before the project's site-specific accessibility/typography overrides.
3. Keep page layouts, branded hero sections, data visualizations and unique components in the project's own stylesheet.
4. Record the imported version in the project's design-system metadata or changelog.
5. Test desktop and mobile layouts, keyboard focus, text resizing, table overflow and contrast before deployment.

The CSS is dependency-free and does not load fonts, scripts or external assets.

## Versioning

The initial foundation is `0.1.0`. Until it has been validated across multiple sites, changes may refine tokens and semantics. Once adopted by more than one project, changes that affect existing token meanings should be treated as compatibility-sensitive.

## Licensing

The repository is public for inspection and collaboration. No separate open-source reuse license has been assigned at this stage; public visibility alone does not grant permission to redistribute or reuse the source.
