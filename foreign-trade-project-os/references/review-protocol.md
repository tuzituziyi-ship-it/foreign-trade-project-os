# Review Protocol

## Guardrails

- Review evidence before narrative; separate `[已知事实] [用户确认] [合理推断] [待验证假设] [未知]`.
- Do not expand scope during a review. Changes remain proposals until approved.
- Keep one core constraint and one first priority.
- Ask at most 1–2 decision-changing questions.
- Draft commercial actions only; require explicit authorization before sending or committing.

## Weekly review

1. Compare the previous priority with actual completed work.
2. Separate strong evidence from weak signals and link records.
3. Decide whether the core constraint moved, stayed, or was misidentified.
4. Run the Project Auditor scan.
5. Apply Planner–Red Team–Judge to any material change.
6. Select one next priority; move the rest to Later/Out of Scope.
7. Update project state; append only material decisions.

Output: `结果 → 证据 → 偏差 → 最高风险 → 核心约束 → 下周唯一优先级 → 暂时不做 → 需确认`.

## Monthly review

1. Aggregate evidence without double-counting contacts or vanity signals.
2. Audit funnel progression: qualified targets → contacted → meaningful reply → price/quote → paid sample → order → repeat.
3. Reassess buyer definition, offer, landed economics, fulfillment, compliance, and trust gaps.
4. Re-test the core constraint and every active decision's `reconsider_when`.
5. Decide: continue, narrow, modify, pause, or stop. Do not scale without strong commercial evidence.
6. Set one monthly experiment and resource ceiling.

## Anomaly-event review

Trigger on a dispute, payment problem, compliance warning, missed delivery, spec mismatch, supplier failure, unexpected paid signal, repeated objection, rule change, threshold breach, or evidence contradicting an active decision.

Procedure: preserve raw evidence → stop unsafe commitments → identify impact radius → label known/unknown → test whether constraint or scope changed → Planner/Red Team/Judge → obtain approval for material action → log decision.

## Project Auditor

Rate each `高/中/低/未知`, cite evidence, and give one mitigation. Escalate only the highest threat to the current experiment or irreversible exposure.

| Area | Scan question |
|---|---|
| Evidence integrity | Did preference, praise, market size, or a listing become proof? |
| Buyer quality | Are targets genuinely high-fit B2B buyers? |
| Offer | Is the assortment coherent rather than a catalog dump? |
| Unit economics | Are product, packaging, payment, freight, duties/taxes, and margin inputs verified? |
| Product truth | Are material, dimensions, plating, MOQ, lead time, and QC claims traceable? |
| Compliance | Are destination and product obligations current and checked? |
| Fulfillment | Can samples/orders be produced, inspected, documented, and delivered as promised? |
| Commercial safety | Did a draft become an unapproved promise? |
| Scope | Did a new market, tool, website, or channel become active without a decision? |
| Focus | Are multiple items called first priority? |
| Test quality | Were sample, metric, window, and stop/change rules defined first? |
| Bias | Did sunk cost, insistence, or AI confidence override evidence? |

## Review record

```text
Review date / type:
Evidence received:
Result vs prior priority:
Strongest disconfirming evidence:
Auditor highest risk:
Core constraint (same/changed/unknown):
Planner proposal:
Red Team challenge:
Judge decision + confidence:
Next single priority:
Later / Out of Scope:
Stop/change criterion:
User approvals needed:
```
