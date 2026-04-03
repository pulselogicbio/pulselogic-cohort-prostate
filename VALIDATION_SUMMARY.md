# Validation Summary -- Prostate Cancer (TCGA PRAD)

## Result

| Metric | Value |
|--------|-------|
| AUC | 0.9825 |
| 95% Bootstrap CI | [0.959-0.999] |
| Performance Tier | GOLD |
| Statistical Significance | CI excludes 0.50 (confirmed) |

---

## Performance Tier Definitions (MCQC Framework)

| Tier | AUC Threshold | Interpretation |
|------|--------------|----------------|
| GOLD | >= 0.80 | Strong discriminative performance; suitable for advancement |
| CONDITIONAL | 0.70-0.79 | Moderate performance; requires additional validation |
| EXPLORATORY | < 0.70 | Weak signal; may reflect biological heterogeneity or data limitations |

This cohort achieved **GOLD tier** (AUC 0.9825).

---

## Statistical Methodology

- **Validation design:** Bootstrap resampling (1,000 iterations, non-parametric percentile method)
- **Random seed:** 42 (deterministic -- all results exactly reproducible)
- **Confidence interval:** 95% percentile bootstrap CI
- **Significance criterion:** CI lower bound > 0.50 (confirmed for all 39 oncology cohorts)
- **Pipeline:** BPF Locked Pipeline v1.0.0, executed February 11, 2026
- **No cohort-specific tuning:** Identical parameters applied across all cohorts

---

## Portfolio Context

This result is part of the BPF Phase 1 oncology validation:

- **39 cohorts** | **16,958 patients** | **Mean AUC 0.8077** (95% CI 0.7722-0.8430)
- 21 GOLD | 9 CONDITIONAL | 9 EXPLORATORY
- 100% statistical significance (bootstrap CI excludes 0.50 for all 39 cohorts)
- Data source: UCSC Xena Browser (harmonized TCGA, GDC, CGCI)

---

*PulseLogic Biosciences Inc. | BPF Locked Pipeline v1.0.0 | ceo@pulselogic.bio*

