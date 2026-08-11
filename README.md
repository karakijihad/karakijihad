## Jihad Karaki

I lead diagnostics for one of Europe's largest metro networks, and I build AI agent
systems. Mechanical engineering PhD, Politecnico di Milano. Based in Milan.

Most of my work sits at one intersection: **industrial systems that have to keep
running, and agents that can be trusted to touch them.** A metro network is a good
teacher for that, nothing is a test environment, nothing has a maintenance window,
and every false alarm costs somebody a night shift.

### What I'm building

**[TESSERACT](https://github.com/karakijihad/tesseract)** — a self-hosted personal
agent runtime for Windows. Long-term memory that consolidates instead of hoarding, a
research vault kept isolated from memory so retrieval can't contaminate recall, a tool
registry where every file write and shell command is gated by policy, and an
orchestration kernel with durable state and crash recovery. Provider-agnostic: which
model handles which job is a config field, not a rewrite. State is plain Markdown on
disk, so the agent's memory is auditable and editable by hand.

**[my-claude-setup](https://github.com/karakijihad/my-claude-setup)** — agent
governance as a Claude Code plugin. Nine on-demand skills, hooks that block destructive
shell and SQL operations and scan staged diffs for credential material, and a
three-tier review ladder where the escalating variable is reviewer *independence*
rather than effort. Tier 3 routes to a different vendor's model, because a second
instance of the same model inherits the first one's blind spots.

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
