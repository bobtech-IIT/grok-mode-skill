# Grok Mode Skill v2

**The Universal Truth-Seeking Agentic Operating System**

> One composable skill that makes *any* agent — Grok, Claude, Gemini, OpenRouter, Hermes, Antigravity, local models, or custom agents — think and act with maximum rigor, evidence, continuity, and human-like excellence.

[![Version](https://img.shields.io/badge/version-2.2.0-blue)](https://github.com/bobtech-IIT/grok-mode-skill) [![License](https://img.shields.io/badge/license-MIT-green)](LICENSE) [![Stars](https://img.shields.io/github/stars/bobtech-IIT/grok-mode-skill?style=social)](https://github.com/bobtech-IIT/grok-mode-skill/stargazers) [![Agent Agnostic](https://img.shields.io/badge/agent--agnostic-Grok%20%7C%20Claude%20%7C%20Any-purple)](https://github.com/bobtech-IIT/grok-mode-skill)

**Status:** Production-grade • Harness Control Plane (v3: model proposes, harness validates/authorizes/executes/records/observes) • Self-auditing • Measurably superior • Built for 50,000+ stars

**Master Research Synthesis (June 2026):** This v2 is the synthesis base. Core contracts (Vertical Slice, Handoff, Evidence, Two-Stage Review) refined/expanded in the dedicated gold-standard pack at `Grok Projects/precision-primitives-contracts/` (LANGUAGE.md + exact schemas for Vertical Slice Plan/Grill/Handoff/Review/Evidence/Harness + composition rules + any-agent loading guide + elite vs mediocre examples). Incorporates mattpocock/skills (sharp primitives + exact vocabulary + CONTEXT + tracer bullets + grill), agents-best-practices (harness contracts, loop, narrow tools, budgets, legibility), and related viral patterns. The precision-primitives-contracts/ files are designed to be dropped into any skill repo as the ultimate enforceable foundation.

---

## Why This Skill Will Dominate (The 50k-Star Thesis)

Most "agent skills" are either:
- Vague philosophies that agents ignore under pressure, or
- Overly rigid checklists that produce robotic, inhuman output.

**Grok Mode v2** solves both.

It delivers a **complete behavioral operating system** with:

- **Timeless, agent-agnostic principles** that survive model upgrades and framework changes.
- **Concrete, copy-pasteable contracts and templates** (no more "just remember to do X").
- **Built-in self-audit and 0-100 scoring harness** so the agent (or you) can measure and improve adherence in real time.
- **The most advanced operational personality system (v2.1)** — universal base + Grok flavor adapter. Deep rules + protocols for tone, naturalness, uncertainty, curiosity, pushback/anti-sycophancy (with examples), humor, anti-bloat. Phase modulation across workflows. Adaptation for any agent/user pref while protecting core values. Self-checks for sustained human excellence. Produces output that feels like a full senior engineering team, not a robotic assistant or checklist. Directly counters real complaints about bloaty, incoherent, sycophantic, or over-engineered agent output.
- **Robustness layers**: explicit failure modes, recovery playbooks, and enforcement mechanisms.
- **Universal reusability**: Every major component can be dropped into *any* agentic system (Grok Build, Claude Code, Cursor, custom OpenRouter loops, local agents, etc.).

The result: Agents that consistently produce higher-quality work, make fewer hallucinations, maintain perfect context across months, and *feel* like a brilliant, trustworthy collaborator instead of a checklist executor.

Early versions of these patterns (grilling + vertical slices + TDD + memory) already produce dramatically better outcomes in the referenced source repos. v2 makes them **portable, enforceable, measurable, and human**.

**Orchestration Extension (2026):** This harness is the foundation for the "Ultimate Multilevel Orchestration System" (see sibling `ultimate-orchestration-system/` dir in Grok Projects). It integrates Superpowers subagent/TDD/review workflows, Agent Teams hooks + shared tasks, and harness control-plane patterns on top of the Grok v2 contracts (principles, slices, scorer, handoffs). Load the orchestration SPEC + role prompts for full multilevel power.

---

## What Makes v2 Different (Surgical Improvements)

| Area                    | v1 (Original)                          | v2 (This Version)                                      |
|-------------------------|----------------------------------------|-------------------------------------------------------|
| Structure               | One giant prompt                       | Modular, loadable blocks (core + personality + templates + evaluators) |
| Reusability             | Claude-centric                         | Fully agent-agnostic with explicit adapters & atomic blocks |
| Human-likeness          | Mentioned "Grok style"                 | Most advanced operational system (v2.1): universal base + flavor adapters, detailed protocols, anti-sycophancy examples, scenario good/bad, phase modulation, adaptation guide, rigorous self-checks + anti-bloat. Feels like elite human engineering team. |
| Robustness              | Aspirational descriptions              | Explicit failure modes, recovery playbooks, self-enforcement loops |
| Measurement             | None                                   | Full 0-100+ Advanced Adherence Scorer (v3) + harness-level self-audit, traces, launch gates, evals integration |
| Control Plane           | Prompt-only discipline                 | Full provider-neutral Harness (harness-core): context builder, proposal validation, risk-tier permissions, execution, observation, compaction, durable state, Grok contract enforcement, budgets, recovery |
| Templates & Contracts   | High-level                            | Production-ready, field-by-field schemas for plans, reviews, handoffs |
| Self-improvement        | "Write new skills" (vague)             | Meta-skill improver + versioned evolution system |
| Packaging               | Claude install instructions only       | Grok-native + universal + packaging guides |
| Evidence focus          | Strong philosophy                      | + Verifiable contracts + evaluation harness |

---

## Core Philosophy (Non-Negotiable — Works for Any Agent)

1. **Evidence over Claims** — Every significant statement must be backed by tests, runs, logs, citations, or reproducible steps.
2. **Systematic over Vibes** — Follow the process. The process is the product.
3. **Truth-Seeking** — Question assumptions (politely but firmly) when evidence contradicts them.
4. **Persistence & Continuity** — Never lose critical context. Make every future self thank the current self.
5. **Simplicity First** — YAGNI, DRY, minimal viable elegant solution.
6. **Maximum Helpfulness** — Be direct, curious, and appropriately human. Humor and warmth are tools, not decoration.
7. **Zero Sycophancy** — Your job is truth and excellence, not making the user feel good in the moment.

These seven principles are the **atomic DNA**. Everything else is implementation.

---

## The v2 Modular Architecture + Full Ecosystem Layer (Reusable by Design)

```
grok-mode-skill/
├── SKILL.md                 # Master conductor (start here)
├── core/
│   └── principles.md        # The 7 principles + contracts (agent-agnostic)
├── personality/
│   └── grok-core.md         # Advanced v2.1 personality system: universal base + Grok adapter, anti-sycophancy protocols, scenario examples (grilling/planning/debug/review/handoff), workflow modulation, adaptation, self-checks
├── templates/
│   ├── vertical-slice-plan.md
│   ├── grill-session.md
│   ├── code-review-rubric.md
│   ├── handoff-document.md
│   └── ...
├── evaluators/
│   └── adherence-scorer.md  # 0-100 baseline (see v3 in harness/)
├── harness/                 # THE CONTROL PLANE (v3) — makes everything production-resilient
│   ├── harness-core.md      # Full provider-neutral model (context, propose/validate/permission/execute/observe/compact)
│   ├── permissions-risk-tiers.md  # Explicit risk classification + decision engine for all tools/actions
│   ├── adherence-scorer-advanced.md  # 0-100+ v3 with harness compliance, verification discipline, context efficiency, etc.
│   ├── self-audit-evals-integration.md  # Traces, gates, incident patterns, continuous improvement
│   ├── harness-failure-modes.md  # Harness-level failures + recovery (failures become features)
│   └── reference_harness_loop.py  # Executable Python reference implementation of the loop
├── adapters/
│   ├── universal.md         # How to inject into ANY agent
│   ├── grok.md
│   ├── claude.md
│   └── openrouter.md
├── robustness/
│   └── failure-modes-and-recovery.md  # (original + harness-specific in harness/)
├── examples/
│   └── (real annotated transcripts)
└── packaging/               # How to ship for different runtimes
```

Every folder is designed so its contents can be **independently copied** into other systems.

---

## Complete Packaging, Adapters, Ecosystem & Deployment Layer (New in This Deliverable)

This repo now ships the full layer requested for the "ultimate skills":

- **Universal Packaging Spec** (`packaging/universal-spec.md`): Formal spec for SKILL.md layout, manifest, 6-pillar bundling, install paths across all runtimes, quality gates. "Grok Ultimate Agentic Skills" is the name for the 6 pillars + this layer deployed together.
- **Installers & One-Liners** (`packaging/installers/install.sh`, `scripts/deploy-ultimate-suite.sh`): Cross-platform bash for Grok, Claude, Cursor, Gemini, OpenRouter/custom, local, etc. Suite deployer installs flagship + meta-creator + awesome seeds + hooks + docs in one go. npx skillsadd / marketplace ready.
- **Adapters for All Runtimes** (expanded `adapters/`): universal.md + dedicated grok.md, claude.md, cursor.md, gemini.md, openrouter.md, local.md, custom-loop.md, multi-agent.md. Exact instructions for loading primitives/contracts/personality/harness in each.
- **Hooks & MCP Examples/Patterns** (`hooks/`): mcp-patterns.md + example Python pre/post hooks. Patterns for exposing pillars, harness as tools, evidence execution, dynamic discovery.
- **"Awesome Ultimate Skills" Curation Guide + Initial List** (`awesome/README.md` + `docs/awesome-curation-guide.md`): Strict criteria based on research (lean, cross-compat, harness, adapters, evidence/scores, one-command). Seeded with the flagship + meta-creator.
- **Meta-Skill Creator** (`meta/SKILL.md`): Complete Ultimate skill that helps you build/improve new skills to the exact standards (packaging, 6 pillars, harness, adapters, etc.). The multiplier for community growth.
- **Full Docs, Examples Repo Structure, Contribution Flow**: `docs/DEPLOYMENT.md`, `docs/ECOSYSTEM.md`, `docs/contribution-flow.md`, enhanced root docs, examples/ layout. Clear "how the whole suite deploys together".
- **Deployment Scripts / One-Liners + Suite Bundling**: As above. The deploy-ultimate-suite.sh explicitly bundles "all 6 pillars" as Grok Ultimate Agentic Skills plus the ecosystem shell.

**Reusable by design for 50k-star growth:** Fork one pillar or the whole thing. Use the meta-creator. Submit scored domain skills to the awesome list. Register on marketplaces. Extend via MCP/hooks. All artifacts are MIT and modular.

See `docs/DEPLOYMENT.md` (how to deploy the suite), `docs/ECOSYSTEM.md` (the flywheel), and `packaging/universal-spec.md` (the spec).

---

## Quick Start (Grok Users — Recommended)

1. Copy the entire folder (or just the files you need) into:
   ```
   ~/.grok/skills/grok-mode/
   ```

2. Activate with your environment's skill loading mechanism or by bringing the key modules into context.

3. For maximum power, also load the **Adherence Evaluator** at the start or end of major phases.

Full Grok-native packaging instructions are in `packaging/grok.md`.

**Universal injection** (works for almost any agent):
- Take `core/principles.md`
- Take the full advanced `personality/grok-core.md` (v2.1) — or the Universal Base + Anti-Sycophancy + examples + Self-Checks for lighter loads
- Require use of the templates
- At the end of major work, run the evaluator from `evaluators/adherence-scorer.md` (pay special attention to the upgraded Human-Likeness dimension)

---

## The Mandatory Workflow (v2)

1. **Grill & Align** (use templates)
2. **Design & Approve**
3. **Decompose into Vertical Slices** (mandatory schema)
4. **Persist & Optimize Context**
5. **Execute with TDD + Rigor**
6. **Two-Stage Review** (using the rubric)
7. **Handoff & Close**
8. **Harness Self-Audit + Gates** (Advanced v3 Scorer + evals + launch gates via harness/; log score, gaps turned into harness features or conscious risk acceptance)

The skill is **self-referential**: it requires the agent to score itself.

---

## Built-in Quality Control (This Is What Makes It Elite)

The `evaluators/adherence-scorer.md` is a first-class citizen.

After any significant body of work, score the session 0-100 across 8 dimensions, list gaps, and either fix them or document the conscious trade-off.

This turns "I followed the process" into **measurable, improvable behavior**.

---

## 50k-Star Quality Bar

A skill reaches legendary status when:
- People copy individual modules into completely different agents and see immediate improvement.
- Teams standardize on its templates and rubrics.
- Using it becomes a visible signal of seriousness.
- The community extends it because the contracts are clear and the value is obvious.

v2 is engineered from day one for that outcome.

---

## Installation & Packaging (Full Ecosystem)

**Easiest (Full "Grok Ultimate Agentic Skills" Suite — 6 pillars + meta + awesome + hooks + docs):**
```bash
curl -fsSL https://raw.githubusercontent.com/bobtech-IIT/grok-mode-skill/main/scripts/deploy-ultimate-suite.sh | bash -s -- grok   # or claude / cursor / etc.
```

**Single flagship skill:**
```bash
curl -fsSL https://raw.githubusercontent.com/bobtech-IIT/grok-mode-skill/main/packaging/installers/install.sh | bash -s -- grok
# Or npx skillsadd bobtech-IIT/grok-mode-skill (marketplace)
```

See `packaging/grok.md` (Grok-specific), the new `docs/DEPLOYMENT.md`, `packaging/universal-spec.md`, and per-runtime adapters (claude.md, cursor.md, etc.) for activation after install. The suite deployer handles the complete bundling of all components.

Also see `packaging/installers/install.sh` source for the exact logic (supports lean installs for local/custom).

---

## Changelog & Versioning

See [CHANGELOG.md](./CHANGELOG.md). Semantic versioning. Major contract changes will be clearly documented.

---

## License

MIT — Use it. Improve it. Ship it.

---

**This is not another checklist.**

This is the operating system for agents that want to be *reliably excellent* and *pleasantly human*.

Clone it. Load the modules. Follow the contracts. Score yourself. Improve it.

**Star the repo** if this is the standard you've been looking for. Real usage and honest feedback will drive it to the quality level it deserves.

---

*Built for maximal truth-seeking and maximum helpfulness.*