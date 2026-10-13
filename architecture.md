# Architecture

Zenonum is three cooperating systems with hard walls between them.

```text
Founder
   │  one decision conversation
   ▼
┌──────────────────────────┐
│  Factory                 │  builds and changes zenonum itself
│  narrow roles, one atom  │
│  at a time, written gates│
└────────────┬─────────────┘
             │ deploys
             ▼
┌──────────────────────────┐
│  Platform                │  the founder’s strategy and plan
│  graph, agents, scores,  │
│  research, administration│
└────────────┬─────────────┘
             │ accepted contract
             ▼
┌──────────────────────────┐
│  Project world           │  the product the founder ships
│  its own data, secrets,  │  Specified
│  runtime, and releases   │
└──────────────────────────┘
```

The factory is operating. The platform is operating as a closed beta. The project world is the delivery architecture the same governance is now closing around. It is not a second product.

## Platform

The platform holds the founder’s venture as a graph.

A **node** is one durable object: a problem, a customer segment, a goal, an experiment, a constraint, a risk, a contradiction, a task, a decision. A **relation** says how two nodes bear on each other: depends on, groups, contradicts, precedes, replaces. Variables sit on nodes: confidence, importance, upside, downside, cost, revenue pressure.

The founder does not edit that graph as a database. The founder talks. A coach answers in plain language. A separate extractor proposes the canonical write. Deterministic services then recompute what the change did to the rest of the map. Background agents look for gaps, contradictions, and risks on their own clocks.

Administration is a different door: models, prompts, skills, test operations, and observability. A founder session cannot open it.

## Factory

The factory is the agentic workflow that built the platform and still changes it.

Documentation is the source of truth. Code is the current materialization of an accepted contract. An agent does not receive the whole archive. It receives a **harvest**: which nodes, how deep (title, body, essence, variables), and which files it may touch.

Work moves in small atoms. One role writes the contract. Another role may stop the hop for risk. Another role implements exactly that atom. Another role tests and either accepts, returns the work, or stops for the founder. The longest unattended run in construction lasted nearly three days. The limit was the stock of decisions the founder had already made, not the number of steps the agents could take.

Isolation is inside the loop. Two threads may run together when they do not share a file, a decision, or a gate. They do not isolate by opening a side branch for every idea.

Delivery of the platform itself is a script: incremental migrations, fail-closed when state is uncertain, a smoke check after deploy, and a rollback of state when the check requires it. Security headers and rate limits are part of that smoke, not a later hardening project.

## Project world

Specified. When zenonum carries a founder’s own product past the contract, that product lives in a separate world:

- its own database, never the platform’s graph store
- its own secrets, never written into a node and never placed in a model prompt
- its own runtime, promoted from the graph by a deterministic compiler
- its own backups, migrations, and release pointer

Agents may author the specification on the platform graph. They may not treat the running product as a scratchpad. The compiler materializes. An acceptance runner tests the promoted surface. A reviewer who did not write the change issues the verdict.

Co-locating both worlds on one machine during early delivery does not merge them.

## What is an agent, and what is not

An agent is a model role with a mandate, an input, an output, and a list of forbidden actions.

A deterministic service is used wherever drift would be a defect:

- scores and propagation
- schema and hallucination bounds
- context assembly
- migration and deploy
- materialization from graph to a file tree
- secret injection on the acceptance runner only

If a step must be repeatable, it is a versioned service. The model is not asked to improvise it.

## Authority

| Surface | Who decides | What is recorded |
| --- | --- | --- |
| Product meaning, taste, risk appetite | Founder, in one decision conversation | A decision node, with cause |
| Contract and acceptance criteria | Spec owner | Backlog atom and definition of done |
| “This can go wrong” | Independent risk reviewer | A halt, or a written acceptance of the risk |
| Implementation of one atom | Developer | The change, tied to the atom |
| Whether the atom holds | Tester | Automated result, or a return |
| Whether the product still makes sense | Founder, on a prepared acceptance book | Judgment, separate from the machine result |
| Math, schema, materialization | Deterministic services | Run record, formula version, recipe id |

## External tools

Cursor is the workshop the factory was proven in. The delivery architecture treats any capable engineering or browser runner as a replaceable executor. Zenonum keeps the task identity, the context package, the authority boundary, the expected result, the evidence format, and the verdict. The executor does not keep them.
