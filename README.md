# Finance Toolkit

Three small Python command-line tools for exploring loan amortisation, compound growth and exchange rates.

## Projects

| Script | What it does |
|---|---|
| `loan_calculator.py` | Calculates monthly repayments, an amortisation schedule and charts for a fixed-rate loan. |
| `compound_interest.py` | Compares contribution and return scenarios, with growth and sensitivity charts. |
| `currency_exchange_rate_tracker.py` | Fetches EUR/USD rates from Frankfurter, summarises historical observations and plots trends. |

## Run

Use Python 3.10 or newer. Install the dependencies:

```bash
python -m pip install pandas matplotlib requests
```

Run a tool from the repository folder:

```bash
python loan_calculator.py
python compound_interest.py
python currency_exchange_rate_tracker.py
```

The first two tools accept interactive inputs. The currency tracker also needs an internet connection to query the Frankfurter API.

## Assumptions and limits

The calculators use fixed rates and regular monthly contributions or payments. They do not model taxes, inflation, fees, changing rates, payment holidays or investment risk. Exchange-rate history uses the observations returned by Frankfurter; non-business days may have no published rate. The outputs are educational illustrations, not financial advice.
