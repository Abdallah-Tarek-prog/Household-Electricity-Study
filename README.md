#  Household Electricity Consumption Study
### Statistical Analysis using Probability Theory & Statistical Inference

> **1st Place — 14th Undergraduate Engineering Mathematics Research Forum (UMRF)**
> Team: **Supercaliprobabilisticexpialidocious**

---

## 📋 Table of Contents
- [Overview](#overview)
- [Award & Recognition](#award--recognition)
- [Dataset](#dataset)
- [Research Questions & Objectives](#research-questions--objectives)
- [Methodology](#methodology)
- [Key Findings](#key-findings)
- [Repository Contents](#repository-contents)
- [Team](#team)
- [Acknowledgements](#acknowledgements)
- [CV Description](#cv-description)

---

## Overview

This research project investigates individual household electricity consumption patterns using **probability theory** and **statistical inference** methods. By analyzing over **2 million one-minute-interval observations** from a single household in Sceaux, France (December 2006 – November 2010), the study employs more than **10 statistical tests** across parametric, non-parametric, and distribution-fitting frameworks to:

- Characterize consumption distributions
- Identify temporal patterns (hourly, daily, and seasonal)
- Build predictive linear models
- Generate statistically faithful synthetic data
- Assess extreme consumption event probabilities

The findings provide an empirical foundation for **smart grid optimization**, **demand-response program design**, and **infrastructure planning**, with practical implications for capacity expansion and renewable energy integration in temperate-climate regions.

---

## Award & Recognition

 **1st Place — 14th Undergraduate Engineering Mathematics Research Forum (UMRF)**

I am honored to share that our team, **Supercaliprobabilisticexpialidocious**, was awarded **1st Place** at the **14th Undergraduate Engineering Mathematics Research Forum (UMRF)**. This milestone reflects long hours, close collaboration, and deep technical commitment from every member of our team.

Special thanks to the **TCCD - Career Center** under the direction of **Prof. Maha Hassanein** and **Dr. Samah El-Tantawy** for organizing such an inspiring forum, and to our supervisor for their invaluable guidance throughout this journey.

---

## Dataset

| Property | Details |
|---|---|
| **Source** | UCI Machine Learning Repository |
| **Contributors** | Georges Hebrail & Alice Berard (2012) |
| **Location** | Sceaux, France (7 km from Paris) |
| **Period** | December 2006 – November 2010 (47 months) |
| **Observations** | 2,075,259 one-minute-interval measurements |
| **Missing Values** | ~0.97% of rows |
| **License** | Creative Commons Attribution 4.0 International (CC BY 4.0) |
| **URL** | [UCI Dataset](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption) |

### Variables

| Variable | Type | Units | Description |
|---|---|---|---|
| Date | Date | — | Calendar date of measurement |
| Time | Time | — | Time of day |
| Global Active Power | Continuous | kW | Total active power consumed |
| Global Reactive Power | Continuous | kW | Reactive power component |
| Voltage | Continuous | V | Average voltage per minute |
| Global Intensity | Continuous | A | Average current intensity |
| Sub_metering_1 | Continuous | Wh | Kitchen (dishwasher, oven, microwave) |
| Sub_metering_2 | Continuous | Wh | Laundry (washer, dryer, fridge, light) |
| Sub_metering_3 | Continuous | Wh | Climate control (water heater, A/C) |

---

## Research Questions & Objectives

| # | Research Question | Statistical Approach |
|---|---|---|
| RQ1 | Which probability distribution best characterizes household electricity consumption? | Goodness-of-Fit Tests (KS, Anderson-Darling, Chi-Square) |
| RQ2 | Is there a significant difference between weekday and weekend consumption? | Two-Sample t-Test (Welch's), Mann-Whitney U |
| RQ3 | Do seasonal variations significantly affect consumption? | One-Way ANOVA, Kruskal-Wallis, Post-Hoc Tukey HSD |
| RQ4 | Can consumption be accurately predicted from electrical variables? | Simple & Multiple Linear Regression |
| RQ5 | Are categorical variables (hour, day type, season) independent of consumption level? | Chi-Square Test of Independence |

---

## Methodology

The study employs **10+ statistical tests** spanning three analytical frameworks:

### Parametric Tests
- **Welch's Two-Sample t-Test** — Weekday vs. weekend mean comparison
- **One-Way ANOVA** — Seasonal and hourly mean comparisons
- **Two-Way ANOVA** — Interaction effects between season and day type
- **Post-Hoc Tukey HSD** — Pairwise seasonal comparisons after ANOVA
- **Simple Linear Regression** — Global Intensity → Global Active Power
- **Levene's Test** — Equality of variances

### Non-Parametric Tests
- **Kolmogorov-Smirnov (KS) Test** — Distribution fitting
- **Anderson-Darling Test** — Distribution fitting (tail-sensitive)
- **Chi-Square Goodness-of-Fit** — Observed vs. expected frequencies
- **Kruskal-Wallis Test** — Non-parametric ANOVA alternative
- **Mann-Whitney U Test** — Non-parametric two-group comparison

### Simulation Methods
- **Monte Carlo Simulation** — 100,000 synthetic samples from fitted Weibull distribution; extreme event probability estimation; return period analysis

---

## Key Findings

1. **Distribution Fit:** Global active power consumption follows a **Weibull distribution** with exceptional goodness-of-fit quality — superior to Normal and Lognormal candidates.

2. **Weekend Effect:** A statistically significant weekend effect was identified — **weekends show higher average electricity consumption** than weekdays.

3. **Seasonal Variation:** Strong seasonal patterns exist — **winter consumption is significantly higher than summer**, consistent with heating load expectations.

4. **Linear Relationship:** A **strong linear relationship** was found between global intensity and active power, enabling reliable consumption prediction.

5. **Categorical Associations:** Significant dependencies were found between consumption levels and categorical variables — **Season × Consumption** and **Hour × Consumption** associations are statistically confirmed.

6. **Synthetic Data Generation:** Monte Carlo simulation successfully generated synthetic hourly consumption data that preserves the observed statistical properties of the real dataset.

---

## Repository Contents

| File | Description |
|---|---|
| `Report.pdf` | Full research report with methodology, statistical tests, and detailed results |
| `Poster.pdf` | Conference poster presented at the 14th UMRF |
| `Presenation.pptx` | Slide deck used for the forum presentation |

---

## Team

**Team Name:** Supercaliprobabilisticexpialidocious
**Forum:** 14th Undergraduate Engineering Mathematics Research Forum (UMRF) — **🥇 1st Place**

| Member |
|---|
| **Abdallah Tarek** |
| Moslem Ahmed |
| Ahmed Khattaby |
| Abdulrhman Jalal |
| Mostafa Mohammed |
| Ali Tharwat |

---

## Acknowledgements

-  **Prof. Maha Hassanein** — Supervisor and forum director; special thanks for continuous guidance and support throughout this research journey.
-  **Dr. Samah El-Tantawy** — Co-director of the TCCD - Career Center and forum organizer.
-  **TCCD - Career Center** — For organizing the 14th UMRF and creating a platform for undergraduate research excellence.



*"This milestone reflects long hours, close collaboration, and deep technical commitment. I'm excited to keep pushing forward and to turn this momentum into more impactful research."*
