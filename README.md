# TikTok Content Integrity Analysis

## Overview
Exploratory data analysis of TikTok videos to understand engagement patterns
across claim vs opinion content, verified vs unverified authors,
and active vs banned accounts.

## Dataset
- Source: [TikTok User Engagement Data](https://www.kaggle.com/datasets/yakhyojon/tiktok)
- 19,382 rows, 12 columns
- Each row represents a published TikTok video

## Tools Used
- Python, pandas, matplotlib, seaborn

## Key Findings So Far
- Claim videos receive ~100x more views than opinion videos on average
  (501,029 vs 4,956), suggesting significantly higher spread on the platform
- Counterintuitively, unverified authors outperform verified authors in average
  views (265,663 vs 91,439), likely driven by banned or flagged accounts
  inflating the unverified group's numbers
- Banned accounts generated more than double the average views of active accounts
  (445,845 vs 215,927), suggesting engagement velocity may be an early signal
  for accounts that violate platform policies
