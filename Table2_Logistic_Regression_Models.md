# Table 2: Multivariable Logistic Regression Models for 12-Month Survival Prediction

## A. Bilateral Model (n=46, Pseudo R²=0.186)

| Variable | Coefficient (β) | SE | OR | 95% CI | p-value |
|----------|-----------------|------|------|---------|---------|
| Intercept | 0.1600 | 2.412 | — | — | 0.95 |
| Age (per year) | -0.0104 | 0.026 | 0.990 | 0.94–1.04 | 0.73 |
| MGMT Methylated | 0.7775 | 0.749 | 2.176 | 0.50–9.42 | 0.30 |
| EoR ≥95% | 0.7010 | 0.835 | 2.016 | 0.39–10.3 | 0.40 |
| **CES (0-2)** | **-0.9425** | **0.571** | **0.390** | **0.13–1.22** | **0.10*** |
| **IntraM1 Tumor (LL/UL)** | **0.9631** | **0.795** | **2.620** | **0.55–12.4** | **0.22** |

*Trend toward significance (p<0.10)

**Model Interpretation:**
- Each unit increase in CES (0→1→2) reduces odds of 12-month survival by 61% (OR=0.39)
- Each unit increase in IntraM1 Tumor ratio increases odds of survival by 162% (OR=2.62)
- Hosmer-Lemeshow goodness-of-fit: χ²=5.23, p=0.73

---

## B. Unilateral Model (n=50, Pseudo R²=0.125)

| Variable | Coefficient (β) | SE | OR | 95% CI | p-value |
|----------|-----------------|------|------|---------|---------|
| Intercept | -0.7900 | 2.156 | — | — | 0.71 |
| Age (per year) | -0.0274 | 0.024 | 0.973 | 0.93–1.02 | 0.28 |
| MGMT Methylated | 0.1188 | 0.732 | 1.126 | 0.27–4.76 | 0.87 |
| EoR ≥95% | 0.6391 | 0.807 | 1.895 | 0.39–9.22 | 0.43 |
| **IntraM1 Tumor Ratio (LL/UL)** | **1.9225** | **0.992** | **6.838** | **0.98–47.85** | **0.053*** |

*Trend toward significance (p<0.10)

**Model Interpretation:**
- Each unit increase in IntraM1 Tumor ratio increases odds of 12-month survival by 584% (OR=6.84)
- Higher ratio suggests preserved motor cortex organization in tumor hemisphere

---

## C. CES Distribution and 12-Month Survival (Bilateral Cohort, n=46)

| CES Score | n (%) | 12-mo Survival | 95% CI | Interpretation |
|-----------|-------|----------------|--------|----------------|
| 0 | 5 (10.9%) | 80.0% | 28.4–99.5% | Normal bilateral excitability |
| 1 | 18 (39.1%) | 94.4% | 72.7–99.9% | One functional area abnormal |
| 2 | 23 (50.0%) | 56.5% | 34.5–76.8% | Both functional areas abnormal |

**Note:** CES=2 demonstrates markedly worse 12-month survival compared to CES=0-1 (χ²=8.94, p=0.011)

---

## D. Extent of Resection Cutoff Analysis (Univariate, n=77)

| Cutoff | 12-mo Survival (Yes) | 12-mo Survival (No) | OR | 95% CI | p-value |
|--------|---------------------|---------------------|------|---------|---------|
| EoR ≥90% | 75.8% (n=66) | 63.6% (n=11) | 1.79 | 0.46–6.90 | 0.40 |
| **EoR ≥95%** | **78.3% (n=60)** | **58.8% (n=17)** | **2.53** | **0.81–7.95** | **0.11** |
| EoR 100% | 80.6% (n=36) | 68.3% (n=41) | 1.92 | 0.67–5.53 | 0.22 |

**Note:** EoR ≥95% provides optimal prognostic discrimination and is used in the calculator models.

---

## E. Model Comparison

| Model | n | Pseudo R² | AIC | C-statistic | Variables |
|-------|---|-----------|-----|-------------|-----------|
| Clinical Only | 75 | 0.072 | 89.3 | 0.72 | Age, MGMT, EoR |
| **Bilateral (nTMS)** | **46** | **0.186** | **58.2** | **0.76** | Age, MGMT, EoR, CES, IntraM1 Tumor |
| **Unilateral (nTMS)** | **50** | **0.125** | **62.4** | **0.71** | Age, MGMT, EoR, IntraM1 Tumor |

---

## Abbreviations

- **CES**: Cortical Excitability Score (0-2); sum of abnormal iRMTr for UL and LL
- **IntraM1 Tumor**: Intra-hemispheric M1 ratio in tumor hemisphere (LL RMT / UL RMT)
- **EoR**: Extent of Resection
- **iRMTr**: Interhemispheric Resting Motor Threshold ratio
- **SE**: Standard Error (calculated from 95% CI: SE = [ln(OR_upper) - ln(OR_lower)] / 3.92)
- **OR**: Odds Ratio
- **CI**: Confidence Interval

---

*Table generated: December 2024*
*Data source: King's College Hospital GBM cohort (n=77)*
