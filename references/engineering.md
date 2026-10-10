# Software engineering

Use this module for feature work, fixes, refactors, tests, and code review.

## Implement

1. Inspect repository-specific instructions, the working tree, relevant issue/specification, dependency manifests, runtime and framework versions, nearby code, tests, and documented commands. Do not assume a familiar stack uses the latest version.
2. Translate the request into observable acceptance conditions. Identify invariants, compatibility expectations, affected interfaces, and out-of-scope behavior.
3. Consult current authoritative documentation for version-sensitive APIs, security-sensitive behavior, and compatibility decisions. Compare it with the repository's actual versions and conventions. If missing information materially affects correctness, resolve it or report the bounded alternatives.
4. Choose the smallest coherent change that meets the requirements. For larger work, create bounded passes with dependencies and checks. Parallelize only independent tasks and avoid concurrent edits to shared files without an explicit integration plan.
5. Preserve behavior that is relied on by existing callers unless the task authorizes a change. Before removing compatibility code, check release policy, migration needs, and downstream consumers.
6. Update tests and documentation where the behavior or contract changes. Prefer a regression test that demonstrates the defect or new behavior.

## Debug

When an unexpected failure appears, pause unrelated changes and preserve the exact command, error output, environment/version, inputs, and reproduction status. Then:

1. Reproduce with the project's actual commands or classify the failure as intermittent/non-reproducible.
2. Localize the failing layer (test, UI, API, backend, persistence, build, dependency/configuration, or external service).
3. Reduce to a small case and vary one relevant factor at a time.
4. Form a causal explanation, distinguish a product defect from an invalid/stale test or environment issue, then fix the underlying cause rather than hiding the symptom.
5. Add a focused regression check and rerun the original scenario, relevant tests, and appropriate broader gates.

For intermittent failures, preserve timing and environment evidence, inspect order, concurrency, shared state, and external dependencies, and communicate residual uncertainty. Keep temporary diagnostics only when they provide useful, privacy-safe operational evidence.

## Verify

Use project-native commands and report exactly what ran. Select checks according to scope and risk:

- Focused unit or component test for a local behavior change.
- Relevant integration/end-to-end or manual scenario for cross-component behavior.
- Type, lint, build, migration, schema, or contract checks when applicable.
- Browser readiness signals, observed controls, stable accessible selectors, and screenshots/DOM/logs for UI behavior when useful. Prefer event- or state-based waits to arbitrary delays or universal network-idle assumptions.
- Compatibility or regression checks for public, released, persisted, or externally consumed contracts.

Inspect failures rather than weakening or skipping a check to get a green result. Distinguish a check that was not run from one that passed.

## Review

Review the same final diff against two separate questions:

1. **Requirements and behavior:** Does the change implement the stated scope? Are requirements omitted, partly implemented, contradicted, or exceeded? Does visible behavior match the contract?
2. **Engineering quality:** Does the result fit repository conventions and avoid defects in correctness, security, privacy, performance, accessibility, reliability, maintainability, and compatibility relevant to this change?

Anchor each finding to a file/section and concrete evidence. State impact and confidence. Distinguish enforceable requirements from optional design preferences. Avoid treating a maintainability heuristic as an automatic violation. Before handoff, inspect the complete diff and remove accidental artifacts; report changed interfaces or operational consequences when material.
