# TikTok Content Integrity Analysis

## Overview
Exploratory data analysis of TikTok videos to understand engagement patterns
across claim vs opinion content, verified vs unverified authors,
and active vs banned accounts.

This is Part 1 of a two-part data analytics portfolio. [Part 2](https://github.com/tkaixinn/user-retention-analysis) explores customer retention and user behaviour.
## Links
- Tableau Dashboard: [View on Tableau Public](https://public.tableau.com/app/profile/tkaixinn/viz/TikTok_Content_Integrity_Analysis/TikTokContentIntegrityDashboard)

## Dataset
- Source: [TikTok User Engagement Data](https://www.kaggle.com/datasets/yakhyojon/tiktok)
- 19,382 rows (19,084 clean rows), 12 columns
- Each row represents a published TikTok video

## Tools Used
- Python, pandas, matplotlib, seaborn, Tableau

## Questions Explored
1. Do claim videos or opinion videos get more engagement?
2. Does author verification status affect how far videos spread?
3. Do banned accounts show different engagement patterns?
4. Which combination of author status and content type drives the most engagement?
5. Is engagement concentrated among a small number of videos?

## Key Findings
1. Claim videos receive ~100x more views than opinion videos on average
   (501,029 vs 4,956)
2. Counterintuitively, unverified authors outperform verified authors in average
   views (265,663 vs 91,439). This may be influenced by accounts that were later
   banned or flagged within the unverified group
3. Accounts that were later banned generated more than double the average views of
   active accounts (445,845 vs 215,927), suggesting engagement velocity may be an
   early signal for accounts that violate platform policies
4. Accounts that were later banned posting claim videos accumulated the highest
   average views (505,907). However, claim videos attract ~500,000 views across
   all account states, suggesting content type is more strongly associated with
   viewership volume than author ban status
5. View distribution is highly concentrated. The top 20% of videos account for
   63.24% of all views, while the bottom 50% account for less than 1%