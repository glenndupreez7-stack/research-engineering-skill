# Source provenance

This original skill synthesizes workflow ideas from a curated review of public GitHub Agent Skills. The cited files were opened and the repositories' license files were inspected on **2026-10-11**. The `main` branch URLs are mutable; recheck current content, version, and license before reusing a specific implementation, example, or substantial expression.

The skill uses independently written instructions and does not bundle copied source files, code, examples, or templates. The list records topic coverage and provenance; it is not an exhaustive ranking of GitHub skills. Repository adoption and maintenance claims were not independently verified for this review and are intentionally not presented as facts.

## Reviewed sources

1. **Research workflow and evidence synthesis — `mattpocock/skills` (`research`)**
   - Source: [research/SKILL.md](https://github.com/mattpocock/skills/blob/main/skills/engineering/research/SKILL.md) · [raw file](https://raw.githubusercontent.com/mattpocock/skills/main/skills/engineering/research/SKILL.md)
   - Repository license: [LICENSE](https://github.com/mattpocock/skills/blob/main/LICENSE) — MIT.
   - Informed: primary-source-first research, claim-level support, repository-aware evidence artifacts, and separating investigation from synthesis.

2. **Source evaluation and fact verification — `addyosmani/agent-skills` (`source-driven-development`)**
   - Source: [source-driven-development/SKILL.md](https://github.com/addyosmani/agent-skills/blob/main/skills/source-driven-development/SKILL.md) · [raw file](https://raw.githubusercontent.com/addyosmani/agent-skills/main/skills/source-driven-development/SKILL.md)
   - Repository license: [LICENSE](https://github.com/addyosmani/agent-skills/blob/main/LICENSE) — MIT.
   - Informed: detect actual dependency versions, fetch focused official documentation, surface material conflicts, and verify source-backed decisions.

3. **Feature implementation and planning — `dzhng/skills` (`implement-spec`)**
   - Source: [implement-spec/SKILL.md](https://github.com/dzhng/skills/blob/main/skills/engineering/implement-spec/SKILL.md) · [raw file](https://raw.githubusercontent.com/dzhng/skills/main/skills/engineering/implement-spec/SKILL.md)
   - Repository license: [LICENSE](https://github.com/dzhng/skills/blob/main/LICENSE) — MIT.
   - Informed: bounded implementation passes, specification and handoff maintenance, dependency-aware collaboration, and final reconciliation.

4. **Systematic debugging — `addyosmani/agent-skills` (`debugging-and-error-recovery`)**
   - Source: [debugging-and-error-recovery/SKILL.md](https://github.com/addyosmani/agent-skills/blob/main/skills/debugging-and-error-recovery/SKILL.md) · [raw file](https://raw.githubusercontent.com/addyosmani/agent-skills/main/skills/debugging-and-error-recovery/SKILL.md)
   - Repository license: [LICENSE](https://github.com/addyosmani/agent-skills/blob/main/LICENSE) — MIT.
   - Informed: preserve failure evidence, reproduce and localize, reduce to a minimal case, identify cause, and verify a regression check.

5. **Testing and verification — `anthropics/skills` (`webapp-testing`)**
   - Source: [webapp-testing/SKILL.md](https://github.com/anthropics/skills/blob/main/skills/webapp-testing/SKILL.md) · [raw file](https://raw.githubusercontent.com/anthropics/skills/main/skills/webapp-testing/SKILL.md)
   - Skill license: [LICENSE.txt](https://raw.githubusercontent.com/anthropics/skills/main/skills/webapp-testing/LICENSE.txt) — Apache License 2.0.
   - Informed: observe rendered UI before interaction, select checks from the actual target, and preserve useful test evidence. The new skill avoids assuming network-idle is universally appropriate.

6. **Code review and maintainability — `mattpocock/skills` (`code-review`)**
   - Source: [code-review/SKILL.md](https://github.com/mattpocock/skills/blob/main/skills/engineering/code-review/SKILL.md) · [raw file](https://raw.githubusercontent.com/mattpocock/skills/main/skills/engineering/code-review/SKILL.md)
   - Repository license: [LICENSE](https://github.com/mattpocock/skills/blob/main/LICENSE) — MIT.
   - Informed: assess requirement fidelity separately from repository standards and maintainability heuristics; ground findings in specific evidence.

7. **Technical API writing — `wshobson/agents` (`openapi-spec-generation`)**
   - Source: [openapi-spec-generation/SKILL.md](https://github.com/wshobson/agents/blob/main/plugins/documentation-generation/skills/openapi-spec-generation/SKILL.md) · [raw file](https://raw.githubusercontent.com/wshobson/agents/main/plugins/documentation-generation/skills/openapi-spec-generation/SKILL.md)
   - Repository license: [LICENSE](https://github.com/wshobson/agents/blob/main/LICENSE) — MIT.
   - Informed: choose code-first/design-first/hybrid contract ownership, document realistic success and error behavior, and validate the contract against implementation.

8. **Context management and repository navigation — `muratcankoylan/Agent-Skills-for-Context-Engineering` (`filesystem-context`)**
   - Source: [filesystem-context/SKILL.md](https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering/blob/main/skills/filesystem-context/SKILL.md) · [raw file](https://raw.githubusercontent.com/muratcankoylan/Agent-Skills-for-Context-Engineering/main/skills/filesystem-context/SKILL.md)
   - Repository license: [LICENSE](https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering/blob/main/LICENSE) — MIT.
   - Informed: diagnose context failures, retrieve files in bounded slices, persist useful state, isolate collaboration, and clean stale artifacts.

## Licensing note

The reviewed repositories declare MIT licenses except for the reviewed Anthropic web-app testing skill, whose linked skill license is Apache 2.0. This skill is a new synthesis in original wording and includes links for attribution and provenance. Its repository license applies to this original package only; it does not relicense or grant rights to the cited projects, their marks, external documentation, or their dependencies. Review the relevant license before copying source expression, code, or bundled assets.
