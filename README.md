# 📬 Email Campaign Analytics

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ketankhanna/email-campaign-analytics/blob/main/campaign_analytics.ipynb)

The analysis I wish every email team ran after a send, turned into one reusable notebook. It's where my two worlds meet: I execute email campaigns in Adobe Campaign for a living, and I studied data science at U of T.

## What it answers

| Question | How |
|---|---|
| Which programs earn clicks, and which burn out the list? | Weighted CTR vs. unsubscribe rate per program, as a bubble chart |
| Are we trending up or down? | Year-over-year CTR by program |
| Do English and French audiences behave differently? | Language parsed from the campaign naming convention |
| Did the A/B test *really* win? | Two-proportion z-test with p-values, not just "B looks higher" |

## Data
**100% synthetic**, generated in the notebook with a fixed seed so the results are reproducible. No real customer, campaign or company data is used. The code expects a standard export (`Campaignname`, `Sentdate`, `Delivered`, `Unique Clicks`, `Unsubscribe Clicks`), so it drops straight onto a real Adobe Campaign or ESP report.

## Run it
Click **Open in Colab** above and choose *Runtime → Run all*. Nothing to install.

## Tech
Python · pandas · seaborn · matplotlib · statistics (z-test)
