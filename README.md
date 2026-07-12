# Crypto & Gold Terminal

A live crypto/gold technical analysis panel that runs entirely in the browser, using Binance's public API. No login, no API key, no backend required.

## Features

- **Two-step asset picker:** choose a crypto asset first (Bitcoin, Ethereum, BNB, Solana, XRP, Dogecoin, Cardano, Toncoin, or a gold proxy via PAXG), then choose which currency to price it in.
- **Quote currency selector:** USDT (the most widely used quote currency in crypto trading globally) is selected by default, with USDC, TRY, EUR, GBP, and BRL also available.
- **Custom pair input:** type any Binance symbol directly (e.g. `AVAXUSDT`, `ETHEUR`) to override the dropdowns.
- Live candlestick chart with MA7 / MA25 / MA99 moving averages and a volume chart.
- A rule-based **signal gauge** (STRONG BUY / BUY / NEUTRAL / SELL / STRONG SELL) driven by RSI(14), momentum, moving-average alignment, and volume trend.
- An always-on **technical summary** written in plain English from the same indicators — no AI call, no external dependency.
- A scrolling ticker tape of major coins in your selected quote currency, refreshed every 30 seconds.
- Auto-refresh every 20 seconds (can be toggled off).

## Step-by-step: publish this on GitHub Pages

1. **Create a GitHub account** if you don't already have one (github.com — free).
2. **Create a new repository:**
   - Click the "+" in the top-right corner → "New repository".
   - Give it a name (e.g. `crypto-terminal`).
   - Set visibility to **Public**.
   - Click "Create repository".
3. **Upload the files:**
   - On the repo page, click "Add file" → "Upload files".
   - Drag and drop `index.html`, `README.md`, `LICENSE`, and the entire `fonts/` folder from this project.
   - Commit the changes.
4. **Turn on GitHub Pages:**
   - Go to **Settings** (top menu of the repo) → **Pages** (left sidebar).
   - Under "Branch", select `main` (or `master`), keep the folder as `/ (root)`, and click **Save**.
   - Wait 1–2 minutes — GitHub will give you a live link like:
     `https://YOUR-USERNAME.github.io/crypto-terminal/`
5. **Share the link.** Anyone can open it in their own browser — your computer doesn't need to stay on, and no one needs an account.

You can also just double-click `index.html` to open it locally in any modern browser to test it before publishing — it only needs an internet connection.

## Important notes

- **This is not financial advice.** The signal panel is a transparent, fixed rule set (moving-average alignment, RSI, momentum, volume trend) — it does not predict future price movement.
- **There's no direct gold spot pair on Binance**, so PAXG (Pax Gold, a token pegged to one troy ounce of gold) is used as a proxy. It can deviate slightly from spot gold prices.
- Binance's public API may be geo-restricted in some countries; if so, the tool will show an on-screen error rather than fail silently.
- Not every crypto/quote-currency combination exists on Binance (e.g. some altcoins may not have an EUR or BRL pair) — if you pick an unsupported combination, you'll see a clear error message.
- **This project is not affiliated with, endorsed by, or sponsored by Binance.** "Binance" is used only to describe the public data source.
- This project doesn't collect any personal data, and fonts are self-hosted (in the `fonts/` folder) instead of loaded from Google's font CDN, so no visitor data is sent to a third party just by opening the page.
- Please keep this free and non-commercial if you redistribute it — Binance's terms restrict commercial resale or paid/ad-supported services built on their market data.

## Repository contents

- `index.html` — the app itself (self-contained, no build step)
- `fonts/` — self-hosted Inter and JetBrains Mono font files (woff2)
- `README.md` — this file
- `LICENSE` — MIT license

## Contributing

Pull requests are welcome — additional indicators (MACD, Bollinger Bands), more quote currencies, or data from other exchanges would all be great additions.

## License

This project is licensed under the MIT License — see the `LICENSE` file for details. Feel free to use, modify, and redistribute it under those terms.

⚠️Warning: All my work is **experimental**! I can carefully examine the complaints and comments you may receive and put them into practice.⚠️
