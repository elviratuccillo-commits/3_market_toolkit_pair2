# market-toolkit

A minimal toolkit for loading, cleaning, and computing metrics on financial time series.

Component B of MSA-DATI07-01 · Python Environments and Engineering Workflows.

## Team

<!-- TODO (both partners): add your names below, one line each. -->
<!-- This is one of the shared files — you WILL hit a merge conflict here. That is expected. -->

- Partner A: _your name here_
- Partner B: Claudia Jimenez

## Setup

<!-- TODO (Partner A): write the exact commands a new teammate would run to get -->
<!-- from a fresh clone to a working environment. Assume they have Python 3.11+. -->

## How to run

To validate and log the raw data, run the fetch script:
`bash scripts/fetch_prices.sh`
*Produces:* A console summary of rows per ticker and a dated log file in the `logs/` directory.

To calculate financial metrics and generate the performance chart, run the demo:
`python -m src.demo`
*Produces:* A printed risk-adjusted performance summary for each ticker and saves a cumulative wealth chart to `outputs/cumulative_returns.png`.

## Structure

<!-- TODO (both): describe what each folder is for. Keep it short — 1 line each. -->

- `data/raw/` — Contains the original finacial CSV datasets.
- `src/` — Contains the core Python toolkit modules 
- `scripts/` —
- `tests/` —

## Development workflow

Every change goes through a Pull Request. `main` stays green.

1. `git switch -c feature/<your-change>`
2. Do the work, commit as you go
3. Push, open a PR against `main`
4. Your partner reviews. You iterate. You merge when both are happy.
5. Never push directly to `main`.
