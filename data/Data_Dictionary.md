# Data Dictionary

## Technology-Enhanced Rational Number Learning Meta-Analysis (K=12)

**Dataset**: `Base_Datos_K12_FINAL.xlsx`  
**Version**: 1.0  
**Date**: January 10, 2026  
**Studies**: 12  
**Total N**: 1,721 students  
**DOI**: 10.6084/m9.figshare.31015807

---

## Variables

### Study Identification

| Variable | Type | Description | Values/Range | Notes |
|----------|------|-------------|--------------|-------|
| `Study_ID` | Integer | Unique study identifier | 1-12 | Sequential numbering |
| `Authors` | String | First author last name et al. | Text | Format: "Lastname et al." |
| `Year` | Integer | Publication year | 2017-2025 | All studies peer-reviewed |
| `DOI` | String | Digital Object Identifier | Text | Verified DOI for each study |
| `Journal` | String | Publication venue | Text | All Q1/Q2 ranked journals |

### Sample Characteristics

| Variable | Type | Description | Values/Range | Notes |
|----------|------|-------------|--------------|-------|
| `Sample_Size` | Integer | Total participants | 65-300 | Combined intervention + control |
| `N_Intervention` | Integer | Intervention group N | Varies | Students receiving technology |
| `N_Control` | Integer | Control group N | Varies | Traditional/alternative instruction |
| `Country` | String | Study location | 7 countries | Germany, Finland, Spain, China, UK, Taiwan, USA |
| `Grade_Level` | String | Grade range | Text | e.g., "4-5", "6th" |
| `Grade_Category` | Categorical | Grade grouping | Elementary (3-5), Middle (6-7) | Simplified for analysis |
| `Age_Range` | String | Participant ages | Text | Approximately 8-13 years |

### Intervention Characteristics

| Variable | Type | Description | Values/Range | Notes |
|----------|------|-------------|--------------|-------|
| `Tech_Type` | String | Specific technology | Text | e.g., "ITS", "AR app", "Digital manipulatives" |
| `Tech_Category` | Categorical | Broad technology type | ITS, AR/VR, Pedagogical Framework | Primary classification |
| `Duration_Weeks` | Integer | Intervention length | 4-12 weeks | Total calendar duration |
| `Sessions` | Integer | Number of sessions | Varies | Total instructional sessions |
| `Minutes_Per_Session` | Integer | Session length | Varies | Minutes per session |
| `Total_Minutes` | Integer | Total instructional time | Calculated | Duration × Sessions × Minutes |
| `Pedagogical_Focus` | String | Primary learning objective | Text | Conceptual, procedural, magnitude, etc. |
| `Theoretical_Framework` | String | Guiding theory | Text | e.g., "Cognitive Load Theory" |

### Comparison Conditions

| Variable | Type | Description | Values/Range | Notes |
|----------|------|-------------|--------------|-------|
| `Control_Type` | Categorical | Comparison condition | Traditional, Alternative, Waitlist | Type of control/comparison |
| `Control_Description` | String | Details of comparison | Text | Brief description of control condition |

### Study Design

| Variable | Type | Description | Values/Range | Notes |
|----------|------|-------------|--------------|-------|
| `Design` | Categorical | Study design | RCT, Quasi-experimental, Longitudinal | Methodological approach |
| `Randomization` | Binary | Random assignment used | Yes, No | 1 = Yes, 0 = No |
| `Pretest` | Binary | Pretest administered | Yes, No | 1 = Yes, 0 = No |
| `Posttest` | Binary | Posttest administered | Yes, No | All = Yes |
| `Delayed_Posttest` | Binary | Follow-up assessment | Yes, No | 1 = Yes, 0 = No |
| `Blinding` | Binary | Assessor blinding | Yes, No, Unknown | Rarely feasible in education |

### Outcome Measures

| Variable | Type | Description | Values/Range | Notes |
|----------|------|-------------|--------------|-------|
| `Outcome_Instrument` | String | Assessment name | Text | e.g., "Fraction Test", "Custom assessment" |
| `Outcome_Type` | Categorical | Construct measured | Conceptual, Procedural, Composite | Type of understanding assessed |
| `Reliability` | Float | Cronbach's alpha | 0-1 | When reported; otherwise NA |
| `Validity_Evidence` | String | Validity information | Text | Brief description when reported |

### Effect Size Data

| Variable | Type | Description | Values/Range | Notes |
|----------|------|-------------|--------------|-------|
| `g` | Float | Hedge's g effect size | 0.39-0.71 | Bias-corrected standardized mean difference |
| `SE` | Float | Standard error of g | Positive | Sampling error |
| `Variance` | Float | Variance of g | Positive | SE² |
| `CI_lower` | Float | Lower 95% CI bound | Calculated | g - 1.96 × SE |
| `CI_upper` | Float | Upper 95% CI bound | Calculated | g + 1.96 × SE |
| `Weight` | Float | Study weight in meta-analysis | 0-100% | Inverse variance weight |

### Quality Assessment

| Variable | Type | Description | Values/Range | Notes |
|----------|------|-------------|--------------|-------|
| `Selection_Bias` | Categorical | Sample representativeness | Strong, Moderate, Weak | EPHPP criterion 1 |
| `Study_Design` | Categorical | Design appropriateness | Strong, Moderate, Weak | EPHPP criterion 2 |
| `Confounders` | Categorical | Confound control | Strong, Moderate, Weak | EPHPP criterion 3 |
| `Blinding` | Categorical | Assessor blinding | Strong, Moderate, Weak | EPHPP criterion 4 |
| `Data_Collection` | Categorical | Measure quality | Strong, Moderate, Weak | EPHPP criterion 5 |
| `Withdrawals` | Categorical | Attrition handling | Strong, Moderate, Weak | EPHPP criterion 6 |
| `Overall_Quality` | Categorical | Global quality rating | Strong, Moderate, Weak | No weak ratings = Strong |

### Moderator Variables (Coded for Analysis)

| Variable | Type | Description | Values/Range | Notes |
|----------|------|-------------|--------------|-------|
| `Pedagogical_Challenge` | Categorical | Primary challenge addressed | Magnitude, Conceptual, Operational, Multiple | For subgroup analysis |
| `Duration_Category` | Categorical | Length grouping | Short (<4 wks), Medium (4-8), Long (>8) | For moderator analysis |
| `Sample_Size_Category` | Categorical | N grouping | Small (<100), Medium (100-200), Large (>200) | For sensitivity analysis |

---

## Data Processing Notes

### Effect Size Calculation

Effect sizes (Hedge's g) were calculated from:
1. **Preferred**: Pretest-posttest means and SDs for both groups
2. **Alternative**: Post-test means and SDs when pretest not reported
3. **Conversion**: t-statistics, F-statistics, or reported Cohen's d

**Formula**: 
```
g = (M_int_post - M_cont_post) / SD_pooled × J

where J = 1 - 3/(4df - 1) [small-sample correction]
```

### Missing Data

- **Total missing**: Minimal (<5% across all variables)
- **Imputation**: None used; missing data noted as NA
- **Sensitivity**: Leave-one-out analysis confirmed robust results

### Data Transformations

1. **Grade categories**: Collapsed into Elementary/Middle for power
2. **Technology categories**: Grouped by primary mechanism (ITS/AR/VR/Framework)
3. **Duration**: Converted all to weeks for consistency

---

## Meta-Analysis Results Summary

**Pooled Effect**:
- Hedge's g = 0.564
- 95% CI: [0.468, 0.661]
- Z = 11.47, p < 0.001

**Heterogeneity**:
- I² = 0% (negligible)
- Q(11) = 4.29, p = 0.961
- τ² = 0.000

**95% Prediction Interval**: [0.468, 0.661]

---

## Variable Relationships

### Correlations (Kendall's τ)
- Sample Size × Effect Size: τ = -0.15 (ns)
- Duration × Effect Size: τ = 0.09 (ns)
- Year × Effect Size: τ = -0.02 (ns)

### Moderator Effects
- Technology Type: Q_M(2) = 1.09, p = 0.58 (not significant)
- Duration: β = 0.004, p = 0.21 (not significant)
- Grade Level: Descriptive only (k < 5 per group)

---

## Data Quality Checks

 **Range checks**: All effect sizes positive (0.39-0.71)  
 **Outlier detection**: No influential studies (leave-one-out)  
 **Publication bias**: Funnel plot symmetric; I²=0% suggests low bias  
 **Duplicate detection**: No overlapping samples identified  
 **DOI verification**: All 12 DOIs confirmed active  

---

## Usage Notes

### Recommended Practices

1. **Citation**: Always cite both the dataset (Figshare) and the paper
2. **Subset analysis**: Minimum k=3 studies per subgroup
3. **Power**: Current k=12 limits moderator analysis power
4. **Generalization**: Sample predominantly from high-resource contexts

### Known Limitations

- **Small k**: Limited statistical power for moderators
- **Geographic**: Concentrated in developed countries
- **Equity**: No studies examined differential effects by SES/disability
- **Follow-up**: Most studies assessed immediate posttests only
- **Quality threshold**: Q1/Q2 journals may introduce publication bias

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2026-01-10 | Initial release: 12 studies, complete variables |

---

## Contact

For questions about variable definitions or data quality:

**Claudio Urrea**  
ORCID: [0000-0001-7197-8928](https://orcid.org/0000-0001-7197-8928)  
GitHub: https://github.com/ClaudioUrrea/rational-numbers-meta-analysis  
Figshare: https://doi.org/10.6084/m9.figshare.31015807

---

## License

This data dictionary is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
