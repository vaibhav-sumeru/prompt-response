# Evaluation Report: review-signoff-summary

**System Prompt:** v1.md
**Date:** 2026-03-05
**Variations Tested:** 13

## 🎯 PRIMARY METRIC: Numeric Accuracy

| Metric | Value | Status |
|--------|-------|--------|
| Average Numeric Accuracy | 100.0% | ✅ PASS |
| Variations with 100% Numeric Match | 10/13 | |
| Variations with Numeric Mismatches | 0/13 | |
| Total Numeric Mismatches Found | 0 | |

---

## 📋 Overall Evaluation Summary

| Metric | Value |
|--------|-------|
| **Total Variations** | 13 |
| **Overall Average Score** | 75.4/100 |
| ✅ **PASS** | 9 |
| ⚠️ **PARTIAL** | 1 |
| ❌ **FAIL** | 3 |

### Weighted Score Breakdown

| Criterion | Weight | Avg Score | Status |
|-----------|--------|-----------|--------|
| 🔴 Numeric Accuracy | 50% | 100.0% | ✅ |
| Entity Accuracy | 15% | 100.0% | ✅ |
| Ranking Accuracy | 10% | 100.0% | ✅ |
| Coverage Completeness | 10% | 92.4% | ✅ |
| Formatting Compliance | 10% | 89.0% | ⚠️ |
| Mathematical Consistency | 5% | 100.0% | ✅ |

---

## Per-Variation Results

| Variation | Category | Score | Numeric | Entity | Ranking | Coverage | Format | Math |
|-----------|----------|-------|---------|--------|---------|----------|--------|------|
| variation-01 | normal-balanced | PASS (97) | PASS | PASS | PASS | PARTIAL | PARTIAL | PASS |
| variation-02 | normal-balanced | PASS (96.97) | PASS | PASS | PASS | 35/39 | PARTIAL | PASS |
| variation-03 | extreme-skew | PASS (95.33) | PASS | PASS | PASS | PARTIAL | PARTIAL | PASS |
| variation-04 | extreme-skew | PASS (100) | PASS | PASS | PASS | 100/100 | PASS | PASS |
| variation-05 | zero-values | PASS (99.33) | PASS | PASS | PASS | 28/30 | PASS | PASS |
| variation-06 | zero-values | FAIL (-) | - | - | - | - | - | - |
| variation-07 | single-schedule | PARTIAL (99) | PASS | PASS | PASS | PASS | PARTIAL | PASS |
| variation-08 | all-healthy | PASS (97.06) | PASS | PASS | PASS | PARTIAL | PARTIAL | PASS |
| variation-09 | all-worst | PASS (95) | PASS | PASS | PASS | 29/33 | PARTIAL | PASS |
| variation-10 | missing-fields | FAIL (-) | - | - | - | - | - | - |
| variation-11 | all-accepted-zero-nonaccepted | FAIL (-) | - | - | - | - | - | - |
| variation-12 | one-prior-schedule-only | PASS (100) | PASS | PASS | PASS | PASS | PASS | PASS |
| variation-13 | prior-fully-finalized-current-mixed | PASS (100) | PASS | PASS | PASS | 29/29 | PASS | PASS |

---

## 🔧 Action Items (Prioritized by Numeric Impact)

### MEDIUM PRIORITY (Coverage Issues)

1. Add explicit requirement for **signoffStatusBySchedule.rows[1].scheduleId (S-2023-Q4)** (missing in 2 variations)
2. Add explicit requirement for **signoffStatusBySchedule.rows[2].scheduleId (S-2024-Q1)** (missing in 2 variations)
3. Add explicit requirement for **signoffStatusBySchedule.rows[1].closureHealthScore (84.1)** (missing in 1 variations)

---


## Frequently Missing Data Points

- **signoffStatusBySchedule.rows[1].scheduleId (S-2023-Q4)** — missing in 2/13 variations
- **signoffStatusBySchedule.rows[2].scheduleId (S-2024-Q1)** — missing in 2/13 variations
- **signoffStatusBySchedule.rows[1].closureHealthScore (84.1)** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[2].closureHealthScore (85.7)** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[1].scheduleId (S-2024-Q1)** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[1].closureHealthScore (87.2)** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[2].scheduleId (S-2024-Q2)** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[2].closureHealthScore (89.9)** — missing in 1/13 variations
- **Bullet 1: signoffStatusBySchedule.rows[1].scheduleId (S-2023-Q4) and its closureHealthScore (66.6) are missing.** — missing in 1/13 variations
- **Bullet 1: signoffStatusBySchedule.rows[2].scheduleId (S-2024-Q1) and its closureHealthScore (76.7) are missing.** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[2].scheduleId (S-2024-Q1) - The prompt required 'All schedule IDs and their closureHealthScores' to appear, but S-2024-Q1 was not explicitly named.** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[2].closureHealthScore (90.9) - The closure health score for S-2024-Q1 was not explicitly mentioned.** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[2].scheduleId (S-2024-Q2) was not explicitly mentioned.** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[0].closureHealthScore (98.5 for S-2023-Q4) was not explicitly mentioned.** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[2].closureHealthScore (98.2 for S-2024-Q2) was not explicitly mentioned.** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[1].closureHealthScore (17.3)** — missing in 1/13 variations
- **signoffStatusBySchedule.rows[2].closureHealthScore (18.3)** — missing in 1/13 variations

## Formatting Issues

- The risk level name 'Zero Tolerance' was not bolded, despite having the highest nonAcceptedPctOfRisk (33.3%) as required by the prompt. (1/13 variations)
- Bullet 3 exceeds the maximum word count (70 words; max 60 allowed). (1/13 variations)
- Percentage '46%' should be formatted as '46.0%' as per the 'XX.X%' rule. (1/13 variations)
- The risk level name 'Zero Tolerance' should be bolded as it has the single highest nonAcceptedPctOfRisk (80.0%) across all 4 rows, as per bolding rules. (1/13 variations)
- Exactly 3 dash bullets, each starting with '- **Section Label:**'. (1/13 variations)
- Single newline separation between bullets. (1/13 variations)
- Bullet lengths are within the specified ranges (60 words for bullet 1, 60 words for bullet 2, 60 words for bullet 3). (1/13 variations)
- Tone is clinical and data-dense. (1/13 variations)
- No numbers or percentages to format, so no issues there. (1/13 variations)
- No bolding applied as no positive values were present, which is correct. (1/13 variations)
- No banned phrases used. (1/13 variations)
- No date formatting issues as no dates were present. (1/13 variations)
- In Bullet 3, the risk level name 'Zero Tolerance' should be bolded as it has the highest nonAcceptedPctOfRisk (53.3%) across all risk levels, as per prompt instructions. (1/13 variations)
- Bullet 3 exceeds the maximum word count (66 words; max 60 allowed). (1/13 variations)
- Bullet 3 exceeds the maximum word count (86 words; max 60 words). (1/13 variations)

## Suggestions for System Prompt Improvement

1. COVERAGE: Ensure all four schedule IDs and their respective closure health scores are explicitly mentioned in the 'Schedule Closure Trend' bullet, as per the 'Required Data Points' instruction, even if intermediate schedules are also referenced by trend direction.
2. COVERAGE: Ensure all 4 schedule IDs and their closure health scores are explicitly mentioned in Bullet 1, as per the 'Required Data Points' list, even when describing a trend.
3. FORMATTING: Reduce the word count of Bullet 3 to adhere to the 30-60 word limit.

## Word Count Distribution

| Paragraph | Min | Max | Avg | Out of Range |
|-----------|-----|-----|-----|-------------|
