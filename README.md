# Dividend Compounding Calculator

Model how reinvested dividends, ongoing contributions, and price appreciation compound over many years. The tool runs entirely in your browser and reports final portfolio value, total dividends received, and yield on cost, with a DRIP toggle to compare reinvesting against taking dividends as cash.

**Live demo:** https://0xelitesystem.github.io/dividend-compounding-calculator/

**Not financial advice.** This assumes fixed yield, dividend growth, and appreciation rates that no real holding maintains. It is a teaching tool for the mechanics of dividend compounding, not a projection of any specific investment.

## What it does

The Dividend Compounding Calculator simulates a dividend portfolio month by month. Each month it applies price appreciation, adds your contribution, pays a dividend based on the current share count and a growing dividend per share, and either reinvests that dividend or sets it aside as cash depending on the DRIP toggle. It then reports the ending value, the total dividends paid across the horizon, and the yield on cost at the end.

Yield on cost is the ending annual dividend income divided by everything you contributed. It shows how a modest starting yield can grow into a large income stream on the original money when dividends rise over time.

## How to use it

1. Open `index.html` in a browser, or visit the GitHub Pages site.
2. Enter the initial investment, monthly contribution, starting yield, annual dividend growth, annual price appreciation, and horizon in years.
3. Toggle DRIP on to reinvest dividends or off to take them as cash.
4. Read the final value, total dividends, and yield on cost. The stacked chart separates contributions, dividends, and appreciation.

## Inputs and outputs

| Input | Meaning |
| --- | --- |
| Initial investment | Starting capital |
| Monthly contribution | Added each month, buying at the current price |
| Starting dividend yield | First-year yield on the starting price |
| Annual dividend growth | Yearly rate the dividend per share grows |
| Annual price appreciation | Yearly rate the share price grows |
| Horizon | Length of the simulation in years |
| DRIP | Reinvest dividends, or hold them as cash |

## Method and assumptions

Price compounds monthly from appreciation. Dividend per share is based on the starting price times yield, stepped up each year by the growth rate, and paid monthly. With DRIP on, each dividend buys fractional shares at the current price. There are no taxes, fees, or dividend cuts. Rates are held constant, which is why the output should be read as a mechanic, not a forecast.

## Privacy

Runs fully client side. No analytics, no network calls, no storage.

## Related tools

- [dca-visualizer](https://github.com/0xelitesystem/dca-visualizer)
- [position-sizing-calculator](https://github.com/0xelitesystem/position-sizing-calculator)
- [real-return-calculator](https://github.com/0xelitesystem/real-return-calculator)

## License

MIT. Copyright 0xelitesystem 2026.
