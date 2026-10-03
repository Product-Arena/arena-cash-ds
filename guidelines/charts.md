# Charts

Arena Cash charts show money and rates. The number is the hero. Color only marks the series or the result.

## Series

| Role | Token | Rule |
| --- | --- | --- |
| Main series | `--ac-red` | 2px line, or solid bars |
| Comparison (CDI, previous period) | `--ac-gray-500` | 1.5px dashed line, or `--ac-gray-300` bars |
| Area under the main line | `--ac-red` at 10% opacity | One fill, under the main series only |
| Axes and grid | `--ac-gray-300` | Hairline. Labels use 12px Inter, `--ac-gray-500` |
| Gain | `--ac-success` | The delta text, not the whole chart |
| Loss | `--ac-danger` | The delta text, not the whole chart |

Brand red is the product series. Green and red semantic colors are only for up and down. Do not paint a bar green because the month was good.

## Numbers

- Use Inter with `font-variant-numeric: tabular-nums`.
- Currency in BRL: `R$ 1.240,00`.
- Rates with one decimal and a sign when it is a change: `+1,2%`, `-0,4%`.
- No italics on numbers.

## Tooltip

Background `--ac-black`, text `--ac-white`, value in tabular numbers. One tooltip, anchored to the point.

## How to build one

1. Wrap the chart in `.ac-chart`.
2. Put the title in `.ac-chart__title`.
3. For bars, set each `.ac-chart__bar` height as a percentage of the tallest value in the set. The comparison bar uses `.ac-chart__bar--compare`.
4. For a line, use one SVG. The main path is `.ac-chart__series`. The benchmark path is `.ac-chart__series--compare`. The area is `.ac-chart__area`.
5. Put the result next to the title with `.ac-chart__value--up` or `.ac-chart__value--down`.

See `preview/index.html` for a bar chart and a line chart that follow these classes.

## Do not

- Use more than two series on the first version of a chart.
- Use a rainbow palette, gradients, or 3D.
- Encode the result only with color. The label carries the number.
