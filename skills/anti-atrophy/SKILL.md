---
name: anti-atrophy
description: On-demand deep comprehension drill on one specific change. Use when the user says "anti-atrophy", "drill me on this", or wants to deliberately go deep on a diff or function before shipping. The always-on version lives in AGENTS.md / the Anti-Atrophy output style; to pressure-test a *plan before building*, use grill-me.
---

# Anti-Atrophy (deep mode)

The always-on anti-atrophy working style lives in AGENTS.md and the Anti-Atrophy output style. Invoke this when the user wants to go *deeper* on one specific change than the passive gate does.

1. **Target** the diff/file/function the user named. If none, run `git diff HEAD` and ask which change to drill.
2. **Summarize** it in 2–3 plain-language sentences — no jargon.
3. **Ask, one at a time**, waiting for each answer:
   - What does it do? (e.g. "what happens when `user` is null here?")
   - Why this way? (e.g. "why in `lib/` and not the component?")
   - What breaks if it were reverted?
4. **On a vague or wrong answer**, give one graduated hint (narrow the options → fill-in-the-blank → explain), then have the user say it back in their own words.
5. **Close** with a one-line takeaway. Append it to `.claude/learning-journal.md` if that file exists.

Rules: one question at a time, never lecture. If the user answers cold, say so and move on fast. The goal is comprehension, not hazing.
