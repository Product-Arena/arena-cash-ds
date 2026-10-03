# Arena Cash design system

Simplified spec for slides, dashboards, and mockups in the Arena Cash case. Arena Cash is a fictional account-and-card fintech used in Product Arena training.

## Logo

Canonical file: `assets/logo/arena-cash.png`.

Source of truth: the AI Product Sense case kit, `learning/ai-product-sense/02-amplify/case-arena-cash/logo/arena-cash.png`. The same file is also at `learning/ai-product-sense/guia-do-aluno/assets/logo-arena-cash.png`. If another course or repo ships a different mark, use this file.

- The wordmark in this file is near-black. Use it on light backgrounds.
- Clear space: at least 16px on every side.
- Minimum height on screen: 24px.
- Do not recolor, rotate, add a gradient, or redraw the mark.

## Color

| Token | Hex | Use |
| --- | --- | --- |
| `--ac-red` | `#FF494C` | Primary action, main chart series, logo |
| `--ac-black` | `#0A0A0A` | Headers, tooltip, dark surfaces |
| `--ac-white` | `#FFFFFF` | Default background |
| `--ac-gray-900` | `#141414` | Primary text |
| `--ac-gray-500` | `#7A7A7A` | Secondary text, comparison series |
| `--ac-gray-300` | `#D1D1D1` | Borders, axes |
| `--ac-success` | `#1FA05B` | Positive result |
| `--ac-danger` | `#D93434` | Negative result, error |
| `--ac-warning` | `#E08A1E` | Warning |
| `--ac-info` | `#2870E0` | Neutral information |

Red stays under about 15% of a screen. The default surface is light. Text on red or black is white.

## Type

- Display: Archivo, tight tracking (`-0.02em`).
- UI and numbers: Inter. Money uses tabular numbers.

## Components in this repo

| Piece | File |
| --- | --- |
| Tokens | `tokens/tokens.css` |
| Button | `components/button.css` (`primary`, `secondary`, `ghost`) |
| Alert | `components/alert.css` (`success`, `warning`, `danger`, `info`) |
| Chart | `components/chart.css` and `guidelines/charts.md` |

Open `preview/index.html` to see them together.
