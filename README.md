# Ujima AI Pride

## Overview

Ujima AI Pride is a multi-agent loan support ecosystem designed for SACCOs serving smallholder farmers in Uganda and Rwanda.

The system follows the Agent Savannah frameworks:

- RANK
- TRAIL
- HUNT
- GUARD
- CYCLE

The workflow assists loan officers by:

1. Educating members through financial literacy messages.
2. Screening loan applications.
3. Escalating higher-risk cases to human officers.
4. Maintaining ethical oversight and human sovereignty.

---

## Agent Architecture

### Scout Agent

Role:
Financial Literacy Coach

Authority:
Maximum 3 SMS per day.

Cannot recommend specific loans.

Notification Trigger:
Escalates when users mention:

- Loan sharks
- Debt collectors
- Emergency borrowing

Kill Switch:
\*#700#

---

### Guardian Agent

Role:
Loan Triage Agent

Authority:
Can approve loans up to KES 15,000.

Cannot deny applications without 3 risk flags.

Kill Switch:
\*#733#

---

### Hunter Agent

Role:
Human-in-the-Loop Coordinator

Authority:
Never approves loans.

Only prepares officer briefing packs.

Kill Switch:
\*#799#

---

## HUNT Workflow

1. Farmer submits request.
2. Scout detects financial stress.
3. Guardian evaluates application.
4. Cases above threshold are sent to Hunter.
5. Human officer makes final decision.

---

## Data Sovereignty

All data remains within African governance requirements.

Storage region:

AWS Africa (Cape Town)

Compliance:

- Uganda Data Protection and Privacy Act
- Rwanda Data Protection and Privacy Law

---

## Safety Controls

### GUARD Framework

Guardrails:
No gender proxies.

Unusual Pattern Detection:
Flag approval drops above 30%.

Audit Trail:
All decisions logged.

Red Team:
Bias testing performed.

Dignity:
No harmful denial language.

---

## Self Improvement

### CYCLE

Capture:
CSAT

Yield:
Weekly insights

Course Correct:
Human-approved updates

Loop Validation:
Required

Explain:
Plain language reports

---
