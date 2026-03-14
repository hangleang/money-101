# Money 101

A pair of interactive financial literacy calculators in a single, self-contained HTML file.

![Built with HTML/CSS/JS](https://img.shields.io/badge/built%20with-HTML%2FCSS%2FJS-2d5a3d?style=flat-square)

---

## Tools

### 1 — Compound Interest Calculator
See how your money grows over time with interest compounding on top of itself.

- Set an initial investment and optional monthly contributions
- Adjust annual interest rate (1–20%) and time horizon (up to 50 years)
- Choose compounding frequency: yearly, monthly, weekly, or daily
- Live chart showing balance vs. total contributed vs. initial-only growth
- Breakdown bar showing what share of your final balance is principal, contributions, and interest

### 2 — Purchasing Power Erosion
See how inflation silently erodes what your cash can actually buy.

- Set any starting amount and inflation rate (0.5–20%)
- One-click historical presets: Fed target (2%), US average (3%), 2022 peak (6.5%), 1979 crisis (13.5%)
- Side-by-side display of today's value vs. real purchasing power in the future
- Equivalent goods breakdown (coffee, movie tickets, gas, groceries) so the erosion feels concrete
- Live chart of real value decay vs. nominal face value

---

## Getting Started

### Run locally

No build step needed — just open the file in your browser:

```bash
git clone https://github.com/hangleang/money-101.git
cd compound-interest-calculator
open index.html
```

### Deploy to GitHub Pages

1. Push this repo to GitHub (must be public)
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch → main → / (root)**
4. Your site will be live at `https://your-username.github.io/money-101/`

---

## How It Works

**Compound interest with contributions:**
```
Balance(y) = [Balance(y-1) × (1 + r/n) + PMT × (12/n)]  for each period
```

**Purchasing power (inflation-adjusted value):**
```
Real Value = Amount / (1 + inflation_rate)^years
```

Where `r` = annual rate, `n` = compounding periods per year, `PMT` = monthly contribution.

---

## Tech Stack

- **HTML/CSS/JS** — zero build tooling, single file
- **[Chart.js 4.4](https://www.chartjs.org/)** — loaded via CDN for live charts
- **[DM Serif Display + DM Mono](https://fonts.google.com/)** — via Google Fonts

---

## License

No License
