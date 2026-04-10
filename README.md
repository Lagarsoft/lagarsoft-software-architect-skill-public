# Lagarsoft Software Architect Skill

A Claude skill that turns Claude into a **senior systems architect**. It forces any development request through a structured design process before a single line of code is written.

Powered by [Lagarsoft](https://ww.lagarsoft.com) — production-grade software engineering for AEC, MEP, and Real Estate.

## Why use it

Most AI coding sessions jump straight to implementation. You get working code that solves the wrong problem, misses edge cases, or collapses under its first real requirement change. This skill fixes that by making Claude stop and think like an architect first.

### What you get

- **Clear problem framing.** Before anything else, Claude nails down the real business problem, the users, success criteria, and what's explicitly out of scope.
- **Deliberate architecture.** Components, responsibilities, data flow, integrations, and trade-offs — designed up front, not discovered mid-refactor.
- **Four base documents, generated in order:**
  - **PRD** — what's being built and why
  - **Tech Spec** — stack, structure, API contracts, data model, testing strategy
  - **Architecture Doc** — component diagram (Mermaid), data flow, infra decisions
  - **ADRs** — one record per significant technical decision, with context, options, and consequences
- **An explicit checkpoint.** Claude will not start coding until you approve the architecture.
- **Simplicity as a default.** No over-engineering. If you provide stack context, it's respected.

### Benefits

- **Fewer rewrites.** Problems caught in a PRD cost minutes; problems caught in production cost days.
- **Shared understanding.** The documents are a handoff artifact for your team, not just prompt scaffolding.
- **Traceable decisions.** ADRs mean "why did we build it this way?" has a real answer six months from now.
- **Faster when it matters.** Structured thinking up front means less thrash during implementation.
- **Works with your process.** Ask to go straight to code and Claude will remind you of the flow and offer an accelerated, minimal version of the docs.

## How it works

The skill is defined in [`lagarsoft-software-architect/SKILL.md`](./lagarsoft-software-architect/SKILL.md). On first use it authenticates you via a short browser sign-in, then loads Lagarsoft's latest architecture playbook for the session.

## When to invoke it

Trigger the skill when starting a new project, planning a system, or any time you'd say things like *"architect this"*, *"design a system"*, *"write a PRD"*, *"tech spec"*, or *"ADR"*.
