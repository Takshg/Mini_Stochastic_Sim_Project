# Mini Stochastic Simulation Project

This project implements two stochastic simulation concepts in R Markdown notebooks
with knitted PDF outputs:

1) Stochastic processes and long-run behavior in stock series
2) Markov transition modeling for discrete-state systems

## Project Structure

```
Mini_Stochastic/
├─ README.md
├─ stochastic_long_run.pdf
├─ stochastic_long_run.Rmd
├─ markov_transition_modeling.pdf
└─ markov_transition_modeling.Rmd
```

### File Descriptions

- `README.md` — project overview, setup, and usage notes.
- `stochastic_long_run.Rmd` — runnable report with code + outputs for long-run behavior.
- `stochastic_long_run.pdf` — knitted PDF output for long-run behavior.
- `markov_transition_modeling.Rmd` — runnable report with code + outputs for Markov models.
- `markov_transition_modeling.pdf` — knitted PDF output for Markov models.

## Requirements

- R (recommended 4.x)
- Base R packages
- `HMM` package (for FTSE regime modeling)

Install the HMM package if needed:

```
install.packages("HMM")
```

## How to Run

From an R console or RStudio, knit the `.Rmd` files:

```
stochastic_long_run.Rmd
markov_transition_modeling.Rmd
```

Each notebook produces plots and prints key numeric results to the console.

## Outputs

- ACF plots for returns and squared returns
- Simulated index series vs original series
- FTSE simulated end-value histogram and option pricing estimates
- Monopoly steady-state bar plot and expected revenue/cost summaries
- Reservoir steady-state distribution and annual cost exceedance probability

## Notes

- Random seeds are set for reproducibility.
- The EuStockMarkets dataset is included with base R.

## Credits

Inspired by DATA 405/505 (Stochastic Modelling and Simulation), University of British Columbia (UBC).
