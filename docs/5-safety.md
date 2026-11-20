# 5. Safety

[Back to the overview](../README.md)

This project runs AI attackers. These are the limits it works within.

## Where attacks run

- Only against the project's own isolated research range.
- Never against a client system, a live company network or the internet.
- The range holds no client data and no real personal data.

## The cage is always on

Every AI attacker runs inside a network cage. It can reach the range and the AI model it needs, and nothing else. This holds in every mode.

The cage has been tested: a 10-check escape test and 53 unit tests pass.

## Gates before a run

For authorized penetration tests, three checks must pass before any live run: authorization, scope, and the hosting provider's policy. Scope and authorization are enforced in code. The provider check is a written manual step.

## A person stays in charge

- A person starts every run and can stop it.
- A person resets the range and checks the run is valid.
- Decisions about what to build, run or publish are made by a person, not by an AI.

## Pentest mode and APT mode

Question 4 compares two modes: pentest mode, where the AI acts as a careful tester, and APT mode, where it acts like a real adversary.

- APT mode runs only against the isolated research range.
- The cage is on in APT mode, as in every mode.
- How APT mode works is private and is not in any public repository.

## What is not published, and why

| Not published | Why |
| --- | --- |
| Attack scenarios and technique lists | They could help misuse, and they could end up in the training data of models later tested here |
| Answer sheets and detection details | The attacker side must not know them |
| Guardrail settings | Knowing them would bias the tests |
| How APT mode works | It could help misuse |
| Client data of any kind | It is not part of this project |

## Honest reporting

- Nothing is reported as a result until it has been measured.
- Every result will come from at least three runs and will state its limits: how many runs, which model, which range.
- Runs that fail a validity check are kept and marked, not removed.

Next: [Roadmap](6-roadmap.md)
