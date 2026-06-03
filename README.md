# Office Blues — Misery Data

Open data on the cost of work. Two datasets, both derived from public sources, maintained by **[Office Blues](https://officeblues.net)** — a media-and-tools project for the unhappily employed.

> Free to use under **CC BY 4.0**. Quote a figure, build on it, cite us.

## Datasets

### `data/occupation_wages.csv` — U.S. occupation annual wages (n = 823)
Annual wage percentiles (25th, median, 75th, 90th) for 823 detailed U.S. occupations.

| field | meaning |
|---|---|
| `soc` | Standard Occupational Classification (SOC 2018) code |
| `title` | Occupation title |
| `p25_usd` / `median_usd` / `p75_usd` / `p90_usd` | Annual wage percentiles, USD |
| `source_url` | The Office Blues page for this occupation |

**Source:** U.S. Bureau of Labor Statistics, [Occupational Employment and Wage Statistics (OEWS)](https://www.bls.gov/oes/), May 2025 release. Wages are national.

### `data/city_burnout_index.csv` — City burnout index (n = 50)
A composite "burnout" score (0–100, higher = worse) for the 50 largest U.S. metro areas, ranked worst-first.

| field | meaning |
|---|---|
| `cbsa_code` | Census CBSA code |
| `city` / `state` | Metro area / state |
| `population` | Metro population |
| `burnout_score` | Composite score, 0–100 |
| `rank` / `of_cities` | Rank (1 = worst) of 50 |
| `source_url` | The Office Blues page for this metro |

**Methodology:** the burnout score is a composite of public metro-level indicators; the full method is documented at **[officeblues.net/methodology](https://officeblues.net/methodology)**. Treat it as an editorial index (v1), not an official statistic.

## Files
- `data/*.csv` and `data/*.json` — the same data in both formats.
- `datapackage.json` — a [Frictionless Data](https://frictionlessdata.io/) descriptor (schemas + licensing).

## Cite this dataset
```
Office Blues, "Misery Data" (occupation wages + city burnout index),
officeblues.net, CC BY 4.0.
```

## About
Maintained by Office Blues — **<https://officeblues.net>**. Methodology and the underlying tools (e.g. the Meeting Tax Calculator) live there. Aggregates only; no personal or per-visitor data is included.
