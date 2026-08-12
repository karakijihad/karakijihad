## Jihad Karaki

I lead diagnostics for one of Europe's largest metro networks, and I build AI agent
systems. Mechanical engineering PhD, Politecnico di Milano. Based in Milan.

Most of my work sits at one intersection: **industrial systems that have to keep
running, and agents that can be trusted to touch them.** A metro network is a good
teacher for that, nothing is a test environment, nothing has a maintenance window,
and every false alarm costs somebody a night shift.

### What I'm building

**[Trio](https://github.com/karakijihad/trio-cc)** — Claude and Codex reviewing each
other's work. A model is a poor reviewer of its own code and a good reviewer of somebody
else's, so Trio runs OpenAI's Codex as a strictly read-only reviewer, `--sandbox
read-only` hardcoded, not a setting; through five perspectives in parallel: defects,
security, tests, duplication, and drift between what things claim and what they do.
Claude then rules on every finding: confirm, refute, downgrade, escalate. Refuting one
means citing the code that disproves it, because a confident model is not evidence.

**[my-claude-setup](https://github.com/karakijihad/my-claude-setup)** — a standing
operating discipline for Claude Code. Install it once and every repo you open gets the
same rules: minimum-code discipline, a confirm-first threshold, a fast path for small
work, a plan when the work is phased enough to earn one, and a mandatory independent
review at the end of anything that modifies code. Seven protocol references covering security, 
testing, Git, delegation, feedback, planning, and documentation. Loaded on demand rather than 
remaining permanently in context. Nine skills, three hooks, and three commands.

**[trio-cc](https://github.com/karakijihad/trio-cc)** — drives OpenAI's Codex as a
read-only auditor over Claude-authored changes, with each finding adjudicated rather
than auto-applied.

**SIGDX** — a condition-monitoring dashboard for metro infrastructure, built solo.
Public September 2026, once contractual obligations clear.

**[ProLifter](https://docs.prolifter.app/)** — competition-management software for
strength sports (C#, Unity). Commercial, running, paying for itself.

### Elsewhere

- I write at [blog.metaengineershub.com](https://blog.metaengineershub.com/)
- Inventor on a filed railway diagnostics patent (IT 102025000030238).
- Papers on rail corrugation monitoring and vibration propagation:
  [Applied Sciences 2023](https://doi.org/10.3390/app13063773),
  [Springer 2022](https://doi.org/10.1007/978-3-031-07305-2_17).
- Off the keyboard: jiu-jitsu, and I coach strength & conditioning.
