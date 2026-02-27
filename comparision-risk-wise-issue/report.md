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
| **Overall Average Score** | 99.7/100 |
| ✅ **PASS** | 20 |
| ⚠️ **PARTIAL** | 0 |
| ❌ **FAIL** | 0 |

### Weighted Score Breakdown

| Criterion | Weight | Avg Score | Status |
|-----------|--------|-----------|--------|
| 🔴 Numeric Accuracy | 50% | 100.0% | ✅ |
| Entity Accuracy | 15% | 100.0% | ✅ |
| Ranking Accuracy | 10% | 100.0% | ✅ |
| Coverage Completeness | 10% | 99.0% | ✅ |
| Formatting Compliance | 10% | 97.5% | ✅ |
| Mathematical Consistency | 5% | 100.0% | ✅ |

---

## Per-Variation Results

| Variation | Category | Score | Numeric | Entity | Ranking | Coverage | Format | Math |
|-----------|----------|-------|---------|--------|---------|----------|--------|------|
| variation-01 | normal-balanced | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-02 | normal-balanced | PASS (99) | PASS | PASS | PASS | 18/18 | PARTIAL | PASS |
| variation-03 | extreme-skew | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-04 | extreme-skew | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-05 | zero-values | PASS (100) | PASS | PASS | PASS | 21/21 | PASS | PASS |
| variation-06 | zero-values | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-07 | single-zone | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-08 | all-perfect | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-09 | all-worst | PASS (98) | PASS | PASS | PASS | 16/16 | PARTIAL | PASS |
| variation-10 | missing-fields | PASS (100) | PASS | PASS | PASS | 21/21 | PASS | PASS |
| variation-11 | identical-periods | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-12 | entity-cluster | PASS (100) | PASS | PASS | PASS | 21/21 | PASS | PASS |
| variation-13 | entity-audit-type | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-14 | entity-audit-type | PASS (100) | PASS | PASS | PASS | 15/15 | PASS | PASS |
| variation-15 | entity-audit-type | PASS (100) | PASS | PASS | PASS | 11/11 | PASS | PASS |
| variation-16 | entity-audit-type | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |
| variation-17 | entity-audit-type | PASS (98) | PASS | PASS | PASS | 14/14 | PARTIAL | PASS |
| variation-18 | complex-dates | PASS (98) | PASS | PASS | PASS | 16/20 | PASS | PASS |
| variation-19 | missing-change-pct | PASS (100) | PASS | PASS | PASS | 21/21 | PASS | PASS |
| variation-20 | all-improved | PASS (100) | PASS | PASS | PASS | 12/12 | PASS | PASS |

---

## 🔧 Action Items (Prioritized by Numeric Impact)

### MEDIUM PRIORITY (Coverage Issues)

1. Add explicit requirement for **Zero Tolerance T1 count (5)** (missing in 1 variations)
2. Add explicit requirement for **Zero Tolerance T2 count (3)** (missing in 1 variations)
3. Add explicit requirement for **High risk T1 count (10) in Bullet 1 context** (missing in 1 variations)

---


## Frequently Missing Data Points

- **Zero Tolerance T1 count (5)** — missing in 1/20 variations
- **Zero Tolerance T2 count (3)** — missing in 1/20 variations
- **High risk T1 count (10) in Bullet 1 context** — missing in 1/20 variations
- **High risk T2 count (12) in Bullet 1 context** — missing in 1/20 variations

## Formatting Issues

- Header date ranges use 'to' without italics/parentheses wrapping as per clarity rule for preventing run-on sentences. (1/20 variations)
- Header matches exactly. (2/20 variations)
- Period labels wrapped in (*...*) correctly. (1/20 variations)
- Bolding applied to increases per rules. (1/20 variations)
- Three bullets with correct structure. (1/20 variations)
- Header exact match. (1/20 variations)
- Three bullets with bold prefixes. (4/20 variations)
- Period labels italicized and parenthesized. (2/20 variations)
- Bullet 1 under 40 words. (1/20 variations)
- Bolding applied to change value per rules (increase). (1/20 variations)
- Date ranges wrapped in (*...*). (1/20 variations)
- Word counts approximate 15-35 per bullet, compliant with max 40 for Bullet 1. (1/20 variations)
- Bullet 2 (20 words) and Bullet 3 (32 words) fall below 30-word minimum per paragraph; date ranges correctly wrapped in (*...*). (1/20 variations)
- Header matches exact format. (2/20 variations)
- Period labels wrapped in (*...*). (1/20 variations)
- Word counts: Bullet 1 ~35 words, Bullet 2 ~20 words (within guidelines), Bullet 3 ~30 words. (1/20 variations)
- Bolding applied correctly for risk increases. (1/20 variations)
- Word counts compliant (Bullet 1 under 40 words). (1/20 variations)
- Missing bold prefixes for bullets 2 and 3 (should be '**High Risk Detailed Comparison:**' and '**Recurring Critical Risk Comparison:**') (1/20 variations)
- Bullet 2 and 3 word counts below 30 (15 and 28 words respectively), violating 30-60 word guideline per paragraph/bullet. (1/20 variations)

## Suggestions for System Prompt Improvement

1. Formatting: Ensure all date range references, including header, follow (*start* to *end*) pattern with italics for consistency.
2. Bolding: Confirm bolding rules applied correctly for risk increases.
3. FORMATTING: Enforce 30-60 word count strictly in bullet generation instructions to avoid short paragraphs.
4. COVERAGE: Ensure all bullets meet word minimums while covering required data points.
5. COVERAGE: Consider explicitly including Zero Tolerance counts in Bullet 1 if word limit allows for fuller detail.
6. FORMATTING: Bolding rules applied correctly for risk increases.
7. FORMAT: Enforce bold prefixes for all three bullets as specified in system prompt to ensure consistency.
8. COVERAGE: Add word count validation in generation to meet 30-60 words per bullet/paragraph guideline.
9. COVERAGE: Include T1 and T2 counts for Zero Tolerance and High risk explicitly in Bullet 1 to fully meet extraction steps, even in concise format.
10. NUMERIC: All numbers match, but monitor for future rounding in percentage diffs.

## Word Count Distribution

| Paragraph | Min | Max | Avg | Out of Range |
|-----------|-----|-----|-----|-------------|
