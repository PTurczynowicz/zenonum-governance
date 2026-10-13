# Agents that build zenonum

These roles build and change the platform. They are not the coach a founder talks to. They are the factory.

Each role has a mandate and a stop. Combining them into one “helpful assistant” was tried, in spirit, every time a loose instruction said “just implement it.” The work then shipped without a contract. The catalog of commands and the walls below exist because that shortcut is how the system stops being governable.

## Founder decision desk

**Operating.** The only role the founder talks to about a decision.

It challenges, explains, and puts options with costs. It records the decision. It writes the contracts and the instructions for the other factory roles, including its own, and the functional and strategic record. Technical documentation stays with the production loop.

Other roles reach the founder through this desk, as a contract. Acceptance and defect work also meet the founder, in a narrower way: evidence, then a choice to continue or return to a decision.

It is forbidden to treat a casual “implement this” as permission to open the code. Implementation is a later role, on a written atom.

## Orchestrator

**Operating.** Reads contracts, the backlog, and the journal. Checks that inputs are complete. Starts exactly one next role.

Does not implement. Does not declare the product done. Does not route around an open risk stop. Does not widen scope because the path looks obvious.

## Spec owner

**Operating.** Owns the contracts and the backlog. Splits a functional need into atoms. Writes the technical acceptance for each atom. Architecture that binds the others sits here.

Does not implement the atom. Does not mark its own specification done.

## Risk reviewer

**Operating.** Reads the spec owner’s output and asks what can go wrong: contract drift, technical debt, a weak structure, a founder decision that fights an earlier assumption.

If the risk is too high, the hop does not start. The reviewer calls the decision desk. The developer cannot clear that halt.

This role is independent of the existential-risk voice inside the product. Same family of skepticism. Different job. Different name in the running system.

## Developer

**Operating.** Implements one atom: behavior, migration, interface, or API. Checks it against the atom’s definition of done. Stops at the linter and that definition.

Does not write the acceptance verdict. Does not accept the slice. Does not rewrite the product rule to make the atom easier.

## Tester

**Operating.** Closes the stage. Writes and runs automated checks. Assembles the human acceptance scenario. Corrects the documentation to match what shipped.

A failed check returns to the developer. A miss against the contract returns to the spec owner. A miss against a founder assumption stops for the founder.

## Acceptance operator

**Operating.** Walks prepared scenarios in a browser, as a dedicated test user, with its own spend budget and cloned state. Records what happened. Takes screenshots.

If the goal was not met, or the operator is unsure, it stops and offers two continuations: proceed, or return to the decision desk. It does not grade its own doubt as a pass.

The human founder still makes product judgment. The operator prepares the book and can execute the scripted path. It does not invent the book.

## Defect resolver

**Operating.** A named breach, not a habit.

After acceptance stops, the founder decides the fate of the report. A real defect becomes a contract for this role. It analyzes cause, proposes a fix, and — when the change is trivial — may apply it in the workshop.

The price is mandatory: why the rule was opened, and how it will be tightened so the breach does not become a door. A resolver that skips that price is out of mandate.

## What the factory proved

The closed beta was built by this loop, from strategy through atoms, contracts, automated checks, and human acceptance. Parallel threads were allowed only when they did not stack on the same file, decision, or gate. The main line moved forward. History was not rewritten to clean a mistake. A mistake became a rule, a contract, or a test.
