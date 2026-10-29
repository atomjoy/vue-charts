# Vue Chart

Minimal SVG and shadcn vue charts.

## Tailwind

```css
/* Custom colors */
@theme {
	/* Accent */
	/* --color-accent: #7ee100; */

	/* Własny kolor text-custom, bg-custom border-custom, ... */
	--color-custom: #fdc50a;
	--color-custom-txt: #ffffff;

	/* Dla hovera:text-custom-dark-txt, hovera:bg-custom-dark */
	--color-custom-dark: #fed317;
	--color-custom-dark-txt: #000000;

	/* Chart colors (shadcn) */
	--color-chart-1: #0099ff;
	--color-chart-2: #fdc50a;
	--color-chart-3: #7ee100;
}
```
## Data

```js
const mockData = ref<ChartDataPoint[]>([
	{ label: 'Styczeń', value: 35 },
	{ label: 'Luty', value: 55 },
	{ label: 'Marzec', value: 42 },
	{ label: 'Kwiecień', value: 85 },
	{ label: 'Maj', value: 67 },
	{ label: 'Czerwiec', value: 92 },
])

const myMultiSeriesData = ref<ChartSeries[]>([
	{
		name: 'Przychody',
		lineColor: 'stroke-blue-500',
		dotStrokeColor: 'stroke-blue-500',
		dotFillHoverColor: 'fill-blue-600',
		data: [
			{ label: 'Pon', value: 30 },
			{ label: 'Wt', value: 45 },
			{ label: 'Śr', value: 35 },
			{ label: 'Czw', value: 70 },
			{ label: 'Pt', value: 55 },
		],
	},
	{
		name: 'Koszty',
		lineColor: 'stroke-lime-500',
		dotStrokeColor: 'stroke-lime-500',
		dotFillHoverColor: 'fill-lime-600',
		data: [
			{ label: 'Pon', value: 15 },
			{ label: 'Wt', value: 20 },
			{ label: 'Śr', value: 25 },
			{ label: 'Czw', value: 30 },
			{ label: 'Pt', value: 22 },
		],
	},
	{
		name: 'Zysk netto',
		lineColor: 'stroke-fuchsia-500',
		dotStrokeColor: 'stroke-fuchsia-500',
		dotFillHoverColor: 'fill-fuchsia-600',
		data: [
			{ label: 'Pon', value: 15 },
			{ label: 'Wt', value: 25 },
			{ label: 'Śr', value: 10 },
			{ label: 'Czw', value: 40 },
			{ label: 'Pt', value: 33 },
		],
	},
])
```
