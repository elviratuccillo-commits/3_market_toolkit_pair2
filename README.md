# market-toolkit

A minimal toolkit for loading, cleaning, and computing metrics on financial time series.

Component B of MSA-DATI07-01 · Python Environments and Engineering Workflows.

## Team



- Partner A: Elvira Tuccillo
- Partner B: Claudia Jimenez

## Setup
1. Clone the repository
```bash
git clone https://github.com/elviratuccillo-commits/3_market_toolkit_pair2.git
```

2. Create the virtual environment 
```bash
python3 -m venv .venv
```
3. Activate the virtual environment 
```bash
source .venv/bin/activate
```
4. Install the dependencies 
```bash
pip install -r requirements.txt
```
5. Verify the installation:
```bash
pytest tests/ -v
```
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
- `src/` — Contains the core Python toolkit modules and execution pipeline. 
- `scripts/` — It contains the `fetch_prices.sh` script, which validates and summarizes the raw price data.
- `tests/` — It contains tests for the ingestion and metrics modules.

## Development workflow

Every change goes through a Pull Request. `main` stays green.

1. `git switch -c feature/<your-change>`
2. Do the work, commit as you go
3. Push, open a PR against `main`
4. Your partner reviews. You iterate. You merge when both are happy.
5. Never push directly to `main`.
