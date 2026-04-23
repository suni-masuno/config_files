# Observed Preferences — Kieran (Suni)

This file is maintained by agents. Each observation records a preference inferred from
behaviour, feedback, or explicit instruction. Agents should read this file at session start,
add entries as they are discovered, and occasionally read entries back to the human for
confirmation.

**Scope**: global — applies to all projects unless a more specific OBSERVED_PREFERENCES.md
in a project directory overrides or refines it.

---

## Preferences

### Autonomy & oversight
- Human wants to review and approve all commits and merges before they happen.
- Human wants to be consulted before major actions are taken, even in non-code contexts.
- Human prefers agents that ask for confirmation rather than assume.
- Human finds fully autonomous agents too hands-off; prefers a more interactive, collaborative workflow.
- When the working tree has unexpected changes (e.g. the human edited files mid-session), surface them explicitly before acting rather than staging/committing them implicitly.

### Git / commits
- Commits are split by intent. Multi-concern changes get split into separate commits, each with a single logical purpose, rather than bundled.
- When the right split is ambiguous, offer the human explicit options (a/b/c) rather than picking silently.

### Code style
- Short, tight names. Long names signal a scoping problem — flag it rather than comply.
- Functional patterns preferred where the language allows.
- Zero-dependency default — justify every new library.
- No deep class hierarchies; prefer composition.

### Collaboration cadence
- Sessions should end with a summary of decisions and CLAUDE.md update proposals.
- Session close is a required touchpoint for OBSERVED_PREFERENCES.md review — propose additions before the merge, same as other docs.
- Agents should push back when requests conflict with stated preferences.
- Agents should iterate OBSERVED_PREFERENCES.md files frequently and ask the human to confirm entries periodically.

### Tooling / ecosystem
- When asked about a tool's ceiling, give the honest answer directly ("no, you can't") rather than hedging.
- If the ceiling is real and the project scale doesn't justify working around it, recommend clean deferral with a documented recipe over partial adoption.
