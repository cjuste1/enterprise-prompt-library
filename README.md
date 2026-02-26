# Enterprise AI Prompt Library

![Prompts](https://img.shields.io/badge/Prompts-50-c9943a?style=flat)
![Categories](https://img.shields.io/badge/Categories-6-6366F1?style=flat)
![Industries](https://img.shields.io/badge/Industries-8%2B-22c55e?style=flat)
![Status](https://img.shields.io/badge/Status-Production%20Ready-22c55e?style=flat)

> **50 enterprise-grade prompts · 6 business functions · 
> 8+ industries · Every prompt ships with variables, 
> output formats, and performance benchmarks**

---

## What This Is

A production-ready AI prompt library built for enterprise 
business use — not generic templates. Every prompt in this 
library includes:

- **Input variables** — clearly defined, plug-and-play
- **Expected output format** — structured and consistent
- **Performance metrics** — measurable targets for each prompt
- **Iteration notes** — what to test and refine

Built as part of the AI Operator Certification capstone using 
the **CRAFT methodology** (Context, Role, Action, Format, Tone).

---

## Library Structure

| Category | Prompts | Industries |
|----------|---------|------------|
| [Customer Service & Support](./customer-service/) | 10 | Healthcare, Retail, Financial Services, Telecom |
| [Data Analysis & Reporting](./data-analytics/) | 10 | Finance, Healthcare, Retail, Operations |
| [Content Generation](./content-generation/) | 10 | All industries |
| [Process Automation](./process-automation/) | 8 | HR, Finance, Operations, Manufacturing |
| [Quality Assurance](./quality-assurance/) | 6 | Healthcare, Financial Services, Technology |
| [Training & Onboarding](./training-onboarding/) | 6 | All industries implementing AI |
| **Total** | **50** | **8+ industries** |

---

## Sample Prompt: Customer Inquiry Classifier

**ID:** CS-01  
**Category:** Customer Service & Support  
**Industries:** Healthcare · Retail · Financial Services · Telecom

**The Prompt:**
```
You are an expert customer service routing agent. 
Analyze the following customer inquiry and return 
a structured classification.

Customer Message: {{customer_message}}
Channel: {{channel}} (email/chat/voice transcript)
Customer Tier: {{customer_tier}} (standard/premium/enterprise)

Classify and return:
1. PRIMARY INTENT
2. URGENCY SCORE (1-5)
3. SENTIMENT
4. RECOMMENDED DEPARTMENT
5. SUGGESTED PRIORITY
6. INITIAL RESPONSE DRAFT
7. ESCALATION FLAG
```

**Performance Targets:**
- Routing accuracy >90%
- Classification time <3 seconds
- Escalation precision >85%

---

## Sample Prompt: Executive KPI Summary Generator

**ID:** DA-01  
**Category:** Data Analysis & Reporting  
**Industries:** Finance · Healthcare · Retail · Operations

**The Prompt:**
```
You are a senior data analyst preparing a briefing 
for the C-suite. Analyze the following KPI data and 
generate an executive summary written for a CEO 
with 90 seconds to read it.

KPI Data: {{kpi_data_json}}
Reporting Period: {{period}}
Business Unit: {{business_unit}}
Strategic Goals: {{strategic_goals}}

Deliver:
1. HEADLINE (1 sentence — most important insight)
2. PERFORMANCE SNAPSHOT (5 metrics: 🟢/🟡/🔴)
3. TOP WIN
4. TOP CONCERN
5. TREND ANALYSIS
6. RECOMMENDED ACTIONS (3, prioritized)
7. FORWARD OUTLOOK
```

**Performance Targets:**
- Executive satisfaction score >4/5
- Action item adoption rate tracked
- Time-to-brief reduction vs. manual

---

## How to Use This Library

1. Browse to the relevant category folder
2. Select a prompt by business use case
3. Replace all `{{variables}}` with your specific inputs
4. Test output against the performance metrics listed
5. Log iteration notes for your team

---

## Methodology: CRAFT

All prompts are designed using the CRAFT framework:

- **C**ontext — situation and background the AI needs
- **R**ole — expert perspective the AI should adopt
- **A**ction — the specific task to perform
- **F**ormat — how the output should be structured
- **T**one — voice and register of the response

---

## About the Author

Built by **Chrystelle Juste** — AI Enablement Strategist  
specializing in prompt engineering, workflow automation,  
and enterprise AI adoption.

[Portfolio](https://notion.so) · 
[LinkedIn](https://linkedin.com) · 
[Volunteer Wizard Project](../volunteer-wizard-ai-automation)
