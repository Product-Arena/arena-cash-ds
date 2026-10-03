# Arena Cash design system

Small design system for the Arena Cash case: logo, colors, buttons, alerts, and a chart pattern.

It covers tokens, a few components, and one preview. It is not an npm package.

## Logo

`assets/logo/arena-cash.png` is the only Arena Cash logo in this repo.

It is copied from the AI Product Sense kit:

`learning/ai-product-sense/02-amplify/case-arena-cash/logo/arena-cash.png`

That file matches `guia-do-aluno/assets/logo-arena-cash.png` in the same course. Do not replace it with a logo from another course or from the `arena-cash` website repo.

## Preview

Open `preview/index.html` in a browser. No install step.

## Use in a page

```html
<link rel="stylesheet" href="tokens/tokens.css" />
<link rel="stylesheet" href="components/button.css" />
<link rel="stylesheet" href="components/alert.css" />
<link rel="stylesheet" href="components/chart.css" />
```

Paths are relative to your page. Adjust them if the files move.

## What is in scope

- Brand logo
- Color, type, and spacing tokens
- Button and alert
- How to build a bar chart and a line chart

Product screens, navigation, and inputs stay in the case documents. They are not components here.
