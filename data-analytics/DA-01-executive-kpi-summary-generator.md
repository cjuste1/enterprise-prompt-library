# DA-01 · Executive KPI Summary Generator

![Category](https://img.shields.io/badge/Category-Data%20Analytics-6366F1?style=flat)
![Industry](https://img.shields.io/badge/Industries-4-c9943a?style=flat)
![Method](https://img.shields.io/badge/Method-MASTER-22c55e?style=flat)

## Purpose
Transform raw KPI data into a C-suite ready 
executive summary written for a CEO with 
90 seconds to read it.

---

## Industries
Finance · Healthcare · Retail · Operations

---

## Input Variables
| Variable | Description |
|----------|-------------|
| {{kpi_data_json}} | Raw KPI data in JSON format |
| {{period}} | Reporting period e.g. Q3 2026 |
| {{business_unit}} | Department or division name |
| {{strategic_goals}} | Top 3 goals for the period |

---

## The Prompt
```
You are a senior data analyst preparing a briefing 
for the C-suite. Your job is to transform raw data 
into a clear, confident executive summary.

The CEO has 90 seconds to read this.
Every word must earn its place.

KPI Data: {{kpi_data_json}}
Reporting Period: {{period}}
Business Unit: {{business_unit}}
Strategic Goals: {{strategic_goals}}

Deliver your summary in this exact format:

HEADLINE: [1 sentence — most important insight]

PERFORMANCE SNAPSHOT:
- [Metric 1]: [Value] 🟢/🟡/🔴
- [Metric 2]: [Value] 🟢/🟡/🔴
- [Metric 3]: [Value] 🟢/🟡/🔴
- [Metric 4]: [Value] 🟢/🟡/🔴
- [Metric 5]: [Value] 🟢/🟡/🔴

TOP WIN: [1 sentence]
TOP CONCERN: [1 sentence]

TREND ANALYSIS: [2-3 sentences]

RECOMMENDED ACTIONS:
1. [Action — Owner — Timeline]
2. [Action — Owner — Timeline]
3. [Action — Owner — Timeline]

FORWARD OUTLOOK: [1-2 sentences]
```

---

## Performance Targets
- Executive satisfaction score >4/5
- Action item adoption rate tracked monthly
- Time to brief reduced vs manual preparation
- Summary length under 250 words

---

## Iteration Notes
- Include prior period data for trend accuracy
- Add industry benchmarks when available
- Adjust status indicators per company thresholds
- Healthcare: include patient outcome metrics
- Retail: prioritize revenue and inventory metrics

---

## Example Output
```
HEADLINE: Revenue exceeded target by 12% but 
customer acquisition cost rising — immediate 
attention required.

PERFORMANCE SNAPSHOT:
- Revenue: $4.2M vs $3.7M target 🟢
- Customer Acquisition Cost: $142 vs $98 target 🔴
- Customer Satisfaction: 4.3/5 🟢
- Employee AI Adoption: 34% 🟡
- Operational Cost: $1.1M vs $1.0M target 🟡

TOP WIN: Revenue performance strongest quarter 
in 18 months driven by enterprise segment growth.

TOP CONCERN: Customer acquisition cost 45% over 
target — marketing spend efficiency requires 
immediate strategic review.
```

---

*Built by Chrystelle Juste · AI Enablement Strategist*
*[Portfolio](https://notion.so) · 
[LinkedIn](https://linkedin.com)*
