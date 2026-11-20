# 6. Roadmap

[Back to the overview](../README.md)

The steps are in order. Each one depends on the one before. The pilot (step 4) is planned for early 2027. Later steps have no dates yet.

```mermaid
flowchart TB
  R1["1. Publish the cage tool"] --> R2["2. Build the AI attacker agent<br/>and its command log"]
  R2 --> R3["3. Build the research range<br/>and its answer sheet"]
  R3 --> R4["4. Pilot: one AI attack,<br/>caught and missed table"]
  R4 --> R5["5. Human red teamer<br/>on the same mission"]
  R5 --> R6["6. AI defender, scored<br/>like human analysts"]
  R6 --> R7["7. Hidden instructions<br/>in the logs"]
  R7 --> R8["8. Add guardrails,<br/>measure again"]
```

| Step | What it gives | Question |
| --- | --- | --- |
| 1. Publish the cage tool | Others can check how the AI attacker is contained | |
| 2. AI attacker agent and command log | A record of every action, ready for scoring | 1, 4 |
| 3. Research range and answer sheet | The place to measure, and the key to score against | 1 |
| 4. Pilot | The first real numbers: what was caught and what was missed, for one attack path | 1 |
| 5. Human red teamer on the same mission | The human number to compare with | 1 |
| 6. AI defender | An AI analyst scored on the same scale as people | 2 |
| 7. Hidden instructions in the logs | How often the AI defender can be fooled | 3 |
| 8. Guardrails, then measure again | Whether existing guardrails change the numbers | 3, 4 |

## What the pilot will and will not show

The pilot is small on purpose: one model, one range, one attack path, at least three runs. It will show that the method works and give a first caught and missed table. It will not support general claims about AI attackers.

## What would make it stronger

- More than three runs per setup, because AI agents vary from run to run.
- More than one model, so results are not about a single system.
- More than one attack path.
- Access to guardrails and to people who build them.

## Open decisions

See [Fair and repeatable](4-fair-and-repeatable.md#still-open).

[Back to the overview](../README.md)
