# Matter Commons: proposed work packages

These are planning briefs. No task is complete or approved for automatic execution. Before implementation, maintainers must publish a scoped task revision with the actual repository, paths, tools and validation commands.

## W1-T1 — Specify the environmental sensor reference

**Wave:** W1 · **Status:** Planned · **Prerequisites:** None; begin with maintainer scope review

Document purpose, dimensions, interfaces, power and environmental assumptions.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Each requirement has a measurable check or is explicitly marked unresolved.
- The reference excludes regulated or safety-critical use and identifies needed physical tests.

## W1-T2 — Model units, tolerances and design lineage

**Wave:** W1 · **Status:** Planned · **Prerequisites:** W1-T1

Define shared identifiers and constraints across enclosure, board and BOM.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- A unit mismatch and a conflicting clearance requirement are detected in fixtures.
- Every critical dimension links to its requirement or stated assumption.

## W2-T1 — Build the mechanical design adapter

**Wave:** W2 · **Status:** Planned · **Prerequisites:** W1-T1, W1-T2

Integrate a bounded parametric enclosure through an established open CAD tool.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Changing a declared dimension regenerates editable geometry and drawings.
- Unsupported geometry operations fail without replacing the source with an opaque render.

## W2-T2 — Build the board and BOM adapter

**Wave:** W2 · **Status:** Planned · **Prerequisites:** W1-T1, W1-T2

Link circuit components, board outline and bill of materials using an open electronics tool.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Component identifiers remain consistent across schematic, board and BOM.
- A missing or incompatible component is visible before export.

## W3-T1 — Implement board-to-case fit verification

**Wave:** W3 · **Status:** Planned · **Prerequisites:** W2-T1, W2-T2

Check the bounded mechanical envelope, holes and clearance constraints.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- A deliberately oversized board or displaced hole fails the check.
- Results disclose tolerances and what geometry is not covered.

## W3-T2 — Implement proposed design changes

**Wave:** W3 · **Status:** Planned · **Prerequisites:** W2-T1, W2-T2

Allow a human or agent to propose typed changes and inspect affected artifacts.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- A reviewer sees which dimensions, components, drawings and costs may change.
- Rejected changes leave the accepted design package intact.

## W4-T1 — Add a bounded simulation recipe

**Wave:** W4 · **Status:** Planned · **Prerequisites:** W3-T1, W3-T2

Choose one useful supported analysis and document its assumptions and solver limits.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- The recipe includes a reference case with a known expected result.
- Reports separate simulated estimates from measured physical performance.

## W4-T2 — Prepare and document a physical prototype

**Wave:** W4 · **Status:** Planned · **Prerequisites:** W3-T1, W3-T2

Produce reviewed build files and a test procedure; fabricate only with separately authorized resources.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Build outputs include versioned drawings, BOM and assembly notes.
- Any physical results name the actual revision, equipment and observed limitations.

## W5-T1 — Publish the open design package format

**Wave:** W5 · **Status:** Planned · **Prerequisites:** W4-T1, W4-T2

Export requirements, sources, constraints, adapters and licensing metadata.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Another contributor reopens and edits the reference design without private files.
- Missing tool versions or components are diagnosed clearly.

## W5-T2 — Build review and component contribution flows

**Wave:** W5 · **Status:** Planned · **Prerequisites:** W4-T1, W4-T2

Define how contributors propose parts, measurements and design variants.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- A component record distinguishes datasheet claims from community measurements.
- Review preserves attribution and prevents incompatible licenses from being silently combined.

## W6-T1 — Run independent reproduction exercises

**Wave:** W6 · **Status:** Planned · **Prerequisites:** W5-T1, W5-T2

Invite volunteer teams to reproduce the model and, where resourced, the physical check.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- Report discrepancies and failed reproductions alongside successful ones.
- Update requirements or adapters using measured findings.

## W6-T2 — Publish supported workflows and adapter conformance

**Wave:** W6 · **Status:** Planned · **Prerequisites:** W5-T1, W5-T2

Define the first maintained tool versions, checks and contribution boundaries.

Start only after the listed prerequisites and scope are accepted by a maintainer. Work in the project's own repository. Document assumptions, unresolved questions and reproducible evidence. This is a proposed work package, not a claim that the implementation already exists.

Acceptance criteria:

- A second design exercises the same adapters without custom core changes.
- Support claims state geometry, electronics and simulation limits explicitly.
