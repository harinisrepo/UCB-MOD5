# UCB-MOD5
# Coupon Acceptance Analysis — Summary & Notebook Link

**Author:** Tadinada, Harini  
**Student:** UC Berkeley ML/AI Professional Certificate Program

---

## Overview
This project analyzes coupon acceptance behavior using the `coupons.csv` dataset. The goal was to identify patterns and drivers of coupon acceptance across different categories (Bar, Coffee House, Cheap Restaurants, etc.) and contextual attributes.

---

## Key Findings (Percent-based)

### Overall Acceptance
- About **50%** of all coupons were accepted.

### Bar Coupons
- Acceptance increases with bar visit frequency: from ~19% (never) to ~78% (4–8 times/month).
- Younger drivers (<30) and social trips (with friends) show higher acceptance.
- Evening timing and short detours improve acceptance.

### Coffee House Coupons
- Overall acceptance: ~49.9%.
- Habit alignment: frequent coffeehouse visitors accept more (up to ~69%).
- Social context matters: with friends (~60%) > alone (~44%).
- Morning (10AM) and midday (2PM) are prime windows.
- Lower income (<$50K) and younger drivers show modest lifts.

### Cheap Restaurants & Income
- Drivers visiting cheap restaurants >4 times/month and earning <50K accept at ~60%, vs ~56% baseline.

---

## Visualizations
- charts for:
  - Coupon Distribution by coupon type bar chart
  - Coupon Acceptance by temperature distribution histogram
  - Coupon Acceptance by bar visits 1x/month and Age> 25 vs rest of population bar chart
  - Coupon Acceptance by bar visits 1x /month and Age< 30 and  had passengers that were not a kid, and were not widowed 
---

## Hypotheses
- Habit alignment and social context are primary drivers.
- Timing and convenience (short detours) strongly influence acceptance.
- Price sensitivity plays a secondary role compared to behavioral patterns.

---

## How to Reproduce
1. Load `coupons.csv`.
2. Clean data (parse income and age, normalize frequency buckets).
3. Compute acceptance rates by segments.
4. Visualize using bar charts (percent only).

---
## Tools Used
Python 3.x
pandas - data manipulation
NumPy - numerical operations
Matplotlib & Seaborn - visualizations

## Jupyter Notebook
Access the full analysis and code here: https://github.com/harinisrepo/UCB-MOD5/blob/main/MOD5%20Assignment.ipynb


---

## Next Steps
- Build a dashboard summarizing top drivers.
- Fit logistic regression for independent effects.
- Package insights into a presentation for stakeholders.

