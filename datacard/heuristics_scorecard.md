# 📊 Data Card Heuristics Scorecard — Self-Assessment

**Dataset:** IMDB Movie Review Dataset (CSC4007 Lab v1.0)  
**Date:** 2026-04-12  
**Assessor:** CSC4007-NLP Student  
**Purpose:** Self-evaluation of Data Card completeness, accuracy, clarity, timeliness, and actionability

---

## 📋 **Scoring Rubric (1-5 Scale)**

| Score | Definition | Example |
|-------|-----------|---------|
| 1 | Critical gaps; not usable | Missing key metrics, no audit trail, unclear status |
| 2 | Major issues; incomplete | Some metrics present but many estimated; lacks detail |
| 3 | Adequate; acceptable for lab | Core metrics verified; some gaps; mostly clear |
| 4 | Good; ready to use | Most metrics verified; minor gaps; clear + actionable |
| 5 | Excellent; comprehensive | All metrics verified; thorough; clear; well-structured |

---

## 🎯 **5 Evaluation Criteria**

### **1. COMPLETENESS (Covers all necessary topics) — Score: 5/5** ⭐⭐⭐⭐⭐

**Definition:** Data Card addresses all 15 core themes + critical issues

All 15 themes fully covered + 3 foundational questions answered. No major gaps.
- Module 1 (ASK): 5 personas + 7 scopes ✅
- Module 2 (INSPECT): Verified/Estimated/To-be-measured checklist ✅
- Module 3 (ANSWER): 15 themes detailed ✅
- Module 4 (AUDIT): This scorecard ✅

---

### **2. ACCURACY (Numbers verified) — Score: 4.5/5** ⭐⭐⭐⭐

**Definition:** All claims backed by outputs; no contradictions; precise measurements

**Verification Checklist:**

| Claim | Source | Value | Status |
|-------|--------|-------|--------|
| **50,000 records** | `datacard_stats.json` | ✅ Verified | YES |
| **25k/25k balanced** | `datacard_stats.json` | ✅ Verified | YES |
| **40k/5k/5k splits** | `datacard_stats.json` | ✅ Verified | YES |
| **954 char median** | `datacard_stats.json` | ✅ Verified | YES |
| **13,593 max length** | `datacard_stats.json` | ✅ Verified | YES |
| **HTML: 29,202 → 0** | audit_before + audit_after | ✅ Verified | YES |
| **832 duplicates** | `datacard_stats.json` | ✅ Verified | YES |
| **GE: 5/6 PASS** | `validation_summary.md` | ✅ Verified | YES |
| **1,000 Cleanlab issues** | `cleanlab_summary.md` | ✅ Verified | YES |
| **5 manual reviews** | `cleanlab_label_issues.csv` | ✅ Verified | YES |

**Minor Issues:**
- ❌ (1) GE validation still FAIL (unresolved but documented)
- ⚠️ (2) Some metrics estimated (duplicate distribution, label error rate)

---

### **3. CLARITY (Well-organized; actionable) — Score: 4.5/5** ⭐⭐⭐⭐

**Definition:** Clear structure, visual hierarchy, understandable; easy to find info

**Strengths:**
- ✅ Module structure obvious (1→4)
- ✅ Emoji + color coding (🔴🟡✅)
- ✅ Tables for dense data
- ✅ Priorities clearly marked
- ✅ 3 foundational Q's upfront

**Areas:**
- ⚠️ Could add executive summary
- ⚠️ Table of contents would help (long doc)

---

### **4. TIMELINESS (Current; recent data) — Score: 5/5** ⭐⭐⭐⭐⭐

**Definition:** Data Card current; metrics recent; no stale information

**Status:**
- ✅ Generated 2026-04-12 (today)
- ✅ Lab outputs same day (~15 min ago)
- ✅ All metrics fresh
- ✅ Version v1.0 clearly marked

---

### **5. ACTIONABILITY (Clear next steps; feasible; prioritized) — Score: 4/5** ⭐⭐⭐⭐

**Definition:** Reader knows exactly what to do; priorities clear

**Strengths:**
- ✅ CRITICAL / IMPORTANT / OPTIONAL tiers
- ✅ Specific actions with IDs (e.g., "11668→1")
- ✅ GE fail has 3 remediation options
- ✅ Cleanlab results with manual review

**Areas:**
- ⚠️ Could add time estimates (e.g., "1-2 days")
- ⚠️ Some "to be measured" items vague

---

## 📊 **OVERALL SCORE**

| Criterion | Score | Weight | Weighted |
|-----------|-------|--------|----------|
| Completeness | 5/5 | 20% | 1.0 |
| Accuracy | 4.5/5 | 25% | 1.125 |
| Clarity | 4.5/5 | 20% | 0.9 |
| Timeliness | 5/5 | 15% | 0.75 |
| Actionability | 4/5 | 20% | 0.8 |
| **FINAL** | **4.36 / 5** | 100% | **4.36** |

---

## ✅ **VERDICT**

```
╔══════════════════════════════════╗
║  Data Card Quality: ⭐⭐⭐⭐   ║
║  Score: 4.36 / 5.00              ║
║  Status: ✅ READY FOR SUBMISSION ║
╚══════════════════════════════════╝
```

### **Strengths**
- ✅ Complete coverage of all 15 themes
- ✅ Verified data from lab outputs
- ✅ Clear structure + visual hierarchy
- ✅ Current + actionable
- ✅ Troubling issues (GE fail, duplicates, label noise) well-documented

### **Next Steps (v1.1)**
1. **CRITICAL:** Fix GE validation (truncate texts >10k)
2. **IMPORTANT:** Correct 3 label errors; review 200 Cleanlab items
3. **OPTIONAL:** Add neutral class, per-movie stats, soft dedup

---

**Data Card Status: ✅ APPROVED**

*Signed: CSC4007-NLP Student | 2026-04-12*
