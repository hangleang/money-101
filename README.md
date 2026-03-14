# Compound Interest Calculator

A clean, interactive compound interest calculator built with vanilla HTML, CSS, and JavaScript.

![Compound Interest Calculator](https://img.shields.io/badge/built%20with-HTML%2FCSS%2FJS-2d5a3d?style=flat-square)

## Features

- **Initial investment** — set a lump-sum starting amount
- **Monthly contributions** — see the impact of consistent saving
- **Adjustable rate & time horizon** — from 1% to 20%, up to 50 years
- **Compounding frequency** — yearly, monthly, weekly, or daily
- **Live chart** — visualizes balance vs. total contributed vs. initial-only growth
- **Breakdown bar** — shows how much of your final balance is principal, contributions, and interest

## Getting Started

### Run locally

No build step needed. Just open the file in your browser:

```bash
git clone https://github.com/your-username/compound-interest-calculator.git
cd compound-interest-calculator
open index.html
```

### Deploy to GitHub Pages

1. Push this repo to GitHub (must be public)
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch → main → / (root)**
4. Your site will be live at `https://your-username.github.io/compound-interest-calculator/`

## How It Works

The calculator uses the standard compound interest formula with regular contributions:

```
A = P(1 + r/n)^(nt) + PMT × [((1 + r/n)^(nt) - 1) / (r/n)]
```

Where:
- `A` = final balance
- `P` = principal (initial investment)
- `r` = annual interest rate (decimal)
- `n` = compounding periods per year
- `t` = time in years
- `PMT` = periodic payment (contribution per period)

## Tech Stack

- **HTML/CSS/JS** — zero build tooling
- **[Chart.js 4.4](https://www.chartjs.org/)** — loaded via CDN for the growth chart
- **[DM Serif Display + DM Mono](https://fonts.google.com/)** — via Google Fonts

## License

No License
