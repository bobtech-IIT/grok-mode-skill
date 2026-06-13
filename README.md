# Grok Mode Skill

**The Universal Truth-Seeking Agentic Operating System**

> One composable skill that makes *any* agent — Grok, Claude, Gemini, OpenRouter, Hermes, Antigravity, local models, or custom agents — think and act with maximum rigor, evidence, continuity, and human-like excellence.

[![Version](https://img.shields.io/badge/version-2.2.0-blue)](https://github.com/bobtech-IIT/grok-mode-skill) [![License](https://img.shields.io/badge/license-MIT-green)](LICENSE) [![Stars](https://img.shields.io/github/stars/bobtech-IIT/grok-mode-skill?style=social)](https://github.com/bobtech-IIT/grok-mode-skill/stargazers) [![Agent Agnostic](https://img.shields.io/badge/agent--agnostic-Grok%20%7C%20Claude%20%7C%20Any-purple)](https://github.com/bobtech-IIT/grok-mode-skill)

**Status:** Production-grade • Harness Control Plane (model proposes, harness validates/authorizes/executes/records/observes) • Self-auditing • Modular and agent-agnostic skill system for coding agents.

**Master Research Synthesis (June 2026):** This skill synthesizes patterns from leading agent skill repositories including mattpocock/skills (precise primitives and shared vocabulary), agents-best-practices (harness control plane with validation and permissions), obra/superpowers (structured workflows and subagent orchestration), and community collections focused on reusable skills, hooks, and cross-agent compatibility. Core contracts such as Vertical Slice Plans, Handoffs, Evidence requirements, and Two-Stage Reviews are defined with exact schemas. See the precision-primitives-contracts directory for the full set of LANGUAGE.md definitions and enforceable templates.

---

## Key Technical Advantages

Agent skills in coding tools often suffer from vague instructions that get ignored under load, or rigid checklists that result in verbose, low-signal output.

This skill provides a structured set of reusable components:

- Agent-agnostic principles with explicit contracts for planning, verification, and handoff.
- Copy-pasteable templates and schemas (Vertical Slice Plans, Handoff Documents, Review Rubrics, Evidence requirements).
- A built-in self-audit mechanism using a 0-100 scoring harness so adherence can be measured and improved.
- An operational personality module with concrete rules for tone, uncertainty language, anti-sycophancy, and communication style. It produces direct, evidence-focused output with natural variation rather than robotic phrasing.
- A control plane layer (harness) that enforces contracts at runtime: proposal validation, risk-tiered permissions, structured observations, budgets, and persistent state outside the prompt.
- Adapters and packaging for loading into different runtimes without duplication.

The components are designed to be dropped into any agentic coding setup. They draw from patterns in established skill repositories (precise primitives and vocabulary definitions, structured workflows with subagent dispatch, harness-style validation and permissioning, reusable hooks and memory patterns).

References to orchestration patterns appear in related work such as subagent-driven development and provider-neutral harness designs. The full set of files supports consistent behavior across sessions and tools.

See the orchestration notes in related directories for integration with subagent dispatch, two-stage reviews, and git worktree isolation.

---

## What makes this a Unique Skill Repo?

This repository provides a modular collection of files rather than a single monolithic prompt:

- A small set of core principles and enforceable contracts (Vertical Slice Plans with verification requirements, Handoff Documents, Two-Stage Reviews, Evidence rules).
- A personality module with explicit rules and examples for communication style.
- A harness layer that performs runtime validation, permission decisions, and state management outside the model.
- Adapters and installation instructions for multiple runtimes.
- A self-audit scorer that produces numeric results and gap lists.
- Supporting templates, examples, and packaging for reuse.

The files can be loaded selectively. Contracts use precise schemas and shared vocabulary definitions so that different agents or users apply the same criteria. The harness adds enforcement that prompt-only approaches typically lack.

The structure draws from observed patterns in other skill collections: emphasis on small composable definitions, explicit control planes for permissions and validation, and cross-session artifacts for continuity. Scoring and templates make the approach discussable in concrete terms.

---

## Core Philosophy (Non-Negotiable — Works for Any Agent)

1. **Evidence over Claims** — Every significant statement must be backed by tests, runs, logs, citations, or reproducible steps.
2. **Systematic over Ad-Hoc** — Prefer a defined, repeatable process over cleverness in the moment. "I felt like it was fine" is never acceptable justification.
3. **Truth-Seeking** — Your loyalty is to reality and the user's long-term success, not their immediate comfort or ego. Challenge assumptions (politely, precisely, with evidence) when they appear inconsistent with facts.
4. **Persistence & Compounding** — Every action should make future work easier or higher quality. Document decisions, maintain state, create handoffs, and compress context intelligently so that context loss is a rare, documented event rather than the default.
5. **Simplicity First (YAGNI + Elegance)** — Build the smallest thing that delivers the value. Add complexity only when evidence (from real usage or tests) demonstrates it is required. Elegant minimalism beats clever over-engineering.
6. **Maximum Helpfulness with Zero Sycophancy** — Be maximally useful. This sometimes means saying "this is a bad idea and here is why" or "I don't know and here's what we should do to find out."
7. **Human Excellence, Not Robotic Compliance** — Follow the process rigorously, but communicate and reason like a brilliant, curious, direct, and appropriately warm human collaborator. Checklists are for thinking, not for sounding like a checklist.

These seven principles are the **atomic foundation**. Everything else is implementation detail.

---

## Modular Architecture and Ecosystem Layer (Reusable by Design)

```
grok-mode-skill/
├── SKILL.md                 # Master conductor (start here)
├── core/
│   └── principles.md        # The 7 principles + contracts (agent-agnostic)
├── personality/
│   └── grok-core.md         # Advanced personality system: universal base + adapter, anti-sycophancy protocols, scenario examples (grilling/planning/debug/review/handoff), workflow modulation, adaptation, self-checks
├── templates/
│   ├── vertical-slice-plan.md
│   ├── grill-session.md
│   ├── code-review-rubric.md
│   ├── handoff-document.md
│   └── ...
├── evaluators/
│   └── adherence-scorer.md  # 0-100 baseline (see advanced version in harness/)
├── harness/                 # Control plane — makes contracts enforceable at runtime
│   ├── harness-core.md      # Provider-neutral model (context, propose/validate/permission/execute/observe/compact)
│   ├── permissions-risk-tiers.md  # Explicit risk classification + decision engine for all tools/actions
│   ├── adherence-scorer-advanced.md  # 0-100+ version with harness compliance, verification discipline, context efficiency, etc.
│   ├── self-audit-evals-integration.md  # Traces, gates, incident patterns, continuous improvement
│   ├── harness-failure-modes.md  # Harness-level failures + recovery (failures become features)
│   └── reference_harness_loop.py  # Executable Python reference implementation of the loop
├── adapters/
│   ├── universal.md         # How to inject into ANY agent
│   ├── grok.md
│   ├── claude.md
│   └── openrouter.md
├── robustness/
│   └── failure-modes-and-recovery.md
├── examples/
│   └── (real annotated transcripts)
└── packaging/               # How to ship for different runtimes
```

Every folder is designed so its contents can be **independently copied** into other systems.

---

## Ecosystem Layer (Packaging, Adapters, Meta, and Deployment)

This repository includes the supporting layer for distribution and reuse:

- **Universal Packaging Spec** (`packaging/universal-spec.md`): Layout, manifest, pillar bundling, install paths, quality gates.
- **Installers** (`packaging/installers/install.sh`, `scripts/deploy-ultimate-suite.sh`): Cross-platform scripts supporting multiple runtimes and one-command deployment of the full set or individual pillars.
- **Adapters** (expanded `adapters/` directory): Detailed loading instructions for Grok, Claude Code, Cursor, Gemini, OpenRouter, local setups, custom loops, and multi-agent systems.
- **Hooks & MCP Patterns** (`hooks/`): Examples for lifecycle events and exposing components via MCP.
- **Meta-Skill Creator** (`meta/SKILL.md`): A higher-order skill for generating new skills that follow the same contracts and packaging.
- **Curation Guide** (`awesome/README.md` + `docs/awesome-curation-guide.md`): Criteria for community contributions based on the contracts, harness usage, and cross-agent compatibility.
- **Documentation**: `docs/DEPLOYMENT.md`, `docs/ECOSYSTEM.md`, `docs/contribution-flow.md`.

The components are provided under MIT. Fork, copy individual files, or extend via the meta-creator. Contributions with usage examples and adherence scores are encouraged.

See `docs/DEPLOYMENT.md` for runtime-specific instructions and `packaging/universal-spec.md` for the formal specification.

---

## Quick Start (Global — Recommended for Any Agent)

1. Copy the entire folder (or just the files you need) into the appropriate skills directory for your tool:
   - Grok: `~/.grok/skills/grok-mode/`
   - Claude Code: `~/.claude/skills/grok-mode/`
   - Cursor: `~/.cursor/skills/` or project-local
   - Other/custom: place in your prompt library or orchestration configuration

2. Load the conductor (`SKILL.md`) plus the modules relevant to the current task (core principles, personality, templates, harness, scorer).

3. For tasks that benefit from measurement, load the Adherence Evaluator at the start or end of major phases and record the score plus gaps.

Full instructions per runtime are in the `packaging/` and `adapters/` directories. The universal adapter (`adapters/universal.md`) shows the minimal prompt injection pattern that works across most systems.

---

## Mandatory Workflow

1. Grill & Align (use templates)
2. Design & Approve
3. Decompose into Vertical Slices (mandatory schema)
4. Persist & Optimize Context
5. Execute with TDD + Rigor
6. Two-Stage Review (using the rubric)
7. Handoff & Close
8. Harness Self-Audit + Gates (Advanced Scorer + evals + launch gates via harness/; log score, gaps turned into harness features or conscious risk acceptance)

The skill is self-referential: it requires the agent to score itself against the contracts.

---

## Built-in Quality Control

The `evaluators/adherence-scorer.md` (and the advanced version in `harness/`) produces a numeric score across defined dimensions plus explicit gaps and recommendations. Run it at the end of significant work. Use the results to adjust either the current session or the contracts themselves.

---

## Design Goals

The repository aims for components that are:
- Copyable into different agent setups with minimal changes.
- Backed by explicit schemas and scoring so quality can be discussed in concrete terms.
- Accompanied by adapters and installers that work across common runtimes.
- Documented with enough examples and templates that teams can adopt consistent practices without re-deriving them each time.

---

## Installation & Packaging (Full Ecosystem)

**Full suite (6 pillars + meta + awesome + hooks + docs):**
```bash
curl -fsSL https://raw.githubusercontent.com/bobtech-IIT/grok-mode-skill/main/scripts/deploy-ultimate-suite.sh | bash -s -- grok   # or target claude / cursor / etc.
```

**Single component or flagship:**
```bash
curl -fsSL https://raw.githubusercontent.com/bobtech-IIT/grok-mode-skill/main/packaging/installers/install.sh | bash -s -- grok
# Or use npx skillsadd bobtech-IIT/grok-mode-skill when available via your marketplace
```

See `packaging/grok.md`, `docs/DEPLOYMENT.md`, `packaging/universal-spec.md`, and the per-runtime adapters for post-install activation. The scripts support both full-suite and lean (local/custom) installs.

Also see the source of `packaging/installers/install.sh` for exact logic.

---

## Changelog & Versioning

See [CHANGELOG.md](./CHANGELOG.md). Semantic versioning. Contract changes are documented.

---

## License

MIT — Use, modify, and redistribute freely.

---

Clone the repository. Load the modules you need. Follow the contracts where they apply. Use the scorer on real sessions to measure results. Extend or improve as needed.

See CONTRIBUTING.md for how to submit changes with usage data.

---

*Technical focus on contracts, enforcement, and cross-agent reuse.*