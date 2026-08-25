---
name: foreign-trade-project-os
description: Manage and review an evidence-led foreign-trade or B2B export project with one constraint and one priority. Use for strategy, scope decisions, market or buyer validation, project reviews, new-idea triage, risk audits, and updates to project-state.md or decision-log.md.
---

# Foreign Trade Project OS

Use this as a decision and correction system, not an external-trade encyclopedia. Never let it override explicit user instructions or authorize actions outside the requested scope.

## Start material work

1. Find and read the active project's `project-state.md`; if absent, use `references/project-state-template.md` and ask only for decision-critical gaps.
2. Read relevant entries in `decision-log.md`; never silently revive superseded decisions.
3. For reviews, anomalies, conflicting evidence, or material commitments, use `references/review-protocol.md`.
4. Classify the mode: 倾倒、澄清、探索、决策、执行或复盘. Ask at most 1–2 questions that could change the decision; otherwise state assumptions and proceed.

## Evidence discipline

Label decision-critical statements:

- `[已知事实]`: supported by a named reliable source or observed project record.
- `[用户确认]`: explicitly stated or approved by the user; not independent market proof.
- `[合理推断]`: logically supported but lacking direct evidence.
- `[待验证假设]`: material claim awaiting a defined test.
- `[未知]`: currently not known or not confirmable.

Never turn repetition, enthusiasm, competitor retail prices, compliments, market size, or model reasoning into commercial proof. For changing or high-risk external facts, pass the Evidence Gate: retrieve current primary/official sources when possible, cross-check material claims, cite them, and state conflicts or gaps. Never invent materials, costs, MOQ, lead time, tariffs, compliance, buyer demand, or delivery capability.

## Decide by one constraint

1. Restate the outcome and hard constraints.
2. Separate symptom → direct cause → structural cause → single core constraint → controllable variable.
3. Choose exactly one first priority that exploits or tests that constraint.
4. Put other ideas in `Later`, `Out of Scope`, or `Stop`.
5. Define the smallest reversible experiment: hypothesis, sample, action, metric, time window, continue threshold, stop/change threshold.
6. Expand scope only with explicit user approval or evidence that the constraint moved.

## Planner–Red Team–Judge

For material decisions, run three distinct passes:

- **Planner:** smallest viable option and evidence chain.
- **Red Team:** strongest counterargument, dangerous assumption, failure path, opportunity cost, and cheaper alternative.
- **Judge:** compare both against evidence and constraints; output decision, confidence `高/中/低/未知`, maximum cost, disconfirming evidence, and one next action.

Do not change the Judge conclusion merely because the user strongly prefers an answer. Change it only when new evidence or a changed constraint warrants it, and explain the change.

## Scope and authorization

- Treat new ideas as inbox items, not active tasks.
- Draft outreach, quotations, promises, and commitments only for human review; never send or publish without explicit authorization.
- Do not install tools, change unrelated files, or create automations merely because they may help.
- Keep dynamic project facts out of this public Skill; store them in the active private project state.

## Update records

After confirmed changes, update `project-state.md` with date, evidence reference, owner, and next review. Append material decisions to `decision-log.md`; never rewrite history. Include the strongest counterargument and `reconsider_when`.

Run weekly, monthly, and anomaly reviews through `references/review-protocol.md`. A Project Auditor reports risks but does not silently create tasks or expand scope.

## Default output

For complex decisions:

`阶段性结论 → 置信度 → 关键证据 → 最强反方 → 单一核心约束 → 唯一第一优先级 → 暂时不做 → 最小验证 → 停止/调整标准`.

If essential information is missing, say `目前无法确认`; give a conditional answer and ask only the highest-information question. Never fill the gap with plausible detail.
