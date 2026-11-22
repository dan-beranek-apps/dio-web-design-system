# Typography

The system uses the existing Inter/system sans-serif stack for interface and reading text, with Georgia/Times for expressive display headings where a project already uses that editorial contrast.

## Core scale

| Token | Size | Intended use |
|---|---:|---|
| `--dio-font-size-body` | 16px | Main prose, descriptions and normal reading |
| `--dio-font-size-reading` | 15px | Dense card copy, table cells and supporting explanations |
| `--dio-font-size-compact` | 14px | Secondary interface copy and compact controls |
| `--dio-font-size-meta` | 13px | Metadata, navigation labels and non-essential context |
| `--dio-font-size-micro` | 12px | Short identifiers and decorative micro-labels only |

Pixel values describe the default browser setting (16px root). Use rem values so browser text preferences continue to work.

## Rules

1. Keep substantive explanations at 15–16px wherever layout permits.
2. Do not use 12–13px for paragraphs, instructions, table content or evidence descriptions.
3. Reserve the smallest tier for short labels, identifiers and metadata that remain understandable without being read as prose.
4. Do not rely on color or small text alone to communicate status.
5. Keep line height around 1.5–1.7 for reading content.
6. For narrow screens, allow content to wrap and cards to grow; do not reduce text size to preserve a fixed height.
7. Display headings have their own responsive scale and should not be enlarged as part of body-text accessibility adjustments.

## Accessibility testing

Review each consuming site at desktop and mobile widths. Check text resizing, keyboard focus, contrast, table overflow, visible labels and WAVE findings. A target size is a design guideline, not a guarantee of WCAG conformance: evaluate the actual rendered content and context.
