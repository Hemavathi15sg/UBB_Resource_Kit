# Cost Optimization Guide

## Executive Summary

This guide outlines practical levers to optimize GitHub Copilot UBB consumption without reducing developer effectiveness. Each section includes why the control matters, how to implement it, and expected business impact.

> **Key Takeaway**
> Optimize for value per AI credit, not minimum AI usage.

---

## 1. Prompt Compression & Language Tax

### Why it matters
Verbose prompts increase token usage and can introduce ambiguity that leads to retries.

### Best practices
- Use concise, outcome-focused prompts.
- Remove repeated context and duplicate instructions.
- Prefer explicit acceptance criteria over long narrative descriptions.

### Optimization tips
- Use structured prompt templates for recurring tasks.
- Add constraints first (scope, format, expected output).
- Keep context narrowly tied to the immediate objective.

### Expected impact
| Metric | Typical Improvement |
| --- | --- |
| Input token volume | Reduced by 15% to 30% |
| Retry rate | Reduced by 10% to 20% |
| Response relevance | Improved due to clearer intent |

---

## 2. Context Management & Escalation Ladder

### Why it matters
Oversharing context increases token load and slows responses.

### Best practices
- Start with file-level context.
- Escalate only when needed: file -> module -> repository.
- Avoid sharing entire codebases for localized changes.

### Optimization tips
- Pre-select only relevant files before asking complex tasks.
- Summarize unchanged background instead of pasting large blocks.
- Use checklist-based escalation criteria for support teams.

### Expected impact
| Metric | Typical Improvement |
| --- | --- |
| Average tokens per request | Reduced by 20% to 40% |
| Time to usable answer | Improved by 10% to 25% |
| Cost predictability | Increased through consistent scoping |

---

## 3. Output Control using Copilot Instructions

### Why it matters
Unbounded output increases token consumption and review effort.

### Best practices
- Define response format and coding standards in Copilot Instructions.
- Request summaries, diffs, or scoped outputs where appropriate.
- Require concise answers unless deep analysis is explicitly needed.

### Optimization tips
- Standardize output patterns for design, coding, and review tasks.
- Ask for tables or checklists when decision tracking is needed.
- Use explicit word or section limits for recurring workflows.

### Expected impact
| Metric | Typical Improvement |
| --- | --- |
| Output token usage | Reduced by 15% to 35% |
| Review effort | Reduced due to consistent structure |
| Team consistency | Increased across contributors |

---

## 4. Workflow Modes (Ask -> Plan -> Agent)

### Why it matters
Using an advanced workflow mode for simple tasks can increase processing overhead.

### Best practices
- Use Ask for direct questions and explanations.
- Use Plan for architecture and scoped design work.
- Use Agent for multi-step automation requiring tools and execution.

### Optimization tips
- Publish a mode selection matrix for teams.
- Train users to downgrade mode when the task scope is small.
- Require Plan mode before large implementation changes.

### Expected impact
| Metric | Typical Improvement |
| --- | --- |
| Unnecessary agent runs | Reduced by 20% to 50% |
| Completion speed on simple tasks | Improved |
| Cost-to-value ratio | Improved through mode discipline |

---

## 5. Agent Configurations (Custom Agents, Skills, Subagents)

### Why it matters
General-purpose agents can create inconsistent behavior and retries.

### Best practices
- Create purpose-built custom agents for high-frequency scenarios.
- Use reusable skills for standard patterns.
- Route specialized tasks to focused subagents.

### Optimization tips
- Track top recurring prompts and build targeted agents.
- Keep agent instructions concise and testable.
- Audit retry causes monthly and tune agent definitions.

### Expected impact
| Metric | Typical Improvement |
| --- | --- |
| Retry volume | Reduced by 15% to 30% |
| First-pass quality | Increased |
| Operational consistency | Increased across teams |

---

## 6. Model Routing & Reasoning Budget

### Why it matters
Model choice has a direct effect on credit consumption and response quality.

### Best practices
- Use lightweight models for routine tasks (documentation, refactoring, scaffolding).
- Reserve premium reasoning models for complex debugging and architecture.
- Define approved model-task mappings by role and workload.

### Optimization tips
- Implement a model routing guide in internal standards.
- Track high-cost workloads and verify model-task fit.
- Set exceptions that require justification for premium models.

### Expected impact
| Metric | Typical Improvement |
| --- | --- |
| Average cost per task | Reduced by 10% to 35% |
| Quality on complex tasks | Maintained or improved |
| Budget predictability | Improved through controlled routing |

---

## 7. MCP Tool Pruning

### Why it matters
Excess tool availability can increase reasoning complexity and unnecessary tool calls.

### Best practices
- Expose only tools needed for each workflow.
- Remove stale or duplicate MCP integrations.
- Separate tool profiles by team or use case.

### Optimization tips
- Perform a quarterly tool inventory.
- Measure tool invocation frequency and remove unused tools.
- Limit powerful tools to trusted scenarios with clear guardrails.

### Expected impact
| Metric | Typical Improvement |
| --- | --- |
| Tool-call overhead | Reduced |
| Agent latency | Improved |
| Governance control | Increased |

---

## 8. Enterprise Guardrails & Budget Policies

### Why it matters
Without policy controls, spend variance can escalate quickly during adoption.

### Best practices
- Configure budget hierarchy: enterprise -> cost center -> user.
- Set thresholds and alerts at 75%, 90%, and 100%.
- Review usage trends before approving budget increases.

### Optimization tips
- Define pre-approved actions per threshold breach.
- Use role-based policy tiers for higher-value technical roles.
- Link budget requests to measurable productivity outcomes.

### Expected impact
| Metric | Typical Improvement |
| --- | --- |
| Spend variance | Reduced |
| Forecast accuracy | Improved |
| Governance maturity | Increased |

> **Best Practice**
> Combine budget policies with enablement programs to avoid productivity disruption.

---

## Optimization Scorecard

<details>
<summary>Monthly optimization review checklist</summary>

- [ ] Prompt standards documented and adopted.
- [ ] Escalation ladder applied in team workflows.
- [ ] Copilot Instructions standardized across repositories.
- [ ] Mode selection guidance published and followed.
- [ ] Custom agents/skills reviewed for performance.
- [ ] Model routing policy in place and monitored.
- [ ] MCP tool inventory reviewed and pruned.
- [ ] Budget guardrails validated and alert actions tested.

</details>
