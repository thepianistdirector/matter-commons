# Matter Commons: task contracts

Twelve proposed work packages, with named waves and dependency order. None is completed by publishing this document. The linked Tanduna revision is the contribution authority; this repository records the maintainer's intended contract while Tanduna's structured requirement support is being updated.

Every task below names its repository, branch, verified planning commit, preferred model, allowed fallback, immutable public skills, task-specific testing procedure and maintainer acceptance flow. A later implementation task still needs its prerequisite code, a rebased execution revision, narrow file scope and real functional commands. Do not treat the current planning commit as if that future code exists.

The allowed model pair is GPT-6 Astra and Claude Fable 5.1, with the effort stated per task. A model declaration is not independent runtime evidence; unresolved proof remains visible to the maintainer. See [CONTRIBUTING.md](CONTRIBUTING.md) and [the machine-readable authored contracts](task-contracts.json).

## W1-T1 — Specify the environmental sensor reference

**Wave:** W1 · **Prerequisites:** None; maintainer scope review first

Document purpose, dimensions, interfaces, power and environmental assumptions.

**Saved Tanduna task:** [W1-T1](https://tanduna.com/p/matter-commons/tasks/tsk_844482a7d3ba74b1920eca4b9301de86)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Maintainer accepts the scoped design protocol; this is not product implementation.

**Preferred:** `gpt-6-astra` / medium. **Accepted fallback:** `claude-fable-5-1` / medium. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Each requirement has a measurable check or is explicitly marked unresolved.
- The reference excludes regulated or safety-critical use and identifies needed physical tests.

### Testing procedure

Trace the environmental sensor's purpose, dimensions, power and interfaces to measurable requirements. Walk an unresolved requirement and a needed physical test explicitly; keep regulated/safety-critical applications outside this reference.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

This task uses the saved reproducible manual protocol. Distinguish paper/synthetic exercises from actual participant or physical observations.

**Evidence artifact:** `docs/work/W1-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W1-T2 — Model units, tolerances and design lineage

**Wave:** W1 · **Prerequisites:** W1-T1

Define shared identifiers and constraints across enclosure, board and BOM.

**Saved Tanduna task:** [W1-T2](https://tanduna.com/p/matter-commons/tasks/tsk_72aeb509f80800724b400b9fe2f0862f)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- A unit mismatch and a conflicting clearance requirement are detected in fixtures.
- Every critical dimension links to its requirement or stated assumption.

### Testing procedure

Create enclosure, board and BOM records with shared IDs, units and tolerances. Introduce a unit mismatch and conflicting clearance; verify each is detected and traced to its requirement or assumption.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W1-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W2-T1 — Build the mechanical design adapter

**Wave:** W2 · **Prerequisites:** W1-T1, W1-T2

Integrate a bounded parametric enclosure through an established open CAD tool.

**Saved Tanduna task:** [W2-T1](https://tanduna.com/p/matter-commons/tasks/tsk_7515997808194137220647fb2553cc2a)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Changing a declared dimension regenerates editable geometry and drawings.
- Unsupported geometry operations fail without replacing the source with an opaque render.

### Testing procedure

Change a supported enclosure dimension and regenerate editable geometry/drawings in the chosen tool. Attempt an unsupported operation; preserve source and report the limit rather than replacing it with a render.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W2-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W2-T2 — Build the board and BOM adapter

**Wave:** W2 · **Prerequisites:** W1-T1, W1-T2

Link circuit components, board outline and bill of materials using an open electronics tool.

**Saved Tanduna task:** [W2-T2](https://tanduna.com/p/matter-commons/tasks/tsk_288e661272c62349ef72954ef671a889)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Component identifiers remain consistent across schematic, board and BOM.
- A missing or incompatible component is visible before export.

### Testing procedure

Edit a component and inspect schematic, board and BOM identifiers. Remove or substitute an incompatible component and verify the issue is visible before producing reviewed export files.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W2-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W3-T1 — Implement board-to-case fit verification

**Wave:** W3 · **Prerequisites:** W2-T1, W2-T2

Check the bounded mechanical envelope, holes and clearance constraints.

**Saved Tanduna task:** [W3-T1](https://tanduna.com/p/matter-commons/tasks/tsk_99da06268bc0438f806392421ee44b32)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- A deliberately oversized board or displaced hole fails the check.
- Results disclose tolerances and what geometry is not covered.

### Testing procedure

Check the reference board/case fit, then oversize the board and displace a mounting hole. Verify both counterexamples fail and record tolerances and geometry excluded from the calculation.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W3-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W3-T2 — Implement proposed design changes

**Wave:** W3 · **Prerequisites:** W2-T1, W2-T2, W3-T1

Allow a human or agent to propose typed changes and inspect affected artifacts.

**Saved Tanduna task:** [W3-T2](https://tanduna.com/p/matter-commons/tasks/tsk_d1f50ac1ef1f4a60d83f60fbd91ae689)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- A reviewer sees which dimensions, components, drawings and costs may change.
- Rejected changes leave the accepted design package intact.

### Testing procedure

Propose a typed dimension or component change and inspect affected geometry, drawing and BOM. Reject it and confirm the accepted package remains intact; repeat with a conflicting requirement.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W3-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W4-T1 — Add a bounded simulation recipe

**Wave:** W4 · **Prerequisites:** W3-T1, W3-T2

Choose one useful supported analysis and document its assumptions and solver limits.

**Saved Tanduna task:** [W4-T1](https://tanduna.com/p/matter-commons/tasks/tsk_56826ef304acef919a2dd2af0a1dee83)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- The recipe includes a reference case with a known expected result.
- Reports separate simulated estimates from measured physical performance.

### Testing procedure

Run the chosen solver recipe on a known reference case, then a changed parameter within its supported range. Report assumptions and error/solver limits; label results as simulated rather than physically measured.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W4-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W4-T2 — Prepare and document a physical prototype

**Wave:** W4 · **Prerequisites:** W3-T1, W3-T2, W4-T1

Produce reviewed build files and a test procedure; fabricate only with separately authorized resources.

**Saved Tanduna task:** [W4-T2](https://tanduna.com/p/matter-commons/tasks/tsk_6639dc4c19223b704536a821aef915e8)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Build outputs include versioned drawings, BOM and assembly notes.
- Any physical results name the actual revision, equipment and observed limitations.

### Testing procedure

Review versioned drawings, BOM, assembly notes and a physical test procedure. If separately resourced fabrication occurs, record the actual built revision, equipment, measured results and discrepancies; otherwise mark physical tests NOT RUN.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

This task uses the saved reproducible manual protocol. Distinguish paper/synthetic exercises from actual participant or physical observations.

**Evidence artifact:** `docs/work/W4-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W5-T1 — Publish the open design package format

**Wave:** W5 · **Prerequisites:** W4-T1, W4-T2

Export requirements, sources, constraints, adapters and licensing metadata.

**Saved Tanduna task:** [W5-T1](https://tanduna.com/p/matter-commons/tasks/tsk_237d1500c3c6c9387062ffc3ed44e937)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Another contributor reopens and edits the reference design without private files.
- Missing tool versions or components are diagnosed clearly.

### Testing procedure

Have another contributor reopen and edit the exported design with only public files. Remove a tool version or component reference and verify a clear diagnostic; check artifact and license metadata preservation.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W5-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W5-T2 — Build review and component contribution flows

**Wave:** W5 · **Prerequisites:** W4-T1, W4-T2, W5-T1

Define how contributors propose parts, measurements and design variants.

**Saved Tanduna task:** [W5-T2](https://tanduna.com/p/matter-commons/tasks/tsk_47370c84415d73d90ef0ea9b23fe7d1f)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- A component record distinguishes datasheet claims from community measurements.
- Review preserves attribution and prevents incompatible licenses from being silently combined.

### Testing procedure

Submit a component with separate datasheet claims and measured values, review it, then reject an incompatible-license or untraceable variant. Confirm attribution and accepted design records remain intact.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W5-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W6-T1 — Run independent reproduction exercises

**Wave:** W6 · **Prerequisites:** W5-T1, W5-T2

Invite volunteer teams to reproduce the model and, where resourced, the physical check.

**Saved Tanduna task:** [W6-T1](https://tanduna.com/p/matter-commons/tasks/tsk_ee1fb80ba97d9d7e89f90720fcea07d3)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- Report discrepancies and failed reproductions alongside successful ones.
- Update requirements or adapters using measured findings.

### Testing procedure

Have independent volunteer teams reproduce the model and any separately resourced physical check. Publish failed as well as successful reproduction findings and trace resulting requirement/adapter revisions.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

This task uses the saved reproducible manual protocol. Distinguish paper/synthetic exercises from actual participant or physical observations.

**Evidence artifact:** `docs/work/W6-T1/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.

## W6-T2 — Publish supported workflows and adapter conformance

**Wave:** W6 · **Prerequisites:** W5-T1, W5-T2, W6-T1

Define the first maintained tool versions, checks and contribution boundaries.

**Saved Tanduna task:** [W6-T2](https://tanduna.com/p/matter-commons/tasks/tsk_066cdcae5dd43c8820f1034f4e689249)

**Repository:** [https://github.com/thepianistdirector/matter-commons](https://github.com/thepianistdirector/matter-commons) · **Branch:** `main`

**Planning base commit:** [`b9379b2ae99f6553039edd9133a62c54b478baa0`](https://github.com/thepianistdirector/matter-commons/commit/b9379b2ae99f6553039edd9133a62c54b478baa0)

**Execution gate:** Prerequisite results must be accepted and integrated. Maintainer publishes a new task revision against that integrated base before execution; runtime work also needs the real harness and exact allowed paths.

**Preferred:** `gpt-6-astra` / high. **Accepted fallback:** `claude-fable-5-1` / high. Other models require a maintainer revision before work.

**Required skills:** [contribution protocol](https://raw.githubusercontent.com/thepianistdirector/context-harbor/a288bac1ff8bf87fe382ee6bf15ace4c0a090cbd/.agents/skills/tanduna-contribution/SKILL.md) and [Matter Commons validation](https://raw.githubusercontent.com/thepianistdirector/matter-commons/b9379b2ae99f6553039edd9133a62c54b478baa0/.agents/skills/matter-commons-validation/SKILL.md), at the linked immutable versions.

### Acceptance criteria

- A second design exercises the same adapters without custom core changes.
- Support claims state geometry, electronics and simulation limits explicitly.

### Testing procedure

Run a second bounded design through the same maintained adapters and conformance checks. Include an unsupported geometry/electronics/solver case and state the actual supported versions and limits.

Record setup/fixtures, actions, expected and observed results, relevant logs or artifacts, and PASS / FAIL / NOT RUN for each criterion.

Existing baseline checks (repository root; identity and patch hygiene only):

```sh
git rev-parse HEAD
git status --short
git diff --check b9379b2ae99f6553039edd9133a62c54b478baa0
```

Exact functional commands, fixtures and paths must be ratified in the execution revision once the prerequisite-selected stack/harness exists. Do not claim these future checks ran.

**Evidence artifact:** `docs/work/W6-T2/acceptance.md` plus the actual patch, fixtures and logs within the approved task scope.

### Acceptance workflow

1. Contributor identifies the saved Tanduna task revision, repository/base, accepted prerequisites, selected primary or fallback model and effort, and exact required skill versions.
2. Contributor performs the task-specific testing procedure and maps each original acceptance criterion to setup, expected result, observed result and reproducible evidence. Failed and unrun checks remain visible.
3. Maintainer reproduces the material checks, reviews the scoped patch or design artifact and verifies the stated model/skill evidence. Unsupported model claims or missing evidence remain unresolved rather than accepted automatically.
4. Maintainer records acceptance or requested changes against the reviewed revision. A passing format check, generated patch or completed model invocation does not by itself satisfy the task.
