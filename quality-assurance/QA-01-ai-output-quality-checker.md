# QA-01 · AI Output Quality Checker

![Category](https://img.shields.io/badge/Category-Quality%20Assurance-rose?style=flat)
![Industry](https://img.shields.io/badge/Industries-All-c9943a?style=flat)
![Method](https://img.shields.io/badge/Method-MASTER-22c55e?style=flat)

## Purpose
Evaluate AI-generated content for accuracy, 
tone, completeness, and enterprise readiness 
before it reaches a human audience.
Catches errors, bias, and off-brand language 
before they cause damage.

---

## Industries
Healthcare · Financial Services · 
Technology · All regulated industries

---

## Input Variables
| Variable | Description |
|----------|-------------|
| {{ai_output}} | The AI generated content to review |
| {{intended_audience}} | Who will receive this content |
| {{brand_voice}} | formal / warm / technical / casual |
| {{content_type}} | email / report / training / announcement |
| {{compliance_requirements}} | Any regulatory requirements |

---

## The Prompt
```
You are a senior quality assurance specialist 
with expertise in AI content review and 
enterprise communications standards.

Review the following AI-generated content and 
return a complete quality assessment.

AI Output: {{ai_output}}
Intended Audience: {{intended_audience}}
Brand Voice: {{brand_voice}}
Content Type: {{content_type}}
Compliance Requirements: {{compliance_requirements}}

Return your assessment in this exact format:

OVERALL QUALITY SCORE: [1-10]

ACCURACY CHECK:
- Factual claims verified: [yes/no/partial]
- Unsupported statements: [list or none]
- Recommended corrections: [list or none]

TONE ASSESSMENT:
- Matches brand voice: [yes/no/partial]
- Tone issues found: [list or none]
- Recommended adjustments: [list or none]

COMPLETENESS CHECK:
- All required elements present: [yes/no]
- Missing elements: [list or none]

BIAS AND SENSITIVITY CHECK:
- Potential bias detected: [yes/no]
- Sensitivity concerns: [list or none]

COMPLIANCE CHECK:
- Meets requirements: [yes/no/review needed]
- Flags: [list or none]

FINAL RECOMMENDATION:
[approve / revise / reject with reason]

REVISED VERSION: [if revision needed, 
provide corrected content here]
```

---

## Performance Targets
- Quality score accuracy vs human reviewer >85%
- False positive rate for bias detection <10%
- Compliance flag accuracy >95%
- Review time reduction vs manual >70%

---

## Iteration Notes
- Healthcare: always flag patient safety language
- Financial: flag any specific return or 
  performance claims
- Legal review required for score below 6
- Run twice for regulated industry content
- Add company style guide as context for 
  better tone matching

---

## Example Output
```
OVERALL QUALITY SCORE: 7/10

ACCURACY CHECK:
- Factual claims verified: partial
- Unsupported statements: 
  "AI will save your team 50% of their time" 
  — no supporting data provided
- Recommended corrections: 
  Replace with documented metric or remove claim

TONE ASSESSMENT:
- Matches brand voice: partial
- Tone issues found: 
  Opening paragraph too technical for 
  non-technical audience
- Recommended adjustments: 
  Replace "implement AI workflows" with 
  "start using AI in your daily work"

COMPLETENESS CHECK:
- All required elements present: no
- Missing elements: 
  Call to action and contact information absent

BIAS AND SENSITIVITY CHECK:
- Potential bias detected: no
- Sensitivity concerns: none

COMPLIANCE CHECK:
- Meets requirements: review needed
- Flags: performance claim requires 
  legal review before distribution

FINAL RECOMMENDATION: revise
Primary issues: unsupported time savings claim 
and missing call to action
```

---

*Built by Chrystelle Juste · AI Enablement Strategist*
*[Portfolio](https://notion.so) · 
[LinkedIn](https://linkedin.com)*
