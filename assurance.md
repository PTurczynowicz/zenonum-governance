# Assurance and test results

Testing is part of the product’s claim, not a private habit. A change is not done because an agent says it is done. It is done when the check that role does not control has passed, and when human judgment has been asked only for what a human should judge.

## What the factory runs

Operating snapshot from the construction of the closed beta:

| Evidence | Result |
| --- | --- |
| Automated checks | More than 3,000, across services, contracts, and interface behavior |
| Schema migrations | More than 100 versioned steps, applied in order, fail-closed when state is uncertain |
| API surface | About 120 routes, covered by contract checks rather than by a public schema dump |
| Application modules | About 200 |
| Deploy smoke | Security headers and rate limits included |
| Secret scan on result files | A result that contains a key-shaped value is not written |
| Human product-value scenario | Scripted journey with three separate verdicts |
| Browser-assisted acceptance | Prepared scenarios, dedicated test user, screenshots, stop on doubt |
| Closed beta | In use by 10 external testers on their own projects |
| Independent code and security review | Not performed |

These counts come from the author’s own tooling and have not been independently verified. Counts move. They are published here as the order of magnitude of the system that exists, not as a marketing ceiling.

## Three verdicts, kept apart

| Verdict | Who gives it | What a pass means | What it does not mean |
| --- | --- | --- | --- |
| Deterministic | A check against stored state and responses | The invariant held | The coaching was wise |
| Semantic | A bounded rubric, recommended by the operator | The behavior matched the intent closely enough | The founder liked the strategy |
| Founder judgment | The founder, on a prepared book | The product still makes sense | The automated check can be ignored |

A miss on the deterministic layer is not washed out by a kind reading. A pass on the deterministic layer does not close a question of taste.

## Where a failure goes

| What failed | Where it returns |
| --- | --- |
| A check, a linter, a definition of done | Developer, same atom |
| The contract | Spec owner |
| A founder assumption | Decision desk. The hop stops |
| A goal in browser acceptance, or an operator’s doubt | Stop. Continue, or return to the decision desk |
| A trivial defect after that stop | Defect resolver, with the breach priced in writing |

Partial is a real outcome. An acceptance path that never reached the state under test is partial. It is not recorded as a pass.

## What an evidence file is allowed to contain

Operating.

- Which behavior was asserted, in plain language
- The expected shape and the observed shape
- Pass, partial, or fail
- That a redaction guard ran, and that it found nothing key-shaped
- The kind of check: exact, present, one of a list, a range, or contains

An evidence file is built from an allowlist of fields. It is not a dump of headers, environment, or transport. Model output is checked structurally, because a language reply is not deterministic. The bar is that the claim holds, not that the sentences match.

No session identifier, host name, or credential appears in this public record.

## Layers

Operating today: schema and graph validation, unit and contract checks, interface checks, deploy smoke, scripted human scenarios, and browser-assisted acceptance with a stop rule.

Specified for the delivery stage, in this order:

1. Schema and graph validation
2. Static analysis and compilation
3. Unit checks
4. Contract and integration checks
5. Component checks
6. Browser checks selected by what the change touches
7. Critical browser smoke on deployment
8. Scheduled broader regression
9. A compatibility matrix across product lines
10. Human acceptance for product judgment

Browser automation is acceptance regression. It does not replace the founder’s judgment. The founder is not asked to re-enact the regression by hand either.

## Assurance the founder will be able to read

Specified. An assurance center answers three questions in the same language as the map:

- What is known to work
- What has not been tested
- Which product line or experiment is exposed

A scenario is a durable object: preconditions, actor, actions, expected outcome, the requirements and journeys it covers, whether it is automated, and what evidence it must leave. A run, a screenshot, a trace, and a flake streak are operational records. They point at a scenario, a release, and a graph revision. They are not a node per click.

Continuous change is acceptable when four things hold together: detection, containment, recovery, and learning. An incident becomes a finding, a graph correction, and a regression scenario. That is the same rule the factory already uses on itself: a defect leaves knowledge.

## What this does not claim

The author of the system is not an impartial judge of whether the architecture, the security posture, and the code meet the bar of a regulated institution. The factory was built without that external judge, and the Limitations section of the README says so.

What the evidence does support: a single generalist, in 116 hours, with this separation of duties, produced a closed beta on the order of the snapshot above, and the loop carried it from strategy through automated checks and human acceptance. The delivery stage is how that same evidence standard is meant to follow a founder’s product out of the plan and into a release.
