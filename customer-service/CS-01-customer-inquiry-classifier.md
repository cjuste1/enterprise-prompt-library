# CS-01 · Customer Inquiry Classifier

![Category](https://img.shields.io/badge/Category-Customer%20Service-c9943a?style=flat)
![Industry](https://img.shields.io/badge/Industries-4-6366F1?style=flat)
![Method](https://img.shields.io/badge/Method-MASTER-22c55e?style=flat)

## Purpose
Automatically classify inbound customer inquiries 
by type, urgency, and department to enable fast 
routing and consistent handling.

---

## Industries
Healthcare · Retail · Financial Services · Telecom

---

## Input Variables
| Variable | Description |
|----------|-------------|
| {{customer_message}} | The full customer inquiry text |
| {{channel}} | email / chat / voice transcript |
| {{customer_tier}} | standard / premium / enterprise |

---

## The Prompt
```
You are an expert customer service routing agent 
with 10 years of experience in enterprise support operations.

Analyze the following customer inquiry and return 
a structured classification.

Customer Message: {{customer_message}}
Channel: {{channel}}
Customer Tier: {{customer_tier}}

Return your analysis in this exact format:

PRIMARY INTENT: [one sentence]
URGENCY SCORE: [1-5 with brief reason]
SENTIMENT: [positive/neutral/frustrated/angry]
RECOMMENDED DEPARTMENT: [department name]
SUGGESTED PRIORITY: [low/medium/high/critical]
ESCALATION FLAG: [yes/no with reason]
DRAFT RESPONSE: [2-3 sentence response ready to send]
```

---

## Performance Targets
- Routing accuracy >90%
- Classification time <3 seconds
- Escalation precision >85%
- Draft response usability >80%

---

## Iteration Notes
- Add customer history context for higher accuracy
- Test with edge cases — angry tone with simple request
- Adjust urgency scoring for industry-specific thresholds
- Healthcare: flag any mention of patient safety immediately

---

## Example Output
```
PRIMARY INTENT: Customer requesting refund for 
damaged product received last week
URGENCY SCORE: 3 — financial impact, not safety related
SENTIMENT: frustrated
RECOMMENDED DEPARTMENT: Returns and Refunds
SUGGESTED PRIORITY: medium
ESCALATION FLAG: no — standard return request
DRAFT RESPONSE: Thank you for reaching out about 
your recent order. I completely understand your 
frustration and want to make this right immediately. 
I am connecting you with our Returns team who will 
process your refund within 24 hours.
```

---

*Built by Chrystelle Juste · AI Enablement Strategist*
*[Portfolio](https://notion.so) · 
[LinkedIn](https://linkedin.com)*
