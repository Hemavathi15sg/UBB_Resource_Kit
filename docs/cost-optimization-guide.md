# GitHub Copilot Cost Optimization Guide

## Prompt Compression & Language Tax

- Keep prompts concise and specific.
- Avoid repeating context or instructions.
- Use clear requirements instead of lengthy descriptions.

---

## Context Management & Escalation Ladder

- Start with the smallest relevant context.
- Escalate from file -> module -> repository only when needed.
- Avoid sending entire codebases for simple tasks.

---

## Output Control - Copilot Instructions

- Use Copilot Instructions to define response format and coding standards.
- Request summaries or focused outputs instead of lengthy explanations.
- Reduce unnecessary output tokens.

---

## Workflow Modes - Ask, Plan, Agent

- Ask -> Quick questions and code explanations
- Plan -> Design discussions and feature planning
- Agent -> Complex multi-step automation
- Use the simplest mode that can accomplish the task.

---

## Agent Configurations - Custom Agents, Skills, Subagents

- Create purpose-built Custom Agents.
- Use Skills and Subagents for reusable expertise.
- Reduce retries and improve consistency.

---

## Model Routing & Reasoning Budget

- Use lightweight models for documentation, refactoring, and code generation.
- Reserve premium reasoning models for debugging, architecture, and migrations.
- Match model capability to task complexity.

---

## MCP Tool Pruning

- Expose only the tools agents actually need.
- Remove unused MCP integrations.
- Reduce reasoning overhead and token consumption.

---

## Enterprise Guardrails & Budget Policy

- Configure Enterprise, Cost Center, and User budgets.
- Set alerts at 75%, 90%, and 100%.
- Review usage regularly and optimize before increasing budgets.

---

## Key Takeaway

Don't focus on using fewer AI credits. Focus on getting more value from every AI credit consumed.
