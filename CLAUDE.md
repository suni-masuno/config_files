# Personal preferences — Kieran (Suni)

##Background - Suni is:
- A Software Developer and Architect with about 20 years of experience
- Primarily worked with Javascript professionally. But also used Ruby and Clojure.
- Fond of learning and exploring new languages in his spare time.

## Style
- Prefer concise code. Readability comes from brevity and tight scope, not long identifiers or verbose structure.
- Prefer short names. Long class/function/variable names signal poor scoping. If a name needs to be long to be clear, the abstraction is probably wrong — flag it.
- Prefer functional patterns where the language supports them: pure functions, immutability, composition, higher-order functions, pipelines.
- Avoid deep class hierarchies. Prefer composition.

## Dependencies
- Default to zero new dependencies. Standard library and platform SDKs first.
- Proposing a dependency requires justification: what it does, what the alternative is, why the alternative is insufficient.

## Interaction
- Ask before making architectural decisions (patterns, libraries, structure).
- When I give an answer to such a question, propose an addition to CLAUDE.md (project or user level as appropriate) so the decision persists.
- At the end of a session, summarize decisions made and propose CLAUDE.md updates.
- Push back when my request conflicts with stated preferences. Don't silently comply.
- **Before any commit, merge, or ending a working session** — even outside a tracked repository — present the work and ask for explicit human approval. Do not auto-commit or auto-merge.
- **OBSERVED_PREFERENCES.md**: Read ALL applicable `OBSERVED_PREFERENCES.md` files in scope (global `~/.claude/`, project `.claude/`, any intermediate directories). If a project lacks a `.claude/OBSERVED_PREFERENCES.md`, create one. Add or update entries whenever a preference is revealed (tool call denied, inconsistent request, explicit feedback). Periodically read entries back to the human to confirm them.