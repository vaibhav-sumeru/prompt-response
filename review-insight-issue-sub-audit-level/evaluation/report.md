# Evaluation Report: review-insight-issue-sub-audit-level

**System Prompt:** v3.md
**Date:** 2026-03-02
**Variations Tested:** 11

## 🎯 PRIMARY METRIC: Numeric Accuracy

| Metric | Value | Status |
|--------|-------|--------|
| Average Numeric Accuracy | 54.5% | ❌ FAIL |
| Variations with 100% Numeric Match | 6/11 | |
| Variations with Numeric Mismatches | 5/11 | |
| Total Numeric Mismatches Found | 24 | |

### 🔴 CRITICAL: Numeric Mismatches Breakdown

| Variation | Mismatch Count | Example Mismatch |
|-----------|----------------|------------------|
| variation-03 | 5 | Found: 10, Expected: none |
| variation-07 | 4 | Found: 10, Expected: none |
| variation-08 | 4 | Found: 10, Expected: none |
| variation-09 | 5 | Found: 10, Expected: none |
| variation-11 | 6 | Found: 10, Expected: none |

### 📊 Most Common Numeric Errors

1. **no match** — 9 mismatches across 5 variations
2. **no matching path** — 6 mismatches across 5 variations
3. **no match in schema** — 5 mismatches across 5 variations
4. **none** — 4 mismatches across 5 variations

---

## 📋 Overall Evaluation Summary

| Metric | Value |
|--------|-------|
| **Total Variations** | 11 |
| **Overall Average Score** | 65.6/100 |
| ✅ **PASS** | 6 |
| ⚠️ **PARTIAL** | 0 |
| ❌ **FAIL** | 5 |

### Weighted Score Breakdown

| Criterion | Weight | Avg Score | Status |
|-----------|--------|-----------|--------|
| 🔴 Numeric Accuracy | 50% | 54.5% | ❌ |
| Entity Accuracy | 15% | 54.5% | ❌ |
| Ranking Accuracy | 10% | 59.1% | ❌ |
| Coverage Completeness | 10% | 94.2% | ✅ |
| Formatting Compliance | 10% | 96.4% | ✅ |
| Mathematical Consistency | 5% | 100.0% | ✅ |

---

## Per-Variation Results

| Variation | Category | Score | Numeric | Entity | Ranking | Coverage | Format | Math |
|-----------|----------|-------|---------|--------|---------|----------|--------|------|
| variation-01 | var-05-all-stable | PASS (98) | PASS | PASS | PASS | 16/16 | PARTIAL | PASS |
| variation-02 | var-06-all-increasing | PASS (100) | PASS | PASS | PASS | 16/16 | PASS | PASS |
| variation-03 | var-07-all-decreasing | FAIL (24) | FAIL | FAIL | FAIL | 14/15 | PASS | PASS |
| variation-04 | var-08-no-persistent | PASS (100) | PASS | PASS | PASS | 18/18 | PASS | PASS |
| variation-05 | var-09-multiple-persistent | PASS (98) | PASS | PASS | PASS | 41/48 | PASS | PASS |
| variation-06 | var-10-tie-breaker-issues | PASS (98) | PASS | PASS | PASS | 40/48 | PASS | PASS |
| variation-07 | var-11-one-prev-schedule | FAIL (29) | FAIL | FAIL | PARTIAL | 15/16 | PASS | PASS |
| variation-08 | var-12-zero-issues-current | FAIL (22) | FAIL | FAIL | FAIL | 15/16 | PARTIAL | PASS |
| variation-09 | var-13-extreme-skew | FAIL (24) | FAIL | FAIL | FAIL | 15/16 | PASS | PASS |
| variation-10 | var-14-uniform-distribution | PASS (100) | PASS | PASS | PASS | 24/24 | PASS | PASS |
| variation-11 | var-15-max-trend-buckets | FAIL (29) | FAIL | FAIL | FAIL | 15/16 | PASS | PASS |

---

## 🔧 Action Items (Prioritized by Numeric Impact)

### HIGH PRIORITY (Numeric Accuracy Issues)

1. Fix numeric accuracy for **no match** (9 occurrences)
2. Fix numeric accuracy for **no matching path** (6 occurrences)
3. Fix numeric accuracy for **no match in schema** (5 occurrences)

### MEDIUM PRIORITY (Coverage Issues)

1. Add explicit requirement for **meta.currentScheduleId (not mentioned in Trend Movement paragraph)** (missing in 2 variations)
2. Add explicit requirement for **topByTotalIssues[4].averageIssuesAllSchedules (Vendor Management average not mentioned)** (missing in 1 variations)
3. Add explicit requirement for **trendBuckets.increasing[1].* (Payroll Processing details not covered)** (missing in 1 variations)

---


## Recurring Numeric Mismatches

| JSON Path / Paragraph | Frequency | Severity |
|-----------------------|-----------|----------|
| no match | 9/11 | 🔴 High |
| no matching path | 6/11 | 🔴 High |
| no match in schema | 5/11 | 🟡 Medium |
| none | 4/11 | 🟡 Medium |

## Frequently Missing Data Points

- **meta.currentScheduleId (not mentioned in Trend Movement paragraph)** — missing in 2/11 variations
- **topByTotalIssues[4].averageIssuesAllSchedules (Vendor Management average not mentioned)** — missing in 1/11 variations
- **trendBuckets.increasing[1].* (Payroll Processing details not covered)** — missing in 1/11 variations
- **trendBuckets.increasing[2].* (Vendor Management increasing details not covered)** — missing in 1/11 variations
- **trendBuckets.decreasing[1].* (Data Privacy details not covered)** — missing in 1/11 variations
- **trendBuckets.stable[2].currentIssueCount and previousAverageIssueCount (Procurement counts not mentioned)** — missing in 1/11 variations
- **trendBuckets.stable[1].currentIssueCount and previousAverageIssueCount (Human Resources counts not explicitly stated in trend paragraph)** — missing in 1/11 variations
- **totals.totalIssuesCurrentSchedule and totalIssuesPreviousSchedules (not mentioned)** — missing in 1/11 variations
- **averageIssuesAllSchedules for Internal Controls Check (10) and Operational Audit (7.5)** — missing in 1/11 variations
- **previousAverageIssueCount for all trend items (e.g., 10 for Financial Reporting Audit)** — missing in 1/11 variations
- **subAuditName and metrics for stable bucket items Vendor Management Audit and IT Security Review** — missing in 1/11 variations
- **meta.currentScheduleId (not explicitly mentioned in Paragraph 2)** — missing in 1/11 variations
- **meta.currentScheduleId** — missing in 1/11 variations
- **meta.currentScheduleId (not explicitly mentioned in Trend Movement paragraph)** — missing in 1/11 variations

## Formatting Issues

- Paragraph 2 exceeds 60-word limit (approximately 70 words). (1/11 variations)
- All paragraphs 30-60 words: Para1 ~48, Para2 ~58, Para3 ~38. (1/11 variations)
- Correct bold labels and formatting. (1/11 variations)
- No date issues. (1/11 variations)
- Paragraph 1 word count 67 (exceeds 30-60 limit) (1/11 variations)
- Issue counts in Paragraph 2 (e.g., 120, 70) not bolded despite >0, inconsistent with bolding rule for counts (1/11 variations)

## Suggestions for System Prompt Improvement

1. FORMATTING: Enforce stricter word count limits in generation prompt to ensure 30-60 words per paragraph.
2. COVERAGE: Consider explicit checklist validation in self-check to confirm all required data points.
3. NUMERIC: Input data is schema only, not instance data; all numbers hallucinated. Provide actual JSON payload for evaluation.
4. ENTITY: Response invents sub-audit names; enforce 'Not Available' for missing instance data.
5. COVERAGE: Missing explicit mention of currentScheduleId; instruct to include or note as 'Not Available' if absent.
6. COVERAGE: Instruct to include averageIssuesAllSchedules for all topByTotalIssues items, even if briefly
7. COVERAGE: Require explicit mention of counts for at least two examples per trend bucket to improve completeness
8. TREND: Ensure stable bucket examples include current and previous counts for full data point coverage
9. COVERAGE: Instruct to explicitly include previousAverageIssueCount in trend narration for completeness
10. COVERAGE: Ensure all up to 3 items per trend bucket are mentioned if space allows within word limit
11. NUMERIC: Input data is schema only; provide actual instance data for accurate numeric verification
12. ENTITY: Ensure entity names are extracted directly from payload; flag hallucinations when no data present
13. NUMERIC: Response hallucinates all numbers; instruct to use 'Not Available' for missing payload data beyond schema
14. ENTITY: Enforce strict no-hallucination for names; schema has no entities, so output should note absence
15. Input data is schema only, lacking actual payload; all numeric and entity values in response are hallucinated
16. Enforce strict validation against actual data instances, not schema, to prevent invention of values
17. Provide populated JSON data instead of schema in input_data to enable accurate numeric and entity verification
18. Instruct AI to output 'Not Available' for all metrics when no actual data payload is provided

## Word Count Distribution

| Paragraph | Min | Max | Avg | Out of Range |
|-----------|-----|-----|-----|-------------|
