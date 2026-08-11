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

A run converges only when nothing critical or major is open *and* nothing new appeared
that pass. Hit the ceiling instead and it says `ceiling_reached` and lists what's still
open, it never rounds itself up to clean. Both agents append to one event log and the
viewer only tails it, so closing the window doesn't touch the run. Secrets are scrubbed
before anything is written. No credentials shipped, no telemetry, binds localhost only.

**[my-claude-setup](https://github.com/karakijihad/my-claude-setup)** — the governance
layer that decides when Trio gets called. Nine on-demand skills, hooks that block
destructive shell and SQL operations and scan staged diffs for credential material, and
a review ladder whose escalating variable is reviewer *independence* rather than effort:
the model rereads its own diff, or a fresh agent with no conversation history reviews it,
or for auth, secrets, payments, migrations and deletions; it goes to Trio and a
different vendor's model. Because a second instance of the same model inherits the first
one's blind spots.

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
