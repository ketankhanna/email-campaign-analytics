# 📬 Email Campaign Analytics

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ketankhanna/email-campaign-analytics/blob/main/campaign_analytics.ipynb)

A reusable post-send analysis for email campaigns, turned into one notebook. It's where my two worlds meet: marketing technology and the data science I studied at U of T.

## What it answers

| Question | How |
|---|---|
| Which programs earn clicks, and which burn out the list? | Weighted CTR vs. unsubscribe rate per program, as a bubble chart |
| Are we trending up or down? | Year-over-year CTR by program |
| Do audiences in different languages behave differently? | Language parsed from the campaign naming convention |
| Did the A/B test *really* win? | Two-proportion z-test with p-values, not just "B looks higher" |

## Data
**100% synthetic**, generated in the notebook with a fixed seed so the results are reproducible. No real customer, campaign or company data is used, and nothing reflects any employer. The code expects a standard export (`Campaignname`, `Sentdate`, `Delivered`, `Unique Clicks`, `Unsubscribe Clicks`), so it works on any email platform's report.

## Who did what
- **Me:** the analysis itself: which questions matter after a send, the metrics (weighted CTR, unsubscribe rate), the year-over-year, program and language breakdowns, and the takeaways.
- **AI assist (Claude):** rebuilt it as a clean public version: the synthetic data generator, the A/B significance test and the tidy notebook layout, so no real data ever leaves work.

## Run it
Click **Open in Colab** above and choose *Runtime → Run all*. Nothing to install.

## Tech
Python · pandas · seaborn · matplotlib · statistics (z-test)
