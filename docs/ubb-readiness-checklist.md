# UBB Readiness Checklist

## Executive Summary

This checklist helps organizations validate operational readiness for GitHub Copilot Usage-Based Billing (UBB). It provides a structured path across strategy, governance, monitoring, and adoption so teams can move to go-live with confidence.

> **Important**
> Use this checklist as a decision framework, not a one-time activity. Reassess monthly during the first quarter after rollout.

---

## Readiness Categories

| Category | Purpose | Suggested Owner |
| --- | --- | --- |
| Understanding UBB | Build foundational understanding of AI credit consumption. | Platform Lead |
| Assessing Current Usage | Baseline current behavior and identify high-impact users. | Engineering Operations |
| Governance Setup | Implement enterprise, cost center, and user guardrails. | Copilot Administrator |
| Monitoring & Reporting | Establish visibility, trend tracking, and operating metrics. | FinOps / Platform |
| Developer Enablement | Improve usage quality through education and standards. | Enablement Lead |
| Go-Live Readiness | Confirm controls, communications, and escalation paths. | Program Owner |

---

## 1. Understanding UBB

- [ ] Review GitHub's transition from PRUs to AI Credits.
- [ ] Understand token-based consumption (input, output, cached tokens).
- [ ] Identify which Copilot features consume AI Credits.
- [ ] Document model-specific pricing differences and approved usage patterns.
- [ ] Publish a short internal UBB primer for stakeholders.

> **Best Practice**
> Standardize UBB terminology early so finance, engineering, and platform teams use the same language.

---

## 2. Assessing Current Usage

- [ ] Identify high-usage teams and users.
- [ ] Review Copilot adoption levels across business units.
- [ ] Analyze usage patterns for Chat, Agents, Code Review, and CLI.
- [ ] Flag power users and investigate usage intent.
- [ ] Capture a 30-day baseline for spend, usage volume, and productivity outcomes.

---

## 3. Governance Setup

- [ ] Define enterprise-level additional spend budget.
- [ ] Create cost center or organization budgets.
- [ ] Configure user-level budget policies.
- [ ] Set alert thresholds at 75%, 90%, and 100%.
- [ ] Document exception and escalation workflows.

> **Important**
> Governance is incomplete unless ownership, escalation paths, and approval authorities are documented.

---

## 4. Monitoring & Reporting

- [ ] Enable usage monitoring dashboards.
- [ ] Define a standard monthly usage report format.
- [ ] Track heavy consumers and month-over-month trends.
- [ ] Run a recurring monthly governance review.
- [ ] Track optimization actions and resulting impact.

---

## 5. Developer Enablement

- [ ] Educate teams on AI Credits and token drivers.
- [ ] Train users on model selection and workflow modes.
- [ ] Share prompt engineering best practices.
- [ ] Publish internal Copilot usage guidelines.
- [ ] Provide role-based examples for engineers, architects, and platform teams.

> **Key Takeaway**
> Education is one of the highest-leverage controls for reducing avoidable credit consumption.

---

## 6. Go-Live Readiness

- [ ] Validate budget configurations in production scope.
- [ ] Review and approve governance policies.
- [ ] Confirm escalation process for budget increases.
- [ ] Communicate operational guidance to all stakeholders.
- [ ] Define first-90-days success metrics.

---

## Final Readiness Score

Use the following scoring method to determine go-live posture:

- Each completed item = 1 point.
- Total items = 30 points.
- Readiness % = (completed points / 30) x 100.

| Readiness Score | Status | Recommended Action |
| --- | --- | --- |
| 90% to 100% | Ready | Proceed with controlled go-live and monthly reviews. |
| 70% to 89% | Conditionally Ready | Go-live for pilot groups only; close critical gaps first. |
| Below 70% | Not Ready | Delay rollout; prioritize governance and monitoring foundations. |

<details>
<summary>Scoring worksheet template</summary>

| Category | Completed Items | Total Items | Notes |
| --- | --- | --- | --- |
| Understanding UBB |  | 5 |  |
| Assessing Current Usage |  | 5 |  |
| Governance Setup |  | 5 |  |
| Monitoring & Reporting |  | 5 |  |
| Developer Enablement |  | 5 |  |
| Go-Live Readiness |  | 5 |  |
| Total |  | 30 |  |

</details>
