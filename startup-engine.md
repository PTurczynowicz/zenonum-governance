# Startup engine

The startup is not a document and not a chat transcript. It is a graph that recomputes when a fact changes.

Lean startup is encoded in the data, in the order of questions, and in the interface. It is not a slide the coach recites.

## Nodes and relations

Each node holds a statement and a small set of variables. Typical variables are confidence, importance, chance of success, failure pressure, cost, and revenue. Relations are typed. A change is not “update a paragraph.” A change is a write that other nodes are allowed to feel.

Nodes the founder works with include the shape of a plan: project, founder, customer, problem, offer, goals, experiments, roadmap, constraints, risks, contradictions, and tasks. Some of those stay off the map drawing and in queues, so a large plan remains navigable.

Empty placeholders exist so the method can show a missing piece without pretending the founder already decided it. Stale placeholders age out by rule. The coach does not delete them in prose.

## Six scoring passes

Operating. Six deterministic passes run over the graph. None of them is a model guessing a number.

| Pass | What the founder is owed |
| --- | --- |
| Normalization | Variables from different conversations land on one scale |
| Influence | A change in one node moves the nodes it bears on |
| Success potential | Where upside is real and still under-specified |
| Failure pressure | Where downside is heavy and still under-specified |
| Methodology completeness | Which part of the method is still empty |
| Next-move priority | Which gap is worth the next conversation |

The screen shows a single representative number. The number is an instrument. It is not the truth of the business. Bounds and machine detail stay off the default view and available only in an integrator disclosure.

A hard constraint pass can stop progression when a fundamental limit is violated, such as runway. That stop is code, not a mood in the coach’s reply.

## Two kinds of “what next”

| | Required move | Next best move |
| --- | --- | --- |
| Question it answers | What is missing or broken for this plan to be coherent? | What is the highest-leverage conversation now? |
| Source | Method rules and open contradictions | Ranked potential and confidence |
| Founder experience | A coach that opens on the gap and explains why | A ranked list with a short reason |

The required-move judge may be demanding. That is a product setting, reviewed on purpose, not a license for the judge to invent strategy.

## Conversation, then a canonical write

Every meaningful turn has two mouths and one of them is silent.

1. The coach talks to the founder. Only that reply is shown.
2. The extractor proposes nodes, relations, and variables from the conversation.
3. A schema check and a neighborhood bound run before anything is stored.
4. A local critic can reject a draft that does not hold together.
5. The founder sees a verbatim preview.
6. Save commits that preview. There is no second, hidden rewrite at save time.

If a new fact is ambiguous, it is withheld. The confident remainder can still be saved. The founder hears the clarifying question as a coach message, not as a JSON flag.

Machine fields — private reasons, steering notes, “finished” bits — never become chat text.

## Harvest, not the whole archive

Context is assembled per need.

The assembler chooses which nodes, which depth, and which files. Depth is a ladder: title, statement, essence, variables. An agent that is judging a local contradiction does not receive the entire history of the company. An agent that is reviewing a whole-plan risk does not receive every prompt in the platform.

This is what makes a large documentation graph affordable. The operating archive is tens of megabytes. Pasting it into a prompt is a defect, not a thoroughness.

## Background care

Several agents run because the graph changed, or because a clock fired, not because the founder pressed Send.

They look for contradictions, estimate variables, propose missing children after a goal becomes canonical, scaffold prerequisite chains, and narrate existential risk. A separate research agent runs only after the founder confirms a research brief. It files a report. It does not browse on every sentence.

The founder can set some of this care to manual or automatic. Deep research stays a confirmed brief either way.

## What the engine is for

A single chat window can draft a landing page. It cannot keep a changing strategy, a contradiction from last week, a research report, a required gap, and a roadmap in one accountable state.

The engine can. That was the point of building something larger than a prototype. The workflow was loaded until it should have fallen over. The closed beta is that load, still standing.
