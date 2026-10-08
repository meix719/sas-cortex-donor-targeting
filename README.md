# NYU SPS × SAS Cortex Challenge: Donor Targeting

## Overview
This team project used predictive modeling in the SAS Cortex fundraising simulation to select donors for a promotional mug campaign. Our goal was to maximize operating surplus by balancing expected donations with campaign expenses.

## Achievement
Our team placed **2nd on the final leaderboard** in the 2026 NYU SPS × SAS Cortex Challenge.

## Business Question
Which donors should receive a promotional mug to maximize total donations minus campaign expenses?

## Modeling Approach
We used a two-stage modeling framework:
1. Predict the probability that a donor will give.
2. Predict the donation amount conditional on giving.

We scored donors under two scenarios: receiving outreach and receiving no outreach.

Expected donation = probability of giving × expected amount if giving

Predicted uplift = expected donation with outreach − expected donation without outreach

Our presentation describes selecting donors with predicted uplift greater than $5. The challenge listed a $5 cost per mug for up to 60,000 mugs and a higher $25 cost beyond that tier, making campaign size an important part of the decision.

## Tools and Skills
- SAS predictive modeling tools
- Gradient boosting model pipelines
- Two-stage donation modeling
- Uplift-based donor targeting
- Campaign cost analysis
- Dashboard interpretation and business communication

## Challenge Results
Our presentation reported the following simulation dashboard results:

| Metric | Reported Value |
|---|---:|
| Operating surplus | $8,791,995 |
| Campaign expenses | $300,000 |
| Donors contacted | 60,000 |

Operating surplus represents total donations minus expenses. These are simulation results, not verified real-world fundraising outcomes or the incremental gain caused by outreach.

## Business Takeaway
The donors most likely to give are not necessarily the best outreach targets. Effective targeting considers how much outreach is expected to increase donations and whether that increase exceeds campaign costs.

## Project Materials
[View our team presentation](reports/sas-cortex-presentation.pdf)

This repository presents the project as a portfolio case study. Source data and executable model files are not included.

## Limitations
- Predicted returns do not guarantee a profitable outcome for every donor.
- The presentation does not provide enough validation detail to independently confirm generalization or rule out overfitting.
- Interpreting uplift as a causal effect requires an appropriate study design and assumptions.
- Real-world implementation would require further validation and consideration of donor privacy and outreach preferences.

## Team
Ariana Li, Qunfeng Zhou, Mei Qiong Xue, and Jinyi Yuan.

## My Contribution
I built and tested predictive models for donation probability and donation amount, using the results to support the team’s donor-targeting strategy.
