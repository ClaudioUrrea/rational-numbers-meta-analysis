# Technology-Enhanced Rational Number Learning in K-12: A Meta-Analysis

[![DOI](https://img.shields.io/badge/DOI-10.6084%2Fm9.figshare.31015807-blue)](https://doi.org/10.6084/m9.figshare.31015807)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![ORCID](https://img.shields.io/badge/ORCID-0000--0001--7197--8928-green.svg)](https://orcid.org/0000-0001-7197-8928)

## Overview

This repository contains the complete dataset, analysis code, and supplementary materials for the meta-analysis:

> **Technology-Enhanced Rational Number Learning in K-12 Education: A Meta-Analysis of Intelligent Tutoring Systems, Augmented Reality, and Pedagogical Frameworks**

**Key Findings:**
- Overall effect size: Hedge's g = 0.564 (95% CI [0.468, 0.661])
- 12 high-quality studies across 7 countries (N = 1,721 students)
- Negligible heterogeneity (I² = 0%), suggesting consistent positive effects
- Technology type (ITS, AR/VR, frameworks) did not moderate effectiveness
- Pedagogical design quality matters more than technological sophistication

## Repository Structure

```
.
├── README.md                          # This file
├── LICENSE                            # CC BY 4.0 license
├── CITATION.cff                       # Citation information
├── data/
│   ├── Base_Datos_K12_FINAL.xlsx     # Primary dataset (12 studies)
│   ├── meta_analysis_results_k12.csv  # Analysis results with weights
│   └── Data_Dictionary.md             # Variable descriptions
├── analysis/
│   ├── metaanalysis_k12_UPDATED.R    # Complete R analysis script
│   └── Session_Info.txt               # R session information
├── figures/
│   ├── forest_plot_k12.png           # Forest plot (publication quality)
│   └── funnel_plot_k12.png           # Funnel plot for bias assessment
├── documentation/
│   ├── Coding_Forms.md                # Variable extraction protocol
│   ├── Quality_Assessment.md          # EPHPP quality ratings
│   ├── Search_Strategies.md           # Database search strategies
│   └── Included_Studies.md            # Details of 12 included studies
└── manuscript/
    ├── ETS_Paper_10_01_2026.pdf      # Published paper
    └── ETS_Paper_10_01_2026.docx     # Word version
```

## Quick Start

### Prerequisites

- R version ≥ 4.3.2
- Required R packages:
  ```r
  install.packages(c("metafor", "readxl", "dplyr", "ggplot2"))
  ```

### Running the Analysis

1. Clone this repository:
   ```bash
   git clone https://github.com/ClaudioUrrea/rational-numbers-meta-analysis.git
   cd rational-numbers-meta-analysis
   ```

2. Open R/RStudio and run:
   ```r
   source("Analysis/metaanalysis_k12_UPDATED.R")
   ```

3. The script will:
   - Load data from `Data/Base_Datos_K12_FINAL.xlsx`
   - Perform random-effects meta-analysis
   - Generate forest and funnel plots
   - Conduct subgroup and sensitivity analyses
   - Export results to CSV

## Data Description

### Primary Dataset

The `Base_Datos_K12_FINAL.xlsx` file contains:

- **12 studies** (2017-2025)
- **7 countries**: Germany, Finland, Spain, China, UK, Taiwan, USA
- **1,721 total participants** (range: 65-300 per study)
- **Effect sizes**: Hedge's g ranging from 0.39 to 0.71

### Key Variables

| Variable | Description |
|----------|-------------|
| `Study_ID` | Unique study identifier |
| `Authors` | Study authors |
| `Year` | Publication year |
| `Country` | Study location |
| `Sample_Size` | Total N |
| `g` | Hedge's g effect size |
| `SE` | Standard error |
| `Variance` | Variance of effect size |
| `Tech_Category` | ITS, AR/VR, or Pedagogical Framework |
| `Grade_Category` | Elementary (3-5) or Middle (6-7) |
| `Design` | RCT, Quasi-experimental, or Longitudinal |

See `Data/Data_Dictionary.md` for complete variable descriptions.

## Methodology

### Inclusion Criteria

- **Population**: K-12 students (ages 5-18)
- **Intervention**: Technology-enhanced rational number instruction
- **Comparison**: Traditional instruction or alternative approaches
- **Outcomes**: Validated measures of conceptual understanding or procedural fluency
- **Design**: RCT, quasi-experimental, or rigorous pre-post designs
- **Quality**: Q1/Q2 journals (2015-2025)

### Analysis Approach

- **Model**: Random-effects meta-analysis (REML estimation)
- **Effect size**: Hedge's g (bias-corrected standardized mean difference)
- **Software**: R 4.3.2 with metafor package v4.4.0
- **Heterogeneity**: I², Q statistic, τ²
- **Moderators**: Technology type, pedagogical challenge, duration, grade level
- **Sensitivity**: Leave-one-out analysis, quality stratification

## Results Summary

### Overall Effect

```
Pooled Hedge's g = 0.564
95% CI: [0.468, 0.661]
Z = 11.47, p < 0.001
I² = 0% (negligible heterogeneity)
95% Prediction Interval: [0.468, 0.661]
```

### Interpretation

- **Medium-to-large positive effect** (exceeds Hattie's threshold of 0.40)
- Equivalent to moving from 50th to 71st percentile
- Highly consistent across diverse contexts
- All 12 studies showed positive effects

### Effects by Pedagogical Challenge

| Challenge | k | Mean g | Range |
|-----------|---|--------|-------|
| Magnitude/number line | 3 | 0.64 | 0.61-0.68 |
| Conceptual understanding | 5 | 0.55 | 0.42-0.71 |
| Operational fluency | 2 | 0.50 | 0.39-0.61 |
| Multiple foci | 2 | 0.56 | 0.48-0.63 |

## Reproducibility

This repository provides complete reproducibility:

**Raw data** with extraction protocols  
**Analysis code** with inline documentation  
**Publication-ready figures** (PNG, 800×800, 130 DPI)  
**Quality assessments** with detailed criteria  
**Search strategies** for 6 databases  
**R session information** for package versions  

## Citation

If you use this dataset or code, please cite:

```bibtex
@article{urrea2026technology,
  title={Technology-Enhanced Rational Number Learning in K-12 Education: A Meta-Analysis of Intelligent Tutoring Systems, Augmented Reality, and Pedagogical Frameworks},
  author={Urrea, Claudio},
  journal={Educational Technology \& Society},
  year={2026},
  note={Manuscript submitted for publication},
  doi={10.6084/m9.figshare.31015807}
}
```

**Data Repository:**  
Urrea, C. (2026). *Technology-Enhanced Rational Number Learning Meta-Analysis Dataset* [Data set]. Figshare. https://doi.org/10.6084/m9.figshare.31015807

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

You are free to:
- **Share** — copy and redistribute the material
- **Adapt** — remix, transform, and build upon the material

Under the following terms:
- **Attribution** — You must give appropriate credit and indicate if changes were made

## Contact

**Author**: Claudio Urrea  
**ORCID**: [0000-0001-7197-8928](https://orcid.org/0000-0001-7197-8928)  
**GitHub**: https://github.com/ClaudioUrrea  
**Figshare**: https://doi.org/10.6084/m9.figshare.31015807

## Acknowledgments

This research received no external funding. The author declares no conflicts of interest.

## Version History

- **v1.0** (January 2026): Initial release
  - 12 studies meta-analysis
  - Complete replication materials
  - Publication-ready figures

## Contributing

While this is a completed meta-analysis, suggestions for improvements to documentation or code are welcome. Please open an issue or submit a pull request.

---

**Last Updated**: January 10, 2026
