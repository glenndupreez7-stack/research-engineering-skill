# Efficient workflow and context

Use this module for broad repositories, large tool output, long-running work, and collaboration.

## Navigate with bounded retrieval

- Discover repository structure with directory listings or file globs; search exact symbols and error text with text search; use semantic search when the question is conceptual. Combine methods when useful.
- Read only the relevant files and bounded sections first. Expand retrieval when evidence shows the initial slice is incomplete; avoid loading large unrelated files into working context.
- Inspect project conventions before adding plans, notes, tests, or generated output. Use existing locations and naming patterns.
- For changing technical references, find the exact versioned page or source file rather than reading a broad landing page.

## Persist only useful state

Persist intermediate state when work spans turns, the evidence set is large, another worker must continue, or reproducibility/auditability matters. Keep short tasks in the active context.

When persistence is useful:

- Separate final deliverables, durable evidence, plans, and disposable scratch output.
- Use a run-scoped, unique path and a clear format. Keep a short summary plus pointers to larger raw output.
- Record the objective, acceptance criteria, current status, decisions, sources, checks, blockers, and next action at meaningful checkpoints.
- Before reusing a stored path, verify it exists and still refers to the expected artifact. Read large files in bounded sections.
- Redact credentials, tokens, personal information, and unrelated private data before storing or passing material to collaborators. Apply suitable access and retention limits.
- Clean temporary artifacts after use while preserving material needed to reproduce or audit the result.

## Delegate and integrate

Delegate only work that is meaningfully independent and whose coordination cost is justified. Keep tasks narrowly scoped with an explicit question, evidence standard, output schema, and unique file ownership. Prefer isolated workspaces for independent modifications; avoid shared writes unless synchronized. For deterministic bulk processing, use one bounded script rather than many research agents.

The coordinator remains responsible for checking delegated outputs, integrating changes, resolving conflicts, and rerunning relevant checks after integration. If delegation, a preferred search tool, or a file capability is unavailable, use a serial or manual fallback and report any resulting limitation.

## Avoid waste

Prefer readiness signals and bounded targeted waits to arbitrary sleeps. Save large logs or pages only if they will be searched or reused; summarize them and retain retrieval pointers. Reassess a plan when scope, evidence, dependencies, or risk changes. Use cleanup checkpoints to remove stale notes, duplicate summaries, and obsolete temporary scaffolding.
