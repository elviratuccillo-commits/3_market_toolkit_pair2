# market-toolkit

A minimal toolkit for loading, cleaning, and computing metrics on financial time series.

Component B of MSA-DATI07-01 · Python Environments and Engineering Workflows.

## Team



- Partner A: Elvira Tuccillo
- Partner B: _your name here_

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

<!-- TODO (Partner B): describe how to run  scripts/fetch_prices.sh  and  src/demo.py . -->
<!-- Include what output files each command produces. -->

## Structure

<!-- TODO (both): describe what each folder is for. Keep it short — 1 line each. -->

- `data/raw/` —
- `src/` —
- `scripts/` — It contains the `fetch_prices.sh` script, which validates and summarizes the raw price data.
- `tests/` —

## Development workflow

Every change goes through a Pull Request. `main` stays green.

1. `git switch -c feature/<your-change>`
2. Do the work, commit as you go
3. Push, open a PR against `main`
4. Your partner reviews. You iterate. You merge when both are happy.
5. Never push directly to `main`.
