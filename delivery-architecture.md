# Delivery architecture

The closed beta carries a founder from strategy to an accepted contract. The next stage carries that contract into a product that can be built, tested, released, watched, and revised. It is the same zenonum. It is not an engineering tool that forgot the strategy.

Status below is **Specified** unless a line says **Horizon**.

## What a founder is buying next

- Several durable product lines for different segments, and short-lived variants for experiments
- Journeys, interfaces, design, messaging, architecture, contracts, and code as nodes in one graph
- Agents that plan, implement, test, deploy, observe, and maintain, reviewing one another
- An assurance center, including browser regression, that the founder can read
- Safe use of external research, hosting, analytics, and engineering tools
- A handoff package when an external workshop is the better executor
- Evidence flowing back into the strategy, not dying in a ticket system

Zenonum does not promise “simple products only.” It may attempt work past what the last run proved. The limit is discovered: model, tools, context, risk, budget, and how much guidance the founder can usefully give. A phase that cannot yet run the far target must still leave a path toward it, not a dead end.

## From graph to a running tree

The graph remains the source of truth. A compiler, which is not an agent, materializes a file tree from the nodes that hold implementation sections. It runs a static gate. It records the run. It promotes a pointer. Agents do not edit the promoted tree and call that the specification.

A delivery agent may hold work in progress across several units, materialize, test, and iterate before the orchestrator accepts the bundle. Until acceptance, that work is not the operative plan.

Scope freezes when the plan is accepted. A later “small amendment” outside the frozen set is rejected. Locks are universal: if any batch holds a node, no role writes it. Parallel work continues only on nodes the lock does not cover. That is the factory’s disjoint-thread rule, applied to a founder’s product.

## Coding difficulty is explicit

The business analyst sets, on each unit that contains code, how hard the coding is expected to be. The setting is explicit. It does not inherit from the root of the graph. It does not describe how hard the specification was to write.

Below a threshold, materialization is a single pass. Above it, materialization may iterate, with a reviewer that is not the author, when the gate fails. Either way, a unit that claims to contain code is not complete until materialization has succeeded.

## Risk-based release

| Class | Typical action | Control |
| --- | --- | --- |
| Autonomous | Publish a static experiment on an isolated route, no new secret, no unapproved spend, automatic rollback | Validators and the grant |
| Independent control | Shared behavior, a compatible schema change, a customer-visible workflow | Separate proposer, reviewer, tester, executor |
| Founder | Connect a secret, spend past the grant, destroy data, accept legal terms, change risk policy, clear an emergency stop | Recorded founder decision |

The founder can set autonomy by area, spend, providers, and how often to be told. Those settings change when the orchestrator pauses. They never grant a secret or disable a validator.

An emergency stop pauses new autonomous work, expires grants, and halts in-flight work at the next safe checkpoint. The audit of policy and action is append-only.

## Product lines

Horizon, on a specified spine.

A shared core stays explicit. A product line diverges on purpose. An experiment is a temporary variant, not a quiet edit to the core. Releases are versioned. A prior version is recoverable. Data ownership is deterministic: platform graph in the platform store, customer data in the project store.

Assurance links scenarios to outcomes, journeys, interfaces, contracts, migrations, the shared core, the product line, and the experiment. A change selects regression by those links, not by running the world because it is Tuesday.

## When the run is not enough

1. An independent agent reviews the work.
2. A specialist agent, or a stronger model, takes the narrow failure.
3. The founder is asked for a decision the founder can actually make.
4. An external service is used with a guided contract.
5. A technical handoff exports requirements, architecture, contracts, unresolved decisions, assurance expectations, graph references, and agent instructions to another engineering environment.

The first export of that package belongs to the technical phase. Earlier phases stay valuable inside zenonum without pretending they already produced a repository.

## What stays true while the product moves

Better models do not retire these requirements:

- stable identity of the product and of each product line
- an explicit shared core and intentional divergence
- versioned requirements and releases
- traceable experiments and evidence
- bounded authority
- reproducible execution
- observable failures
- a prior version that can be restored

The closed beta is the proof that a governed multi-agent loop can build a serious product from strategy through acceptance. This stage is that loop, pointed at the founder’s customers.
