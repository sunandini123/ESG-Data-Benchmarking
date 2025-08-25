
# ESG Data Benchmarking (Independent Project)

**Goal:** Benchmark companies on Environmental, Social, and Governance (ESG) factors and surface leaders/laggards by sector.

## Data & Method
- Source: Public ESG dataset (company-level emissions, diversity, and governance fields).
- Cleaning: Basic null handling + consistent column naming.
- Scoring: Normalize E, S, G to 0–100; composite ESG = 0.4*E + 0.3*S + 0.3*G (tunable).
- Outputs: Top 10 companies, sector averages, comparison charts.

## What’s Inside
- `data/` – raw CSV (redacted sample acceptable).
- `notebooks/esg_benchmarking.ipynb` – code to clean, score, and plot.
- `outputs/` – charts (`top10_esg.png`, `sector_esg_by_sector.png`, etc.), scored dataset, and optional Power BI:
  - `ESG_Benchmarking.pbix`
  - `ESG_Benchmarking.pdf`

## Findings (example)
- High-ESG firms cluster in **{your best sector}**; **{another sector}** shows improvement opportunity in **E**.
- Diversity (S) correlates with higher composite ESG in the sample.

## How to Reproduce
1. Clone repo.
2. Put a CSV in `data/` with columns: `Company, Sector, Country, Emissions_tCO2e, Diversity_Pct, Governance_Score`.
3. Run `notebooks/esg_benchmarking.ipynb`.

## License
Personal/educational use.
