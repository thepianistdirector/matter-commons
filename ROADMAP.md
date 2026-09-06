# Matter Commons roadmap

This is a public planning repository. There is no product implementation or playable build yet. The image is an AI-generated vision reference, not a screenshot. All waves and tasks are proposed; no completed work, community approval or funding is implied.

The order reflects dependencies, not calendar commitments. Each wave advances only when its stated outcome is demonstrated and a maintainer accepts the next scope. Capacity targets are hypotheses to test.

## W1 — One physical design with explicit requirements

Define a bounded reference device and its assumptions.

- **W1-T1: Specify the environmental sensor reference.** Document purpose, dimensions, interfaces, power and environmental assumptions.
- **W1-T2: Model units, tolerances and design lineage.** Define shared identifiers and constraints across enclosure, board and BOM.

## W2 — Connect established engineering tools

Create the first editable cross-discipline package.

- **W2-T1: Build the mechanical design adapter.** Integrate a bounded parametric enclosure through an established open CAD tool.
- **W2-T2: Build the board and BOM adapter.** Link circuit components, board outline and bill of materials using an open electronics tool.

## W3 — Prove one useful engineering check

Make changes reviewable across the package.

- **W3-T1: Implement board-to-case fit verification.** Check the bounded mechanical envelope, holes and clearance constraints.
- **W3-T2: Implement proposed design changes.** Allow a human or agent to propose typed changes and inspect affected artifacts.

## W4 — From model to measured prototype

Connect analysis with real-world evidence.

- **W4-T1: Add a bounded simulation recipe.** Choose one useful supported analysis and document its assumptions and solver limits.
- **W4-T2: Prepare and document a physical prototype.** Produce reviewed build files and a test procedure; fabricate only with separately authorized resources.

## W5 — A community can reproduce the design

Make collaboration and portability dependable.

- **W5-T1: Publish the open design package format.** Export requirements, sources, constraints, adapters and licensing metadata.
- **W5-T2: Build review and component contribution flows.** Define how contributors propose parts, measurements and design variants.

## W6 — An engineering ecosystem people can trust

Validate reproducibility and operator effort.

- **W6-T1: Run independent reproduction exercises.** Invite volunteer teams to reproduce the model and, where resourced, the physical check.
- **W6-T2: Publish supported workflows and adapter conformance.** Define the first maintained tool versions, checks and contribution boundaries.

See [TASKS.md](TASKS.md) for observable acceptance criteria.
