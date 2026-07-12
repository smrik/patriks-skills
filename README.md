# Patrik's Claude Code Skills

Custom Claude Code skills for deliberate, comprehension-driven development. Solve the problem of shipping changes without fully understanding them — these skills enforce thinking checkpoints before code goes out.

## Skills

**anti-atrophy** — On-demand deep comprehension drill.

Triggers when you run `/anti-atrophy` before shipping a change. Walks you through: what the change does, why it's designed that way, what assumptions it makes, and what would break if reverted. Forces you to own the reasoning while the AI owns the syntax.

*Example:* You refactor a state-management function. Before merge, run `/anti-atrophy` to articulate why the new approach is safer than the old one — catching edge cases and design flaws before they ship.

## Output Styles

**Anti-Atrophy** — Gates non-trivial changes with comprehension checkpoints.

Use this as your default working style for careful, deliberate work. Claude will pause at key points (before shipping, before major refactors) and ask you to explain decisions, ensuring you stay in control while the AI handles the syntax.

*Example:* Enable this style when implementing a critical path (auth, payments, data pipeline). You get prompted: "What could go wrong here?" before each commit, surfacing risks early.

## Status

Active, in-progress. Focused on comprehension-driven workflows for high-confidence shipping.

## Screenshots

_TODO (Patrik): add screenshots here._
