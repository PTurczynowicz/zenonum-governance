# zenonum-governance

Public governance record for **zenonum**.

Zenonum is a system for building and running a product as a process: strategy, customer, problem, offer, experiments, requirements, implementation, assurance, and the next revision of all of those. It is built for a founder who has domain judgment and does not live in a repository.

This repository shows **how that system is governed**: many agents, narrow mandates, no role that proposes a change also accepts it, a written decision behind material changes, and tests that can send the work back.

It does not publish the product’s intellectual property.

Polski opis: [README.pl.md](README.pl.md).

## What you can verify here

Start with [Separation of duties](separation-of-duties.md) and the [Decision register](decision-register.md).

| Record | What it shows |
| --- | --- |
| [Architecture](architecture.md) | Platform, product runtime, and the factory that builds both |
| [Startup engine](startup-engine.md) | The living map: nodes, relations, scores, required moves, harvested context |
| [Interface](interface.md) | What a founder actually sees and is allowed to trust |
| [Agents that build zenonum](agents-that-build.md) | The factory roles |
| [Agents inside zenonum](agents-inside.md) | The product roles a founder is served by |
| [Permission matrix](permission-matrix.md) | Who may act, who may only judge, who may not touch the work |
| [Separation of duties](separation-of-duties.md) | The rules that keep autonomy from becoming a shortcut |
| [Decision register](decision-register.md) | A public fragment. Names, customers, and internal identifiers removed |
| [Assurance](assurance.md) | What was tested, how a failure is classified, what the evidence must contain |
| [Delivery architecture](delivery-architecture.md) | The next stage: from an accepted contract to a running, reversible product line |

## Maturity

Three words are used on purpose. They mark what is operating today. Limits are stated in the Limitations section below and in [Assurance](assurance.md).

| Word | Meaning |
| --- | --- |
| **Operating** | In the closed beta, or in the factory that built it |
| **Specified** | Decided and designed into the same product. Implementation is the current work |
| **Horizon** | The direction the decisions already point at |

The prose describes the operating model as one system. The tables mark which part is operating today.

## Operating snapshot

Figures from the construction that produced the closed beta. They move as the product moves.

| | |
| --- | --- |
| Builder time on the factory | 116 hours |
| Calendar span | 2026, alongside a full-time role |
| Product code | about 180,000 lines |
| Application modules | about 200 |
| Automated checks | more than 3,000 |
| Versioned schema migrations | more than 100 |
| API routes | about 120 |
| Product agents | 24, in 15 roles |
| Factory roles | 8 |
| Scoring passes | 6 |
| Documentation graph | about 35 MB, addressed as nodes, never pasted in full |

One person: a generalist with a finance and product background, not an engineer. A workflow that was the product under test.

## Limitations

This is the work of one author. The architecture, the security posture, and the code have not been independently reviewed, and nothing here claims compliance with any regulation or standard. The closed beta has been used by 10 external testers on their own projects. The delivery stage is specified, not yet built. The figures come from the author’s own tooling, and they move as the product changes.

## What this repository refuses to contain

- Prompt text, skills, and the method for writing them
- Scoring formulas, weights, and thresholds
- Source code, schemas, and wire contracts
- Customer data, sessions, and private decision history
- Secrets, host layout, allowlists, and credentials
- A license to build a copy

Copyright in this text stays with the author, Paweł Turczynowicz. Reading it is not a grant to reproduce the product.

## Why governance is the product

Models converge on the average product for a category. A founder’s advantage is empathy, unusual knowledge, and hypotheses far from that average. Zenonum’s job is to keep that advantage inside a process that can still be audited.

Autonomy is the default where the action is reversible, isolated, and already covered by a check. The founder is interrupted where the decision needs a human who can actually make it: taste, risk appetite, spend, secrets, legal exposure, irreversible data. Everything else is a role with a stop condition.

## Authorship

Prepared with the help of AI agents and edited by the author. © 2026 Paweł Turczynowicz. [LinkedIn](https://www.linkedin.com/in/pawel-turczynowicz)
