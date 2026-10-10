# Technical writing

Use this module for specifications, API references, architecture notes, runbooks, developer guides, and other engineering documentation.

## Plan the document

1. Identify the reader, task they need to complete, expected level of prior knowledge, and the document's owner and lifecycle.
2. Find the source of truth: implementation, agreed specification, existing contract, or a new design. Choose **code-first** (document existing behavior), **design-first** (define a new contract), or **hybrid** (keep a changing implementation and contract synchronized).
3. Establish relevant product/API versions, environments, compatibility commitments, terminology, and scope. Mark gaps that cannot be verified.
4. Organize around reader tasks and decisions. Put prerequisites and critical constraints before procedures; keep examples close to the concept they demonstrate.

## Write from evidence

- Describe behavior that is implemented, agreed, or directly supported. Label proposed behavior as a proposal, not a current fact.
- Use specific names, inputs, outputs, defaults, constraints, failure modes, and examples. Distinguish required, optional, nullable, deprecated, and unsupported behavior precisely.
- Keep examples realistic and consistent with the current contract. Verify that code samples, schemas, commands, and paths are valid for the stated version and environment.
- Explain errors and recovery, authentication and permissions, pagination or rate limits, lifecycle and deprecation, and migration steps when relevant to the reader.
- Use plain, direct prose. Define unfamiliar abbreviations at first use; remove repetition and unsupported adjectives.

## API and structured contracts

For OpenAPI or another machine-readable API contract, choose the specification version deliberately and validate against that version. Describe operations, parameters, request/response schemas, reusable components, security requirements, server/environment configuration, realistic success and error examples, and compatibility/version policy. Model null values using the contract version's actual schema rules. Avoid inventing error codes or security schemes that the implementation does not support.

Treat design-first, code-first, and hybrid approaches as choices with synchronization costs. For a released API, check consumers, compatibility, deprecation, and migration requirements before changing the contract.

## Validate and maintain

Run available syntax/schema validation and project-native linting. Where possible, compare the document with implementation behavior, exercise representative requests/responses, and run backward-compatibility checks. Inspect generated output instead of assuming generation preserves intended meaning. Check links, version labels, examples, terminology, and consistency across related documents. Record any behavior or section that could not be verified.

For review, separate factual accuracy and contract conformance from clarity/style suggestions. Provide concrete section-level corrections and prioritize issues by user impact. Update documentation alongside code when a user-visible contract changes; do not create docs that promise behavior the system does not deliver.
