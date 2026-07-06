# Job Evaluation Framework

## Scoring Dimensions

Evaluate each job posting against these five dimensions:

### 1. Technical Skills Match (0-100)
How well do the required or preferred skills align with Pushpak's capabilities?

| Score | Meaning |
|-------|---------|
| 80-100 | Core requirements focus on reconciliations, internal controls, documentation, data quality, accounting systems, or entry-level IT audit with training. |
| 60-79 | Most requirements match, with 1-2 learnable gaps such as formal audit testing methodology or a specific GRC tool. |
| 40-59 | Partial match, significant upskilling needed, such as cybersecurity frameworks or advanced analytics. |
| 0-39 | Fundamental mismatch, such as senior software engineering, senior cybersecurity, or unrelated sales roles. |

**Strong match areas:** reconciliations, variance analysis, documentation review, approval and authorization checks, audit-ready records, audit trails, Excel analysis, data validation, enterprise systems, stakeholder follow-up.
**Moderate match areas:** IT audit associate, technology risk associate, SOX or controls testing, data governance, accounting systems analysis, internal audit support.
**Weak match areas:** senior IT audit management, direct cybersecurity engineering, penetration testing, advanced production software development, senior CPA roles requiring completed designation.

### 2. Experience Match (0-100)
Does work history align with what they are looking for?

| Score | Meaning |
|-------|---------|
| 80-100 | Entry-level or associate role where accounting, systems, controls, data validation, and audit readiness are directly relevant. |
| 60-79 | Related role where transferable controls and data skills are clear but direct IT audit experience is not required. |
| 40-59 | Adjacent role that would require a strong transition narrative and quick upskilling. |
| 0-39 | Role requires senior direct experience or unrelated background. |

**Strong:** dealership accounting controls, transaction verification, reconciliations, internal control checkpoints, enterprise data validation, IBM Maximo asset records, Excel reporting.
**Moderate:** IT audit associate, internal controls analyst, data governance analyst, accounting systems analyst, audit and assurance associate with technology exposure.
**Entry-level:** formal IT general controls testing, GRC platforms, SOX control testing, cybersecurity frameworks, ERP audit tools.

### 3. Behavioral/Culture Fit (0-100)
Does the role and company culture match the behavioral profile?

| Score | Meaning |
|-------|---------|
| 80-100 | Culture values accuracy, process discipline, documentation, clear standards, mentorship, and stakeholder collaboration. |
| 60-79 | Mixed signals but mostly compatible. |
| 40-59 | Some friction, such as highly ambiguous work or little onboarding into audit methods. |
| 0-39 | Significant mismatch, such as quota-heavy sales or chaotic environments with weak controls. |

**Red flags to research:** unclear role expectations, no training for entry-level audit methods, heavy travel, senior-only team, poor reviews around mentorship, or roles that are titled audit but are mainly sales or support.

### 4. Location & Logistics (Pass/Fail + Notes)
- Mississauga, Brampton, Toronto, Oakville, and broader GTA: PASS
- Hybrid in the GTA: PASS
- Remote Canada: PASS
- Requires relocation outside the GTA: FAIL unless Pushpak explicitly approves
- Frequent travel: FLAG and discuss with Pushpak

### 5. Career Alignment & Motivation (0-100)
Does this role advance Pushpak's transition into IT audit, controls, data governance, or accounting systems?

| Score | Meaning |
|-------|---------|
| 80-100 | Strongly aligned with IT audit, technology risk, controls, data governance, or accounting systems. |
| 60-79 | Good role that builds relevant controls, systems, or data quality experience. |
| 40-59 | Decent job but only indirectly supports the long-term goal. |
| 0-39 | Dead end or backwards step away from audit, systems, or data controls. |

**Career goals:**
- Transition into IT audit or technology risk.
- Build on accounting and computer science education through controls, systems, and data integrity work.
- Progress toward CPA designation while developing audit, assurance, and risk experience.

**Motivation filter:** Evaluate not just whether Pushpak can do the tasks, but whether the tasks build toward IT audit.
- Tasks that energize: reconciliations, controls review, data validation, system records, audit trails, variance investigation, stakeholder coordination, process standardization.
- Tasks that drain: unrelated sales, generic customer service, repetitive data entry with no controls or audit pathway, roles requiring senior experience without training.
- Non-task factors: mentorship, structured onboarding, hybrid flexibility, GTA location, exposure to audit or risk methodology.

### 6. Salary Benchmark (Optional)

If the salary lookup tool is configured (`salary_data.json` exists), look up the company:
```
python salary_lookup.py "<Company Name>" --json
```

If a city is known from the posting, add `--city "<City>"` to narrow results.

If the salary tool is not configured, skip this section.

## Output Format

Present the evaluation as:

```
## Job Fit Evaluation: [Role] at [Company]

| Dimension | Score | Notes |
|-----------|-------|-------|
| Technical Skills | XX/100 | [brief note] |
| Experience Match | XX/100 | [brief note] |
| Behavioral Fit | XX/100 | [brief note] |
| Location | PASS/FAIL | [brief note] |
| Career Alignment | XX/100 | [brief note] |

**Overall Score: XX/100** (weighted average of scored dimensions)

### Verdict: [Strong Fit / Good Fit / Moderate Fit / Weak Fit / Poor Fit]

### Key Strengths for This Role
- [bullet points]

### Gaps to Address
- [bullet points]

### Recommendation
[1-2 sentences: apply/skip/apply with caveats]
```

## Weighting
- Technical Skills: 30%
- Experience Match: 25%
- Behavioral Fit: 15%
- Career Alignment: 30%

(Location is pass/fail, not weighted.)

## Thresholds
- **Strong Fit** (75+): Definitely apply, tailor everything
- **Good Fit** (60-74): Apply, address gaps in cover letter
- **Moderate Fit** (45-59): Consider carefully, discuss with Pushpak
- **Weak Fit** (30-44): Probably skip unless strategic reasons
- **Poor Fit** (<30): Skip
