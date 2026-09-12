# AI Strategy One-Pager - Juno Automated Prioritization

## 1. Problem & Workflow

Juno prevents PMs from making reactive prioritization decisions based on stakeholder pressure rather than a complete view of urgency, customer impact, and risk. The squeakiest wheel gets the grease.

## 2. Target Metrics

- Time to Prioritization: Average time from a P0 escalation being raised to a PM approving its priority. This measures whether Juno is unblocking decisions.

- PM override: How often PMs reject or substantially change Juno’s recommended priority. You want speed without bad recommendations.

Time to Prioritization Decision

## 3. Autonomy Level

Copilot. Juno performs the analysis and recommends actions, but the PMs retain approval authority. I would not choose Agent because prioritization decisions can affect customer commitments, roadmap direction, and engineering priorities, making full autonomy risky to implement.

## 4. Data & Model Approach

Buy + Ground. We will use an existing LLM and ground it with RocketShip data through RAG. We are not taking the shortcut of fine-tuning a model and treating static training as a substitute for access to current operational signals.

## 5. Risks & Mitigations

Risk: Juno making a bad prioritization call that changes a customer commitment or engineering priority before a human catches it. Once teams act on that decision, the damage can be hard to unwind and trust in Juno drops fast.

Mitigation: Juno can recommend and draft, but it cannot change roadmap priorities, customer commitments, or engineering work without explicit PM approval.

## 6. V1 Scope

- Juno will not make final roadmap or prioritization decisions. It can recommend what should come first, but a PM has to approve the decision.

- Juno will not make or change customer commitments. It cannot promise dates, scope, or delivery outcomes to customers or Sales on its own.
