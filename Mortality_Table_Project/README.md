# Actuarial Mortality Analysis & Life Table Modeling

## Overview

This project develops a complete actuarial life table using U.S. Social Security Administration (SSA) mortality data. The analysis replicates core actuarial techniques used in life insurance and pension modeling, including survival estimation, mortality analysis, and life expectancy calculations.

In addition to constructing standard life table functions (qx, lx, ex), the project extends to gender-based mortality comparisons and applies a Gompertz mortality model to capture the exponential relationship between age and mortality risk.

---

## Objectives

* Construct and validate a full actuarial life table from raw mortality data
* Analyze survival patterns and age-dependent mortality behavior
* Compare mortality and life expectancy across genders
* Quantify and interpret life expectancy differentials
* Fit a Gompertz mortality model using log-linear regression

---

## Methodology

### Life Table Construction

Using SSA data, the following standard actuarial relationships were implemented:

* Survival probability: px = 1 − qx
* Survivorship: lx+1 = lx · px
* Deaths: dx = lx − lx+1
* Life expectancy: ex = Tx / lx

A radix of 100,000 was used to model cohort survival.

---

### Mortality Analysis

* Generated survival curves (lx), mortality curves (qx), and life expectancy curves (ex)
* Evaluated non-linear mortality trends across age cohorts
* Identified exponential growth in mortality consistent with actuarial theory

---

### Gender-Based Comparison

* Compared male and female mortality rates across all ages
* Constructed life expectancy gap: ex(female) − ex(male)
* Analyzed persistent longevity advantage and divergence patterns

---

### Gompertz Mortality Model

A Gompertz model was fitted to adult mortality data:

* μ(x) = A · e^(Bx)
* ln(qx) ≈ ln(A) + Bx

Log-linear regression was used to estimate model parameters and evaluate goodness of fit.

---

## Key Results

* Mortality increases exponentially with age, particularly after mid-life
* Female mortality rates are consistently lower than male rates across all ages
* Life expectancy declines non-linearly with age due to conditional survival effects
* A persistent female life expectancy advantage is observed across all cohorts
* The Gompertz model provides a strong fit to observed adult mortality patterns

---

## Repository Structure

* data - Data sourced from the U.S. Social Security Administration (SSA) Period Life Tables: https://www.ssa.gov/oact/STATS/table4c6.html
* `report/` — cleaned SSA life table
* `outputs/` — visualizations (survival, mortality, life expectancy, gap)

---

## Tools & Skills

* Excel (data structuring, actuarial calculations, visualization)
* Python (optional: regression modeling, data analysis)
* Statistical modeling (log-linear regression)
* Actuarial concepts: life tables, survival analysis, mortality modeling

---

## Visualizations

![Survival Curve](outputs/survival_curve.png)

![Mortality Curve](outputs/mortality_curve.png)

![Life Expectancy Curve](outputs/life_expectancy_curve.png)
