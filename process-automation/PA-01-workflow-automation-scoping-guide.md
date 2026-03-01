# PA-01 · Workflow Automation Scoping Guide

![Category](https://img.shields.io/badge/Category-Process%20Automation-c9943a?style=flat)
![Industry](https://img.shields.io/badge/Industries-All-6366F1?style=flat)
![Method](https://img.shields.io/badge/Method-MASTER-22c55e?style=flat)

## Purpose
Identify, evaluate, and prioritize business processes 
ready for AI automation — before building anything.
Turns vague automation requests into clear, 
scoped, actionable project briefs.

---

## Industries
HR · Finance · Operations · Healthcare · 
Manufacturing · Professional Services

---

## Input Variables
| Variable | Description |
|----------|-------------|
| {{process_name}} | Name of the process to evaluate |
| {{department}} | Department that owns the process |
| {{frequency}} | How often the process runs |
| {{time_per_run}} | How long it takes each time |
| {{people_involved}} | Number of people required |
| {{pain_points}} | What is most frustrating about it |

---

## The Prompt
```
You are a senior AI automation consultant with 
expertise in workflow design and process optimization.

Evaluate the following business process for 
AI automation readiness and return a complete 
scoping brief.

Process Name: {{process_name}}
Department: {{department}}
Frequency: {{frequency}}
Time Per Run: {{time_per_run}}
People Involved: {{people_involved}}
Pain Points: {{pain_points}}

Return your evaluation in this exact format:

AUTOMATION READINESS SCORE: [1-10 with reason]

CURRENT STATE SUMMARY:
[2-3 sentences describing the process as it exists]

TIME IMPACT ANALYSIS:
- Weekly time cost: [hours]
- Annual time cost: [hours]
- Estimated automation savings: [percentage]

TOP 3 AUTOMATION OPPORTUNITIES:
1. [Specific step that can be automated]
2. [Specific step that can be automated]
3. [Specific step that can be automated]

RECOMMENDED TOOLS:
- [Tool 1]: [specific use in this process]
- [Tool 2]: [specific use in this process]

IMPLEMENTATION PRIORITY: [high/medium/low]
ESTIMATED BUILD TIME: [hours/days]
RISKS TO CONSIDER: [2-3 bullet points]

FIRST STEP: [exactly what to do this week]
```

---

## Performance Targets
- Scoping accuracy vs actual build outcome >85%
- Time estimate variance <20%
- Stakeholder brief approval rate >90%
- Automation readiness score correlation with success

---

## Iteration Notes
- Always calculate annual time cost — small daily 
  tasks become compelling when annualized
- Score below 5 — recommend process redesign first
- Score above 8 — fast track to build phase
- Include data privacy check for healthcare processes
- Flag any process involving PII for security review

---

## Example Output
```
AUTOMATION READINESS SCORE: 9/10
High repetition, rule-based logic, 
clear inputs and outputs — ideal for automation.

CURRENT STATE SUMMARY:
The volunteer qualification process requires a 
coordinator to manually review each application, 
verify credentials, classify applicant type, 
and send a confirmation email. The process runs 
40-60 times per month with no standardization.

TIME IMPACT ANALYSIS:
- Weekly time cost: 10 hours
- Annual time cost: 520 hours
- Estimated automation savings: 96%

TOP 3 AUTOMATION OPPORTUNITIES:
1. AI classification of applicant type on submission
2. Automated credential verification via Perplexity AI
3. Personalized confirmation email by applicant path

RECOMMENDED TOOLS:
- Zapier Pro: workflow orchestration and routing
- AI by Zapier: applicant classification
- Perplexity AI: credential verification

IMPLEMENTATION PRIORITY: high
ESTIMATED BUILD TIME: 3-5 days
RISKS TO CONSIDER:
- Edge cases requiring human review
- Data privacy for applicant credentials
- Coordinator training on exception handling

FIRST STEP: Map all 4 qualification paths 
on paper before opening Zapier
```

---

*Built by Chrystelle Juste · AI Enablement Strategist*
*[Portfolio](https://notion.so) · 
[LinkedIn](https://linkedin.com)*
