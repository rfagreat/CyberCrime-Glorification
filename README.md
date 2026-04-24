# 🔓 What's There to Flex? — Cybercrime Glorification & Youth Radicalisation

> **A Systematic Literature Review on the Cultural Glorification of Cybercrime and Its Role in Youth Radicalisation Toward Cybercriminal Activity**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![PRISMA 2020](https://img.shields.io/badge/Method-PRISMA%202020-blue.svg)](http://www.prisma-statement.org/)
[![Studies: 71](https://img.shields.io/badge/Included%20Studies-71-green.svg)](#key-findings)
[![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-yellow.svg)](https://www.python.org/)

---

## Abstract

No other category of crime enjoys the cultural prestige afforded to cybercrime. While drug trafficking, gang violence, and financial fraud face cultural stigmatisation, cybercrime benefits from a distinctive **"flex culture"** where perpetrators are praised across social media, entertainment, and digital subcommunities. This systematic literature review examines the phenomenon of cybercrime glorification and its influence on youth radicalisation toward cybercriminal activity, employing the **PRISMA 2020 framework**.

The review synthesises evidence from **71 studies** (1990–2026), drawn from an initial pool of **917 records** across five databases, across five thematic domains:

1. Hacker subculture and identity construction
2. Media portrayals of cybercrime in film and television
3. Social media as a platform for cybercrime glorification
4. Youth pathways into cybercriminal activity
5. Criminological theories applied to cybercrime motivation

---

## Key Findings

| Metric | Value |
|--------|-------|
| Records exported | 917 |
| Unique records screened | 853 |
| Final included studies | 71 |
| Year range | 1990–2026 |
| Studies from 2020 onwards | 40 (56.3%) |
| Databases searched | 5 (Google Scholar, ACM, IEEE, Scopus, WoS) |

### Glorification Level Distribution

| Level | Count | % |
|-------|-------|---|
| Tangential | 26 | 36.6% |
| Peripheral | 21 | 29.6% |
| Central | 17 | 23.9% |
| Absent | 7 | 9.9% |

### Crime Type Distribution

| Type | Count | % |
|------|-------|---|
| Cybercrime (general) | 47 | 66.2% |
| Cybercrime (fraud) | 16 | 22.5% |
| Hacktivism | 3 | 4.2% |
| Gang culture | 2 | 2.8% |
| Crime (general) | 2 | 2.8% |
| Terrorism | 1 | 1.4% |

---

## Repository Structure

```
├── README.md                          ← You are here
├── LICENSE                            ← CC BY 4.0 license
├── data/
│   └── SLR_71_Studies_FINAL.xlsx      ← Complete dataset (all 853 records + final 71)
├── notebooks/
│   └── SLR_Analysis.ipynb             ← Google Colab notebook with all analyses
├── figures/                           ← Generated charts and visualisations
│   ├── 01_PRISMA_flow_diagram.png
│   ├── 02_publication_year_distribution.png
│   ├── 03_database_contribution.png
│   ├── 04_study_design_distribution.png
│   ├── 05_crime_type_distribution.png
│   ├── 06_glorification_level.png
│   ├── 07_geographic_distribution.png
│   ├── 08_glorification_crimetype_heatmap.png
│   ├── 09_glorification_design_heatmap.png
│   ├── 10_temporal_glorification_evolution.png
│   ├── 11_top_journals.png
│   ├── 12_word_cloud_titles.png
│   └── 14_dashboard_key_findings.png
├── docs/
│   ├── SEARCH_STRATEGY.md             ← Search queries and database strategy
│   ├── PRISMA_CHECKLIST.md            ← PRISMA 2020 compliance checklist
│   └── CODEBOOK.md                    ← Variable definitions and coding scheme
├── scripts/
│   └── generate_figures.py            ← Standalone script to regenerate all figures
└── .gitignore
```

---

## Analyses Included

The Colab notebook (`notebooks/SLR_Analysis.ipynb`) produces **14 analyses**:

| # | Analysis | Description |
|---|----------|-------------|
| 1 | PRISMA Flow Diagram | Full screening pipeline: 917 → 853 → 571 → 329 → 71 |
| 2 | Publication Year Distribution | Temporal trends with cubic trend line |
| 3 | Database Contribution | Pie charts comparing all records vs. final included |
| 4 | Study Design Distribution | Methodology breakdown (Qualitative leads at 21.1%) |
| 5 | Crime Type Distribution | Pie chart of crime categories |
| 6 | Glorification Level | Consolidated + detailed bar charts |
| 7 | Geographic Distribution | Colour-coded by region |
| 8 | Glorification × Crime Type | Heatmap crosstabulation |
| 9 | Glorification × Study Design | Heatmap crosstabulation |
| 10 | Temporal Evolution | Stacked bars showing glorification trends over time |
| 11 | Top Journals/Sources | Ranked bar chart |
| 12 | Word Cloud | From all 71 study titles |
| 13 | Summary Statistics | Full text report |
| 14 | Combined Dashboard | 6-panel overview |

---

## Quick Start

### Option 1: Google Colab (Recommended)

1. Open `notebooks/SLR_Analysis.ipynb` in [Google Colab](https://colab.research.google.com)
2. Upload `data/SLR_71_Studies_FINAL.xlsx` when prompted
3. Uncomment the install and upload cells
4. Run all cells

### Option 2: Local Environment

```bash
git clone https://github.com/YOUR_USERNAME/cybercrime-glorification-slr.git
cd cybercrime-glorification-slr

pip install pandas numpy matplotlib seaborn openpyxl wordcloud

python scripts/generate_figures.py
# OR
jupyter notebook notebooks/SLR_Analysis.ipynb
```

---

## Theoretical Framework

This review applies two primary criminological lenses:

- **Differential Association Theory** (Sutherland) — criminal behaviour is learned through interaction with others who frame it positively
- **Social Learning Theory** (Bandura) — media glorification acts as vicarious reinforcement; the "flex culture" provides social proof that cybercrime leads to status and prestige

---

## Identified Research Gap

A critical finding of this review is that **no existing study provides an integrated, global-level framework treating glorification as an independent variable in youth cybercrime radicalisation**. While individual studies address fragments (hacker subculture, Nigerian fraud glamorisation, media portrayals), the synthesis reveals this as a fragmented field in need of a unifying model.

---

## Search Strategy

Three search strings (S1, S2, S3) were applied across five databases:

| Query | Focus | Databases |
|-------|-------|-----------|
| S1 | Cybercrime + glorification/notoriety/prestige | All 5 |
| S2 | Youth + cybercrime pathways/motivation | All 5 |
| S3 | Hacker + culture/subculture/identity | All 5 |

See [`docs/SEARCH_STRATEGY.md`](docs/SEARCH_STRATEGY.md) for full query strings.

---

## Citation

If you use this dataset or analysis in your work, please cite:

```bibtex
@article{cybercrime_glorification_slr_2026,
  title={What's There to Flex? A Systematic Literature Review on the Cultural 
         Glorification of Cybercrime and Youth Radicalisation},
  author={Faizan Ali, Kashif Ali},
  year={2026},
  note={Available at: https://github.com/rfagreat/cybercrime-glorification-slr}
}
```

---

## Contributing

This is an academic research repository. If you have suggestions or identify relevant studies that should be included, please open an issue.

---

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the material with appropriate attribution.
