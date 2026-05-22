# NepseDataHome

<div align="center">

# 📈 NepseDataHome

### The Open Data Infrastructure for Nepal's Capital Markets

Historical, fundamental, technical, and market-wide datasets for the Nepal Stock Exchange (NEPSE), designed for researchers, investors, quantitative analysts, students, and developers.

[Features](#features) •
[Datasets](#datasets) •
[Research](#research-applications) •
[Installation](#installation) •
[Contributing](#contributing)

</div>

---

## Overview

NepseDataHome is a comprehensive data platform focused on collecting, organizing, validating, and serving Nepal Stock Exchange (NEPSE) market data.

The project aims to solve one of the largest challenges in Nepal's financial ecosystem:

> Lack of accessible, structured, research-ready market data.

Instead of scattered spreadsheets, manually downloaded reports, and fragmented data sources, NepseDataHome provides a unified repository of market information that can be used for:

- Quantitative research
- Algorithmic trading research
- Portfolio analysis
- Academic studies
- Financial journalism
- Machine learning
- Time-series forecasting
- Market surveillance
- Investment research

---

# Why NepseDataHome Exists

Nepal's capital market has experienced significant growth over the past decade.

However, access to clean, structured, machine-readable datasets remains limited.

Researchers often spend more time collecting data than analyzing it.

NepseDataHome aims to become:

- Nepal's largest open market dataset
- A foundation for quantitative finance research
- A source for AI and machine learning projects
- A public resource for students and researchers
- A developer-friendly market data platform

---

# Features

## Historical Market Data

Access historical trading information across listed securities.

Includes:

- Open price
- High price
- Low price
- Close price
- Last traded price
- Volume traded
- Turnover
- Number of transactions

---

## Company Information

Structured information for listed companies.

Examples:

- Symbol
- Company name
- Sector
- Listing information
- Market category

---

## Sector Analysis

Analyze performance across sectors.

Examples:

- Commercial Banks
- Hydropower
- Microfinance
- Life Insurance
- Non-Life Insurance
- Hotels & Tourism
- Finance
- Manufacturing
- Investment

---

## Market Indices

Track historical performance of:

- NEPSE Index
- Sensitive Index
- Float Index
- Sector Indices

---

## Corporate Actions

Repository for:

- Bonus shares
- Cash dividends
- Rights offerings
- FPOs
- Mergers
- Acquisitions
- Stock splits

---

## Fundamental Data

Financial indicators including:

- EPS
- Book Value
- Net Worth
- Dividend History
- PE Ratio
- Market Capitalization

---

## Research Ready

Data is organized for:

- Python
- R
- SQL
- Excel
- Power BI
- Tableau

---

# Dataset Structure

```text
NepseDataHome/

├── data/
│   ├── companies/
│   ├── prices/
│   ├── sectors/
│   ├── indices/
│   ├── fundamentals/
│   ├── dividends/
│   ├── rights/
│   ├── announcements/
│   └── market_summary/
│
├── notebooks/
│   ├── analysis/
│   ├── forecasting/
│   ├── machine_learning/
│   └── visualization/
│
├── scripts/
│   ├── collectors/
│   ├── cleaners/
│   ├── validators/
│   └── exporters/
│
├── api/
│
├── docs/
│
└── README.md
```

---

# Available Data Categories

| Category | Description |
|-----------|------------|
| Daily Prices | Historical OHLCV data |
| Indices | Market and sector indices |
| Fundamentals | Financial statements and ratios |
| Dividends | Dividend distributions |
| Rights Shares | Rights issue history |
| Market Summary | Daily market statistics |
| Corporate Actions | Events affecting securities |
| Sector Data | Industry classifications |
| Company Profiles | Listed company metadata |

---

# Research Applications

NepseDataHome can support:

## Quantitative Finance

- Momentum strategies
- Mean reversion
- Factor investing
- Portfolio optimization
- Risk modelling

---

## Machine Learning

- Price prediction
- Volatility forecasting
- Classification models
- Regime detection
- Market anomaly detection

---

## Academic Research

Potential areas:

- Market efficiency
- Behavioral finance
- Emerging markets research
- Liquidity studies
- Event studies

---

## Data Journalism

Useful for:

- Election-related economic coverage
- Market investigations
- Corporate reporting
- Economic trend analysis

---

# Example Use Cases

## Loading Historical Data

```python
import pandas as pd

df = pd.read_csv("data/prices/NABIL.csv")

print(df.head())
```

---

## Calculate Returns

```python
df["returns"] = df["close"].pct_change()
```

---

## Moving Average

```python
df["ma50"] = df["close"].rolling(50).mean()
```

---

## Sector Performance Analysis

```python
sector_returns = (
    df.groupby("sector")
      .returns
      .mean()
)
```

---

# Future Roadmap

## Phase 1

- Historical market datasets
- Company metadata
- Sector classification
- Data validation pipeline

## Phase 2

- Public API
- Automated updates
- Data explorer dashboard
- Download center

## Phase 3

- Real-time feeds
- Quantitative research toolkit
- Portfolio analytics
- Screening engine

## Phase 4

- AI-powered market assistant
- Research paper generation
- Forecasting models
- Institutional datasets

---

# Who Is This For?

### Students

Learning finance, economics, and data science.

### Researchers

Studying emerging capital markets.

### Investors

Analyzing listed companies.

### Journalists

Investigating financial stories.

### Developers

Building market tools and applications.

### Data Scientists

Training predictive models.

---

# Contributing

Contributions are welcome.

Areas where contributors can help:

- Data validation
- Historical data collection
- Documentation
- API development
- Visualization tools
- Research notebooks

---

# Citation

If you use NepseDataHome in research:

```bibtex
@dataset{nepsedatahome,
  title={NepseDataHome},
  author={Sakshyam Banjade},
  year={2026},
  publisher={GitHub},
  url={https://github.com/sakshyambanjade/NepseDataHome}
}
```

---

# License

MIT License

See LICENSE for details.

---

# Author

**Sakshyam Banjade**

AI Researcher • Quantitative Systems Builder • Developer

GitHub:
https://github.com/sakshyambanjade

Project:
https://github.com/sakshyambanjade/NepseDataHome

---

## Vision

To become the most comprehensive open data platform for Nepal's capital markets and enable the next generation of quantitative finance, AI research, and investment analysis in Nepal.
