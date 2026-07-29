# Czech Banking Customer and Transaction Analysis

An exploratory analysis of anonymized relational banking data covering customers, accounts, cards, loans, standing orders, and transactions.

The project moves from raw linked tables to decision-oriented questions about customer behavior, product usage, credit risk, and transaction flows.

## Questions explored

- How are customers and accounts distributed across districts?
- Which card products are most common, and who uses them?
- How do loan amount, duration, payment, and status relate?
- Which districts show a higher share of problematic loans?
- How do inflows, outflows, and interbank transfers change over time?

## Workflow

1. Load and inspect the related CSV tables.
2. Parse dates and standardize categorical values.
3. Join customer, account, district, card, loan, and transaction data.
4. Build descriptive summaries and visualizations.
5. Translate observed patterns into staffing, service, and risk-management considerations.

## Tools

Python, Pandas, NumPy, Matplotlib, Seaborn, and Plotly.

## Repository contents

- [Analysis notebook](Czech-banking-customer-trans-analysis.ipynb)
- `account.csv`, `card.csv`, `client.csv`, `disp.csv`, `district.csv`, `loan.csv`, `order.csv` — source tables
- [Data dictionary](<Data dictionary.pdf>)

## Run locally

```bash
git clone https://github.com/AyushUprety/banking-customer-analysis.git
cd banking-customer-analysis
jupyter notebook Czech-banking-customer-trans-analysis.ipynb
```

## Limitations

The dataset is historical and anonymized. The findings are descriptive, not a production credit-scoring system. Any lending or staffing decision would require current data, fairness testing, policy constraints, and review by qualified domain stakeholders.
