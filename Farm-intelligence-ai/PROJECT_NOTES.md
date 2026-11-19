# 🌱 FARM INTELLIGENCE AI

### Project Development Newsletter | Issue 001

**Reporting Period:** November 11–19, 2026\
**Development Environment:** Windows | Python | Jupyter Notebook | VS Code | GitHub

---

## Executive Summary

Farm Intelligence AI is an evolving data science initiative designed to transform agricultural data into actionable insights for farmers, agricultural investors, and farm managers.

Our long-term vision is to build an integrated intelligence platform capable of analyzing livestock health, crop production, farm finances, and environmental conditions.

Rather than developing the entire platform immediately, we adopted a phased, project-based learning strategy. Each stage builds practical data science capabilities while producing reusable components for the future platform.

**Our first agricultural analytics project is now developed, documented, and published to GitHub.**

Using historical corn grain production data from the United States Department of Agriculture (USDA), we have established a foundation for analyzing agricultural production trends, variability, and potential anomalies.

## 1. Our Vision: A Connected Agricultural Intelligence Platform

Farm Intelligence AI is being designed around four major operational areas.

**Livestock Intelligence:** Monitor animal records, health indicators, herd performance, and potential health risks.

**Crop Intelligence:** Analyze crop production, historical yields, seasonal patterns, and agricultural performance.

**Financial Intelligence:** Evaluate operating expenses, agricultural revenue, profitability, and investment performance.

**Environmental Intelligence:** Incorporate weather, rainfall, soil conditions, water availability, and environmental risk factors.

These capabilities will eventually connect through a shared data platform supporting dashboards, analytics, forecasting, and decision-support tools.

Our development philosophy is simple:

*Start with reliable data, develop strong analytical skills, and progressively build intelligent capabilities.*

## 2. Our First Project: Washington State Corn Production Analysis

Our first practical project focuses on Washington State corn grain production between 2015 and 2025.

**Data source:** USDA National Agricultural Statistics Service (NASS), Quick Stats.

The original dataset contained 54 records and 21 columns, including annual production observations and other reporting-period records.

We identified 11 annual production observations suitable for historical analysis.

### Data Preparation Accomplishments

We successfully:

1. Imported the USDA CSV dataset using Pandas.
2. Examined the dataset's structure, column names, and missing values.
3. Identified why dropping every row with a missing value would eliminate useful records.
4. Selected relevant columns, including year, reporting period, state, data item, and production value.
5. Filtered the dataset to retain annual production observations.
6. Removed comma separators from production values and converted them to numeric data.
7. Sorted observations chronologically.
8. Calculated year-over-year production changes.

This stage established an important principle for Farm Intelligence AI: **data quality must be assessed before conclusions are drawn.**

## 3. Agricultural Production Findings

Our analysis produced the following historical production figures.

| Year | Corn production (bushels) |
| ---- | ------------------------- |
| 2015 | 16,125,000                |
| 2016 | 19,975,000                |
| 2017 | 18,000,000                |
| 2018 | 18,480,000                |
| 2019 | 19,908,000                |
| 2020 | 19,380,000                |
| 2021 | 21,080,000                |
| 2022 | 17,600,000                |
| 2023 | 18,000,000                |
| 2024 | 24,205,000                |
| 2025 | 31,375,000                |

### Key Production Indicators

- **Total production across 11 years:** 224,128,000 bushels.
- **Average annual production:** Approximately 20.38 million bushels.
- **Highest annual production:** 2025, at 31.375 million bushels.
- **Lowest annual production:** 2015, at 16.125 million bushels.
- **Largest year-over-year increase:** 2024, approximately 34.47%.
- **Largest year-over-year decline:** 2022, approximately 16.51%.

Our findings show that corn production did not increase consistently every year. Instead, production fluctuated, with particularly strong growth recorded in 2024 and 2025.

These results demonstrate the value of examining historical patterns rather than relying on a single year's production figure.

## 4. Statistical Analysis: Understanding Agricultural Variability

During Day 9, we expanded beyond basic trend analysis to examine production variability and the distribution of annual observations.

### Statistical Results

| Metric                         | Result                      |
| ------------------------------ | --------------------------- |
| Mean annual production         | 20,375,273 bushels          |
| Median annual production       | 19,380,000 bushels          |
| Sample standard deviation      | 4,221,012 bushels           |
| Sample variance                | 17,816,943,818,182 bushels² |
| Coefficient of variation       | 20.72%                      |
| Potential statistical outliers | 1                           |

### What These Results Tell Us

The mean exceeds the median, indicating that higher production observations influence the average.

The coefficient of variation of 20.72% indicates that the sample standard deviation is approximately one-fifth of average annual production.

Using the interquartile range method, we identified the 2025 production figure of 31.375 million bushels as a potential statistical outlier.

Importantly, an outlier is not necessarily an error. It may represent a genuine change in agricultural production.

We therefore retained the observation and documented the need for additional investigation.

Our current analysis does not establish whether production changes were caused by rainfall, weather conditions, harvested acreage, agricultural practices, or other factors.

Those questions will require additional datasets.

## 5. Data Visualization: Turning Numbers into Insights

We developed multiple visualizations using Python and Matplotlib.

**Production Trend Line Chart**

Illustrates annual corn grain production from 2015 through 2025, making historical changes easier to interpret.

**Year-over-Year Growth Chart**

Shows annual percentage increases and decreases, highlighting periods of stronger growth and production decline.

**Box Plot**

Summarizes the production distribution, including the median, quartiles, and potential outlier.

**Histogram**

Displays how annual production observations are distributed, with many values concentrated between approximately 16 million and 21 million bushels.

Together, these visualizations establish the foundation for a future agricultural performance dashboard.

## 6. Technical Skills and Tools Developed

Our project has provided practical experience across several core data science disciplines.

| Technology       | Application                                          |
| ---------------- | ---------------------------------------------------- |
| Python           | Programming fundamentals and analytical calculations |
| Pandas           | Data import, filtering, cleaning, and transformation |
| NumPy            | Numerical computing foundations                      |
| Jupyter Notebook | Interactive analysis and documentation               |
| Matplotlib       | Production trends and statistical visualizations     |
| VS Code          | Local development environment                        |
| Git              | Version control and change tracking                  |
| GitHub           | Project documentation and portfolio publishing       |

We also practiced Python variables, data types, conditional logic, loops, user input, and basic programming exercises.

Our IBM Data Science Professional Certificate studies provide a complementary foundation for these practical activities.

## 7. Project Management and Version Control Milestone

An important achievement was establishing a repeatable development and publishing workflow.

Our project repository contains the agricultural analysis notebook, project notes, and USDA data file.

We also encountered a real Git collaboration challenge when the local and GitHub branches contained different commits.

Rather than overwriting either version, we:

1. Investigated the branch divergence.
2. Protected uncommitted notebook changes using Git stash.
3. Created a backup branch.
4. Rebased the local work against the updated GitHub branch.
5. Resolved a documentation conflict.
6. Successfully pushed the updated project to GitHub.
7. Restored the previously stashed notebook changes.

**Publishing milestone:** November 19, 2026\
**Published GitHub commit:** `baedf43`

This experience strengthened our understanding of version control, change management, and protecting project deliverables.

### Project Repository

[https://github.com/nushlicon/data-science-portfolio/tree/main/Farm-intelligence-ai](https://github.com/nushlicon/data-science-portfolio/tree/main/Farm-intelligence-ai)

## 8. Development Progress

| Project milestone                             | Status                           |
| --------------------------------------------- | -------------------------------- |
| Establish Python development environment      | Completed                        |
| Learn Python fundamentals                     | Completed foundational exercises |
| Create Farm Intelligence AI project structure | Completed                        |
| Obtain agricultural production data           | Completed                        |
| Clean and prepare USDA dataset                | Completed                        |
| Analyze historical production trends          | Completed                        |
| Calculate year-over-year changes              | Completed                        |
| Perform descriptive statistical analysis      | Completed                        |
| Identify potential production outliers        | Completed                        |
| Create statistical visualizations             | Completed                        |
| Publish Day 9 analysis to GitHub              | Completed                        |
| Compare production across historical periods  | Next                             |
| Develop interactive agricultural dashboard    | Planned                          |
| Integrate additional agricultural datasets    | Planned                          |
| Build predictive analytics models             | Future phase                     |

## 9. What's Next: Day 10 and Beyond

Our next development milestone focuses on **grouping, aggregation, and comparative agricultural analysis**.

We will use Pandas `groupby()` and `.agg()` to compare average annual corn production across historical periods.

The initial comparison will examine 2015–2020 versus 2021–2025.

This will help us understand how production performance differs between earlier and more recent observations.

As the platform develops, we intend to expand into:

**Phase 1 — Agricultural Data Analytics:** Historical production analysis, data quality, visualization, and descriptive statistics.

**Phase 2 — Agricultural Performance Dashboards:** Interactive charts, performance indicators, and comparative reporting.

**Phase 3 — Integrated Farm Data:** Additional crop datasets, livestock records, farm finances, and environmental observations.

**Phase 4 — Predictive Analytics:** Forecasting, anomaly detection, and risk identification using statistical and machine learning methods.

**Phase 5 — Farm Intelligence AI Platform:** An integrated decision-support environment combining agricultural data, analytical models, and intelligent recommendations.

These phases describe our development roadmap, not features that have already been implemented.

## Closing Message

Farm Intelligence AI began with a question:

*How can data science help farmers make better operational and investment decisions?*

Our first development cycle has transformed that question into a working agricultural analytics project.

We have moved from Python fundamentals to analyzing authentic USDA production data, calculating meaningful statistics, visualizing agricultural trends, and publishing a documented project on GitHub.

The next challenge is to move from describing what happened historically toward understanding performance drivers and, eventually, predicting what may happen next.

**Our mission remains unchanged: Build Farm Intelligence AI one dataset, one analytical model, and one practical project at a time.**

---

**FARM INTELLIGENCE AI**\
*Data-Driven Agriculture. Intelligent Decisions. Sustainable Growth.*

**End of Issue 001 | November 19, 2026**

Add a clear stakeholder call to actionCreate a concise reader-friendly opening
