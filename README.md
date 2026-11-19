[![Portfolio validation](https://github.com/Mrroof/financial-modelling-forecasting/actions/workflows/portfolio-validation.yml/badge.svg)](https://github.com/Mrroof/financial-modelling-forecasting/actions)

# Financial Modelling and Forecasting

> **Portfolio case study · Excel · scenario analysis · bank operating model**

## Executive summary
A formula-driven 12-month bank operating model that compares downside, base and upside assumptions. The workbook demonstrates how balance-sheet growth, lending yields, deposit funding costs, fee income, operating expenses and impairment can flow through to illustrative profit before tax.

## Business question
How sensitive is projected bank profitability to changes in deposit growth, loan growth, pricing, fee income, operating expenses and impairment?

## Workbook
`model/financial_scenario_model.xlsx`

## Workbook map
| Sheet | Purpose |
|---|---|
| Assumptions | Starting values and scenario selector |
| Scenarios | Downside, base and upside driver assumptions |
| Operating Model | Twelve monthly operating projections |
| Guide | Instructions, definitions and limitations |

## How to use
1. Open the workbook in Excel or a compatible spreadsheet application.
2. Select `Downside`, `Base` or `Upside` in `Assumptions!B2`.
3. Replace illustrative opening balances with appropriately sourced figures.
4. Review and adjust assumptions on the Scenarios sheet.
5. Review monthly deposits, loans, interest income, interest expense, net interest income, fees, expenses, impairment and profit before tax.

## Core calculation logic
- Closing deposits = opening deposits × (1 + deposit growth)
- Closing loans = opening loans × (1 + loan growth)
- Monthly interest income = closing loans × lending yield ÷ 12
- Monthly interest expense = closing deposits × deposit cost ÷ 12
- Net interest income = interest income − interest expense
- Profit before tax = net interest income + fee income − operating expenses − impairment

## Analytical considerations
A robust bank model should document assumption sources and dates, distinguish average from closing balances, model repricing and maturity profiles, account for non-performing loans and impairment methodology, and test sensitivities. This workbook is a learning template rather than a fully validated bank forecast.

## Data and usage notice
All opening balances and assumptions are illustrative, not actual bank figures or forecasts. Do not use the workbook for business decisions without replacing assumptions, checking formula logic against accounting policies and validating outputs with qualified reviewers.

## Repository structure

```text
model/financial_scenario_model.xlsx   # Main scenario-driven workbook
.github/workflows/                    # Automated workbook validation
```

## Review checklist

Before adapting the workbook for a real organisation, confirm the period conventions, opening-balance definitions, interest calculation basis, scenario assumptions, and links between schedules. Recalculate the workbook in a spreadsheet application after changing assumptions and independently review key formulas.
