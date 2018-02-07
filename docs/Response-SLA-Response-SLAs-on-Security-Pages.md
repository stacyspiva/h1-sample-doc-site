---
id: Response-SLAs-on-Security-Pages
title: Response SLAs on Security Pages
---
We display a summarized version of a program’s response efficiency metric performance on their hacker facing security page. This enables you to set more realistic expectations with hackers regarding the amount of time it will take them to receive a first response, be paid a bounty, etc..

## Average Response Efficiency Metrics
A program’s average response efficiency metrics (calculated using a rolling 3 month average) are displayed on its security page. You can configure which metrics to display in **Settings** > **Program** > **Metrics Display**.

![Response SLA on Security Page Image 1](https://support.hackerone.com/hc/article_attachments/115018414966/mceclip0.png)

## Response Efficiency Indicator
A program’s current responsiveness state (based on performance against SLA targets) is displayed through a colored response efficiency indicator on its’ security page and report submission page. This provides additional context to potential hackers when they are looking to submit reports to your program.

![Response SLA on Security Page Image 2](https://support.hackerone.com/hc/article_attachments/115018414986/mceclip1.png)

## Indicator Types

Below are the indicator types and criteria:

Indicator Type | Criteria
-------------- | --------------
Green | All reports meet SLA target
Orange | ≥ 5 reports miss SLA target; no fails
Red | ≥ 1 report fails SLA limit
