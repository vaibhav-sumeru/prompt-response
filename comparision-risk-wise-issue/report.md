# Evaluation Report: comparision-risk-wise-issue

**System Prompt:** v1.md
**Date:** 2026-02-27
**Variations Tested:** 20

## 🎯 PRIMARY METRIC: Numeric Accuracy

| Metric | Value | Status |
|--------|-------|--------|
| Average Numeric Accuracy | 100.0% | ✅ PASS |
| Variations with 100% Numeric Match | 20/20 | |
| Variations with Numeric Mismatches | 0/20 | |
| Total Numeric Mismatches Found | 0 | |

---

## 📋 Overall Evaluation Summary

| Metric | Value |
|--------|-------|
| **Total Variations** | 20 |
| **Overall Average Score** | 99.9/100 |
| ✅ **PASS** | 20 |
| ⚠️ **PARTIAL** | 0 |
| ❌ **FAIL** | 0 |

### Weighted Score Breakdown

| Criterion | Weight | Avg Score | Status |
|-----------|--------|-----------|--------|
| 🔴 Numeric Accuracy | 50% | 100.0% | ✅ |
| Entity Accuracy | 15% | 100.0% | ✅ |
| Ranking Accuracy | 10% | 100.0% | ✅ |
| Coverage Completeness | 10% | 100.0% | ✅ |
| Formatting Compliance | 10% | 99.5% | ✅ |
| Mathematical Consistency | 5% | 100.0% | ✅ |

---

## Per-Variation Results

| Variation | Category | Score | Numeric | Entity | Ranking | Coverage | Format | Math |
|-----------|----------|-------|---------|--------|---------|----------|--------|------|
| variation-01 | normal-balanced | PASS (100) | PASS | PASS | PASS | 15/15 | PASS | PASS |
| variation-02 | normal-balanced | PASS (100) | PASS | PASS | PASS | 14/14 | PASS | PASS |
| variation-03 | extreme-skew | PASS (100) | PASS | PASS | PASS | 20/20 | PASS | PASS |
| variation-04 | extreme-skew | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-05 | zero-values | PASS (100) | PASS | PASS | PASS | 15/15 | PASS | PASS |
| variation-06 | zero-values | PASS (99) | PASS | PASS | PASS | 12/12 | PARTIAL | PASS |
| variation-07 | single-zone | PASS (100) | PASS | PASS | PASS | 13/13 | PASS | PASS |
| variation-08 | all-perfect | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-09 | all-worst | PASS (100) | PASS | PASS | PASS | 20/20 | PASS | PASS |
| variation-10 | missing-fields | PASS (100) | PASS | PASS | PASS | 15/15 | PASS | PASS |
| variation-11 | identical-periods | PASS (100) | PASS | PASS | PASS | 13/13 | PASS | PASS |
| variation-12 | entity-cluster | PASS (100) | PASS | PASS | PASS | 15/15 | PASS | PASS |
| variation-13 | entity-audit-type | PASS (100) | PASS | PASS | PASS | 15/15 | PASS | PASS |
| variation-14 | entity-audit-type | PASS (99) | PASS | PASS | PASS | 14/14 | PARTIAL | PASS |
| variation-15 | entity-audit-type | PASS (100) | PASS | PASS | PASS | 21/21 | PASS | PASS |
| variation-16 | entity-audit-type | PASS (100) | PASS | PASS | PASS | 16/16 | PASS | PASS |
| variation-17 | entity-audit-type | PASS (100) | PASS | PASS | PASS | 14/14 | PASS | PASS |
| variation-18 | complex-dates | PASS (100) | PASS | PASS | PASS | 15/15 | PASS | PASS |
| variation-19 | missing-change-pct | PASS (100) | PASS | PASS | PASS | 18/18 | PASS | PASS |
| variation-20 | all-improved | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |

---

## 🔧 Action Items (Prioritized by Numeric Impact)

---


## Formatting Issues

- Bullet 2 is approximately 18 words, slightly below 20-word minimum; otherwise compliant with header, structure, bolding, and period labeling. (1/20 variations)
- Bullet 2 word count approximately 18, slightly under the 20-40 word requirement. (1/20 variations)
- All bullets 20-40 words: Bullet 1 (28 words), Bullet 2 (20 words), Bullet 3 (28 words). Period labels correctly wrapped in (*...*). Header exact match. (1/20 variations)

## Suggestions for System Prompt Improvement

1. FORMATTING: Enforce stricter word count checks for bullets to ensure 20-40 words minimum.
2. COVERAGE: Confirm all mandatory data points are explicitly stated without omission in future generations.
3. None required; response fully compliant.

## Word Count Distribution

| Paragraph | Min | Max | Avg | Out of Range |
|-----------|-----|-----|-----|-------------|
