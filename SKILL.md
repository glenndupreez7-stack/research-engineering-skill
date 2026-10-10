---
name: research-engineering-skill
description: Integrated workflows for evidence-led technical research, efficient software engineering, and technical writing. Use when investigating technical questions, implementing, debugging or reviewing code, or creating and maintaining specifications, API references, and engineering documentation—especially when facts, requirements, tests, and citations must stay aligned.
---

# Research Engineering

Use this skill to complete technical work from context discovery through evidence, execution, verification, and handoff. Adapt the depth to the task; do not add ceremony that does not reduce uncertainty or risk.

## Choose a workflow depth

- **Quick:** A narrow, familiar, low-impact change. Inspect relevant context, make the change, run the most relevant check, and report what was verified.
- **Standard:** A multi-file or uncertain task. Inspect project guidance and versions, define acceptance criteria, keep a short plan and evidence notes, then verify the result.
- **Deep:** A broad investigation, long-running feature, public contract, migration, or high-impact decision. Break it into bounded work units, preserve a traceable evidence record, resolve material conflicts, and run layered verification. Delegate only genuinely independent work when a suitable mechanism exists; retain one integration owner.

Choose the smallest depth that can establish a dependable result. Increase depth when uncertainty, external impact, compatibility, security, or failure cost rises.

## Shared workflow

1. **Frame the task.** Identify the question or artifact, intended audience, scope boundaries, success conditions, freshness or version needs, and explicit user constraints. Ask only when a missing choice would materially change the result. Otherwise use a reversible, clearly stated assumption.
2. **Inspect reality.** For repository work, locate project instructions, the relevant specification or issue, manifests and runtime versions, current changes, tests, and the existing contract. For research, identify what evidence would answer the question. For writing, locate the source of truth and audience.
3. **Plan bounded work.** List the next concrete actions and their exit checks. Split work by independent outcomes, not arbitrary file count. Keep scope and acceptance criteria visible as evidence changes.
4. **Execute with evidence.** Use authoritative, version-appropriate sources for technical claims and project-local conventions for implementation. Distinguish what was observed from what was inferred or assumed. Preserve decision-relevant evidence when work spans turns or tools.
5. **Verify the outcome.** Match checks to the task: source inspection, targeted tests, broader tests, build/type checks, contract validation, controlled experiments, or observed UI behavior. Do not describe a check as passed if it was not run.
6. **Reconcile and hand off.** Compare the final artifact to the request and acceptance conditions. Remove accidental scratch output, update durable documentation when needed, identify unresolved uncertainty, and summarize the result and evidence.

## Keep kinds of information distinct

When distinctions matter, label and separate:

- **Verified facts:** Directly supported by a cited authoritative source, reproduced behavior, or a completed check.
- **Observations:** What a file, command, test, page, or system visibly showed, with its context.
- **Inferences:** Conclusions drawn from evidence; state the reasoning briefly.
- **Assumptions:** Temporary choices made because information was unavailable; say how they affect the result.
- **Recommendations:** Proposed actions, separated from established facts.
- **Open questions:** Material points that remain unknown or need a user decision.

Attach evidence to the claim it supports. For technical research, cite a source close to the relevant statement and record its version or access context when that could affect correctness. Never turn an unverified behavior into a fact through confident wording.

## Route to the relevant module

- **Investigating a question or comparing technical claims:** Follow [Research and evidence](references/research.md).
- **Changing, debugging, testing, or reviewing software:** Follow [Software engineering](references/engineering.md).
- **Writing specifications, API references, or engineering docs:** Follow [Technical writing](references/technical-writing.md).
- **Long tasks, large outputs, repository navigation, or parallel work:** Use [Efficient workflow and context](references/efficient-workflow.md).
- **Source selection and provenance for this skill:** See [Source provenance](references/source-provenance.md).

Use only the relevant modules. Combine them when a task crosses boundaries—for example, research an API, implement against it, test the behavior, and update its reference documentation.

## Completion standard

A task is ready to hand back when its requested deliverable exists, material acceptance conditions have been checked, evidence and uncertainty are accurately represented, and the user can see what changed and what remains. For short tasks, communicate this in a few sentences; use structured sections only when they improve clarity.

**Any unneeded directories can be deleted.** Not every skill requires all three types of resources.
