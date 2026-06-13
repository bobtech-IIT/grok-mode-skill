# Grok Mode Skill v2

**The Universal Truth-Seeking Agentic Operating System**

> One composable skill that makes *any* agent — Grok, Claude, Gemini, OpenRouter, Hermes, Antigravity, local models, or custom agents — think and act with maximum rigor, evidence, continuity, and human-like excellence.

[![Version](https://img.shields.io/badge/version-2.0.0-blue)](https://github.com/bobtech-IIT/grok-mode-skill) [![License](https://img.shields.io/badge/license-MIT-green)](LICENSE) [![Stars](https://img.shields.io/github/stars/bobtech-IIT/grok-mode-skill?style=social)](https://github.com/bobtech-IIT/grok-mode-skill/stargazers) [![Agent Agnostic](https://img.shields.io/badge/agent--agnostic-Grok%20%7C%20Claude%20%7C%20Any-purple)](https://github.com/bobtech-IIT/grok-mode-skill)

**Status:** Production-grade • Self-auditing • Measurably superior • Built for 50,000+ stars

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
- **A true Grok personality module** that produces naturally curious, direct, witty, evidence-obsessed output — not corporate checklist theater.
- **Robustness layers**: explicit failure modes, recovery protocols, and enforcement mechanisms.
- **Universal reusability**: Every major component can be dropped into *any* agentic system (Grok Build, Claude Code, Cursor, custom OpenRouter loops, local agents, etc.).

The result: Agents that consistently produce higher-quality work, make fewer hallucinations, maintain perfect context across months, and *feel* like a brilliant, trustworthy collaborator instead of a checklist executor.

Early versions of these patterns (grilling + vertical slices + TDD + memory) already produce dramatically better outcomes in the referenced source repos. v2 makes them **portable, enforceable, measurable, and human**.

---

## What Makes v2 Different (Surgical Improvements)

| Area                    | v1 (Original)                          | v2 (This Version)                                      |
|-------------------------|----------------------------------------|-------------------------------------------------------|
| Structure               | One giant prompt                       | Modular, loadable blocks (core + personality + templates + evaluators) |
| Reusability             | Claude-centric                         | Fully agent-agnostic with explicit adapters & atomic blocks |
| Human-likeness          | Mentioned "Grok style"                 | Deep, operational personality module with examples, tone rules, and anti-patterns |
| Robustness              | Aspirational descriptions              | Explicit failure modes, recovery playbooks, self-enforcement loops |
| Measurement             | None                                   | Full 0-100 Adherence Evaluator + self-audit protocol built into every session |
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

## The v2 Modular Architecture (Reusable by Design)

```
grok-mode-skill/
├── SKILL.md                 # Master conductor (start here)
├── core/
│   └── principles.md        # The 7 principles + contracts (agent-agnostic)
├── personality/
│   └── grok-core.md         # Deep Grok voice + tone calibration + examples
├── templates/
│   ├── vertical-slice-plan.md
│   ├── grill-session.md
│   ├── code-review-rubric.md
│   ├── handoff-document.md
│   └── ...
├── evaluators/
│   └── adherence-scorer.md  # 0-100 scoring prompt (use on any session)
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
- Take the relevant parts of `personality/grok-core.md`
- Require use of the templates
- At the end of major work, run the evaluator from `evaluators/adherence-scorer.md`

---

## The Mandatory Workflow (v2)

1. **Grill & Align** (use templates)
2. **Design & Approve**
3. **Decompose into Vertical Slices** (mandatory schema)
4. **Persist & Optimize Context**
5. **Execute with TDD + Rigor**
6. **Two-Stage Review** (using the rubric)
7. **Handoff & Close**
8. **Self-Audit** (0-100 scorer — log the score and gaps)

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

## Installation & Packaging

See the `packaging/` directory for Grok, Claude, universal/custom agents, etc.

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