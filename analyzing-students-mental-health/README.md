# Analyzing Students' Mental Health

**Healthcare Research Analytics | Exploratory Data Analysis**

**Technologies:** PostgreSQL, SQL, Python, pandas, Matplotlib  
**Environment:** DataCamp DataLab  
**Completed:** October 2026

## Project Overview

This project explores the relationship between length of stay in Japan and three mental health indicators among international university students: depression, social connectedness, and acculturative stress.

The analysis combines SQL-based data exploration, validation, and aggregation with Python visualizations to identify descriptive patterns and assess their reliability.

## Research Question

How is the length of stay in Japan associated with depression, social connectedness, and acculturative stress among international university students?

## Dataset

The dataset contains 286 student records from a 2018 survey conducted at an international university in Japan.

The analysis focuses on **201 international students**, examining four principal variables:

| Variable | Description |
|---|---|
| `stay` | Length of stay in Japan, in years |
| `todep` | Depression score (PHQ-9) |
| `tosc` | Social connectedness score (SCS) |
| `toas` | Acculturative stress score (ASISS) |

Data completeness checks identified no missing values in the selected analytical variables for the 201 international students.

## Methodology

The project follows an exploratory, descriptive analytical approach:

1. **Dataset exploration:** Examined dataset structure, variables, and student classifications using PostgreSQL.
2. **Data validation:** Checked completeness of the variables used in the analysis.
3. **SQL aggregation:** Calculated average mental health scores and sample sizes by length of stay.
4. **Python visualization:** Developed charts using pandas and Matplotlib.
5. **Interpretation:** Evaluated observed patterns alongside sample sizes and methodological limitations.

The principal trend visualizations focus on students with stays of **1–4 years** (194 of 201 international students), since longer-stay groups contained very few observations.

## Key Findings

### Depression (PHQ-9)

Average depression scores increased from **7.48** among first-year students to **9.09** among third-year students, before declining to **8.57** in the fourth-year group.

The pattern is not consistently increasing across all four years.

### Social Connectedness (SCS)

Average social connectedness decreased from **38.11** in the first-year group to **33.93** in the fourth-year group, an approximate **10.97% reduction**.

The pattern suggests lower average connectedness among the longer-stay groups examined, although the trend is not strictly monotonic.

### Acculturative Stress (ASISS)

Average acculturative stress increased from **72.80** in the first-year group to **87.71** in the fourth-year group, an approximate **20.48% increase**.

This was the clearest directional pattern observed among the three indicators.

## Limitations

- The analysis is descriptive and cross-sectional; it cannot establish causality or changes within individual students over time.
- The dataset originates from a single university, limiting generalizability.
- Sample sizes vary considerably across length-of-stay groups, particularly after four years.
- Potential confounding factors were not controlled.
- No inferential statistical tests were performed.

Future research could incorporate larger and more representative samples, longitudinal data, multivariable methods, and statistical hypothesis testing.

## View the Full Analysis

**[Open the complete Jupyter notebook](notebook.ipynb)**

The notebook contains the research objectives, SQL queries, validation results, Python visualizations, interpretations, and conclusions.

**Execution note:** The analysis was developed and executed in DataCamp DataLab. Some SQL cells rely on the DataLab environment and may require adaptation to run in a standard Jupyter setup.

