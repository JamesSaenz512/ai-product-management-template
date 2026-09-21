# Juno PM - AI Copilot for Rocketship's Product Organization

> Juno is RocketShip’s AI Associate Product Manager, embedded in Slack, Notion, and Jira, whose single job is to turn overwhelming product signals into prioritized, actionable work so human PMs can make better decisions faster.

_James Saenz · AI PM Cohort · September 2026_

Repo: https://github.com/JamesSaenz512/ai-product-management-template

This repo is my final project for the AI Product Management Certification — **Juno PM - AI Copilot for Rocketship's Product Organization**. Each module’s artefact lives in its own folder; this README is the dashboard and the pitch.

---

## Module artefacts

### M1 · Prompting
- **System prompt** — [`01-prompting/system-prompt.md`](01-prompting/system-prompt.md)
- **Prototype** — https://juno-pm-dashboard--jbsaenz512.replit.app/

### M2 · Strategy
- **Decision matrix** — [`02-strategy/decision-matrix.md`](02-strategy/decision-matrix.md)
- **AI Strategy one-pager** — [`02-strategy/strategy-one-pager.md`](02-strategy/strategy-one-pager.md)

### M3 · RAG / AI PRD
- **AI PRD** — [`03-rag-prd/prd.md`](03-rag-prd/prd.md)

### M4 · AI-Native UX
- **AI user flow** — [`04-ai-ux/user-flow.md`](04-ai-ux/user-flow.md)
- **Trust-gap mitigations** — [`04-ai-ux/trust-gaps.md`](04-ai-ux/trust-gaps.md)

### M5 · Agentic Workflows
- **Agent Workflow Spec (AWSpec)** — [`05-agentic-workflows/awspec.md`](05-agentic-workflows/awspec.md)
- **Agent Control Panel** — [`05-agentic-workflows/agent-control-panel.md`](05-agentic-workflows/agent-control-panel.md)

### M6 · Evals &amp; Guardrails
- **Eval stack** — [`06-evals/eval-stack.md`](06-evals/eval-stack.md)
- **Human evaluation rubric** — [`06-evals/human-rubric.md`](06-evals/human-rubric.md)

---

## PM Execution Plan

### Where Juno is today
- Juno is fully designed across the six course modules. 
- The prompt, strategy, harness, UX, agent workflow, human rubric, and eval stack are all defined. 
- The product is still at the prototype/spec stage, so the next step is turning those decisions into a working, testable system.

### What ships next (next 2 sprints)
- Sprint 1: Build out the working Juno flow using the Slack, Jira, support, and strategy connections we already defined. Add the permissions, handoff rules, verification checks, and eval logging from the harness and AWSpec.
- Sprint 2: Run Juno on real or realistic P0 triage cases with a PM in the loop. Start collecting user feedback, human rubric scores, and automated eval results, then use those results to tighten the model, data, or architecture before expanding use.

### What I watch (dashboards)
- Daily: positive/negative feedback, edits or overrides, abandoned recommendations, handoffs, and response time.
- Weekly: human rubric average, citation problems, safety/refusal issues, and repeated user complaints.
- Per release: golden-set accuracy, citation pass rate, safety pass rate, and whether any hard gate failed.

### Red lines (what blocks shipping)
- Any PII leak blocks the release.
- Any serious safety or refusal failure blocks the release.
- Any missing, fabricated, or wrong citation blocks the release.
- Golden-set accuracy below 90% blocks the release.

### Governance
- Compliance: Keep sensitive or regulated information inside approved systems and escalate anything that needs legal or policy review.
- Safety: Protect PII, block unsafe behavior, and hand risky decisions back to a person.
- Reliability: Juno should fail clearly when a source or tool is unavailable instead of guessing, and it should stay within the accuracy and citation bars we set.
- Reputation: Juno should never make up risks, customer details, or evidence. If the answer is uncertain, it should say so instead of sounding more confident than the evidence supports.

---

## Build Insights

- **Friction point.** Keeping all the pieces consistent as Juno got more detailed was harder than I expected. A decision about tools, memory, confidence, or human handoff in one module could affect several other parts of the product.
- **Key learning.** AI needs a much more complete product spec than a normal feature. It is not enough to say what Juno should do; I also have to define what it can see, what it can change, when it stops, when a human takes over, and how I will know if it is doing a good job.
- **Aha moment.** The biggest aha for me was that the model is only one part of the product. Most of the trust in Juno comes from the rules around it — the data it uses, the tools it can access, the guardrails, human checkpoints, and the evals that prove it is working.

---

_Certification submission — AI Product Management Certification._
