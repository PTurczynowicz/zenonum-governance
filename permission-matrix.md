# Permission matrix

Read this as governance, not as an API. “May” means the role is allowed to cause that effect. “No” means the effect is a defect if it happens.

Status: **Operating** for the factory and the closed beta. **Specified** for delivery into a founder’s own product.

## Factory

| Action | Founder desk | Orchestrator | Spec owner | Risk reviewer | Developer | Tester | Acceptance operator | Defect resolver |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Challenge a decision and record it | May | No | Proposes | May halt | No | No | Reports | Reports |
| Choose the next role | No | May | No | May stop the hop | No | May return work | May stop | No |
| Write or change a contract | May direct | No | May | May object | No | May flag a miss | No | May propose |
| Implement one atom | No | No | No | No | May | No | No | May, only if trivial and recorded |
| Accept the atom | No | No | No | No | No | May | May execute, not judge taste | No |
| Change product meaning | May | No | No | No | No | No | No | No |
| Rewrite history to erase a mistake | No | No | No | No | No | No | No | No |
| Run in parallel with another thread | — | May, if disjoint | May, if disjoint | May, if disjoint | May, if disjoint | May, if disjoint | May, if disjoint | May, if disjoint |

Disjoint means: not the same file, not the same decision, not the same gate.

## Product, closed beta

| Action | Coach | Guardrail | Extractor | Critic | Scoring engines | Background care | Research | Admin curator | Founder |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Speak to the founder | May | Refusal only | No | No | No | No | Via a report | No | May |
| Propose a graph write | No | No | May | Verdict only | No | May, in their lane | Files a report | No | By saving the preview |
| Commit a write | No | No | No | No | Propagate on save | No | No | No | May |
| Compute scores | No | No | No | No | May | No | No | No | No |
| See secrets or another founder’s plan | No | No | No | No | No | No | No | No | Own plan only |
| Change an agent instruction | No | No | No | No | No | No | No | May, in administration | No |
| Lower a safety cadence | No | No | No | No | No | No | No | No | No |

## Delivery into a founder’s product

Specified.

| Action | Product owner | Analyst | Architect | Delivery | Critic | Risk reviewer | Compiler | Acceptance runner | Orchestrator | Founder |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Business scope and journey | May | No | No | No | Verdict | Flag | No | No | Schedule | May override |
| Technical contract | Outline | May | Layout | No | Verdict | Flag | No | No | Freeze scope | May override |
| Implementation sections | No | No | No | May | Plan verdict | Flag | Materialize | No | Lock | No |
| Edit the promoted running tree | No | No | No | No | No | No | Promote pointer | Read and run | No | No |
| Issue a verdict | May | May | May | No | May | May | Optional | May | May | May |
| Inject a project secret | No | No | No | No | No | No | Into the product runtime only | Into the test run only | Trigger | May connect |
| Spend beyond the grant | No | No | No | No | No | No | No | No | No | May |
| Lower a deterministic risk class | No | No | No | No | No | No | No | No | No | Only by changing policy, which is itself recorded |

## Autonomy levels

Specified as policy. Parts of the factory already run at the first two levels.

| Level | When it is enough | Who still has to be someone else |
| --- | --- | --- |
| Autonomous | Reversible, isolated, observable, inside budget, already covered by a check | A validator. Not a second opinion |
| Independent control | Shared behavior, a compatible schema change, a customer-visible workflow, recoverable but wide | Proposer, reviewer, tester, and executor are different roles |
| Founder control | Secrets, spend past the grant, irreversible data, legal or regulated exposure, emergency stop, risk policy | The founder. Not as a stand-in for a test suite |

Agents may raise the risk class. They may not lower a trigger that a rule already fired.

## Credential walls

Operating.

| Wall | Rule |
| --- | --- |
| Prompt and tool arguments | No secret, ever |
| Acceptance identity | A dedicated test user. Its credential is injected by the runner, not typed into a prompt |
| Logs | Redacted. A result file that contains a key-shaped value is refused |
| Platform store vs product store | Separate databases, even on one host |
| Public API description | Disabled on staging and production |
| Allowlists | Closed beta, administration, and acceptance are different lists |
