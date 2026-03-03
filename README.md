Marketing Channel Performance Analysis (Google Analytics Sample)
Overview

This project analyses marketing channel performance to identify where traffic volume does not translate into session quality, and where optimisation efforts should focus.

Business Question

Which channels drive the most sessions, and which channels drive the highest-quality sessions relative to their traffic share?

Dataset

Google Analytics Marketing Channel dataset (provided as CSV).

Key fields used:

Channel

Total Sessions

High Quality Rate (high-quality sessions as a % of total sessions)

Traffic Share

Quality Share

Performance Gap (Quality Share − Traffic Share)

Approach

Traffic concentration

Calculated traffic share by channel to identify dominant sources.

Efficiency (quality rate)

Compared channels by their high-quality session rate.

Performance gap

Visualised where channels underperform (high traffic but lower quality share) vs overperform.

Key Findings

Google / Organic drives ~31% of traffic but under-indexes on quality relative to its traffic share.

Direct shows similar underperformance.

Referral and Shop Referral show higher efficiency (higher quality per session).

Recommendations (What I would test next)

Improve organic quality: break organic traffic into segments (intent + landing page) to identify where low-quality visits originate.

Investigate direct attribution: verify whether “direct” contains misclassified traffic (missing UTM tags, redirects).

Scale high-performing referrals: identify referral partners/pages driving high-quality sessions and expand them.

Model budget reallocation: simulate shifting effort/spend from underperformers to high-performing segments.

Tools Used

Tableau Public (visualisations)

SQL / spreadsheet calculations (aggregation + derived metrics)

PowerPoint (final presentation)

Links

Tableau Public Dashboard: https://public.tableau.com/views/MarketingChannelPerformance_17696986047020/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

GitHub Repository: (this repo)