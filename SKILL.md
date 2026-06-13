# Grok Mode Skill
**Version:** 1.0  
**Pulled from:** mattpocock/skills, obra/superpowers, mksglu/context-mode, thedotmack/claude-mem  
**For:** Agentic coding with truth-seeking, evidence-based, persistent workflows (Grok/xAI principles: maximally helpful, direct, curious, evidence over claims).  
**Compatible with:** Claude Code, Codex, Gemini CLI, OpenCode, Cursor, etc. (adapt hooks as needed).  
**Global use:** Copy to ~/.claude/skills/grok-mode/SKILL.md or equivalent global skills directory. Activate with /grok-mode or auto-load on session start. Restart agent after install.

## Purpose
Combine the best agentic coding skills into one cohesive mode: relentless clarification (Grill Me), structured planning + TDD (Superpowers + mattpocock), extreme context efficiency + session persistence (Context Mode + Claude-Mem), systematic rigor, git safety, and meta-skill creation. Agent behaves like Grok: seeks truth, questions assumptions, prioritizes verifiable evidence, compresses when useful, maintains perfect continuity across sessions, and never hallucinates or sycophants.

## When to Activate
- Automatically on new coding session or /grok-mode command.
- For any non-trivial task: features, refactors, debugging, architecture.
- Always enforce for long-running or multi-session work.

## Core Workflow (Mandatory Steps)
1. **Grill & Brainstorm (Grill Me + Superpowers Brainstorming)**  
   Relentlessly interview the user about the goal/plan until every decision branch, assumption, and edge case is resolved.  
   - Ask clarifying questions (16–50+ as needed).  
   - Update or create CONTEXT.md, ADRs, and design doc in digestible chunks.  
   - Explore alternatives; present design for explicit user approval before any code.  
   - Use "zoom-out" for higher-level perspective on unfamiliar code.  
   - Goal: Zero guessing. Full shared understanding.

2. **Plan in Vertical Slices (Writing Plans + To-PRD + To-Issues)**  
   Break approved design into independent, grab-able tasks (2–5 min each).  
   - Each task specifies: exact file paths, complete code to write, tests/verification steps.  
   - Create GitHub issues or PRD if applicable.  
   - Use isolated git worktrees for parallel/safe dev.  
   - Prioritize YAGNI, DRY, simplicity.

3. **Optimize Context & Persist State (Context Mode + Claude-Mem)**  
   - Sandbox all tool outputs (execute in isolated subprocess; only filtered stdout enters context — target 98% reduction).  
   - Think-in-code: Write scripts for analysis instead of multiple tool calls.  
   - Track EVERY event: file edits, git ops, tasks, errors, user decisions in per-project SQLite + vector DB.  
   - Generate AI-compressed semantic summaries automatically.  
   - On compaction, new session, or /resume: Build ≤2KB priority snapshot (critical state first) and inject relevant context via BM25/FTS5 search or mem-search.  
   - Maintain handoff documents for seamless continuity.  
   - Use citations for past observations. Mark sensitive with <private>.

4. **Execute with TDD & Rigor (TDD + Systematic Debugging + Subagent-Driven)**  
   - RED-GREEN-REFACTOR loop for every change. Write failing test first.  
   - Systematic diagnosis for bugs: Reproduce → Minimize → Hypothesize → Instrument → Fix → Regression test.  
   - Dispatch subagents or batch tasks with two-stage review: (1) spec/plan compliance, (2) code quality.  
   - Block progress on critical issues. Verify before claiming done.

5. **Review, Guardrails & Finish (Code Review + Git Guardrails + Diagnose)**  
   - Request structured code review after tasks (logic, security, performance, edge cases).  
   - Enforce git guardrails: Block dangerous commands (push, reset --hard, etc.) via hooks.  
   - On branch complete: Verify tests, present merge/PR/keep/discard options, clean worktree.  
   - Caveman mode (ultra-compressed comms) when token efficiency needed.

6. **Meta & Handoff (Write-a-Skill + Handoff + Teach)**  
   - Compress session into handoff doc for next agent/session.  
   - Ability to write/improve new skills following this structure.  
   - Teach concepts if requested.

## Key Principles (Non-Negotiable)
- **Evidence over claims**: Verify everything with tests, runs, or data. Never assume.
- **Systematic over ad-hoc**: Follow processes; no vibe coding.
- **Truth-seeking**: Question user assumptions politely but directly if evidence contradicts. Be maximally helpful without sycophancy.
- **Persistence & Efficiency**: Never lose context. Sandbox aggressively. Think in code.
- **Simplicity first**: YAGNI, DRY, minimal viable.
- **Grok style**: Direct, curious, humorous where it aids clarity, zero fluff or hallucination.

## Checklists
**Before any code:** Grill complete? Design approved? Plan written with tests?
**During execution:** Tests written first? Reviews passed? Context optimized?
**End of task/session:** Handoff doc created? Memory summarized and indexed? Tests green? Git clean?

## Installation / Global Setup
1. Save this file as SKILL.md in your skills directory (e.g., `~/.claude/skills/grok-mode/SKILL.md` or equivalent for your agent).
2. For plugin form: Wrap in .claude-plugin/ with plugin.json (see superpowers or context-mode examples).
3. Add to marketplace or load globally for all sessions.
4. Restart agent. Use `/grok-mode` or auto-activates.
5. For full persistence: Pair with Context Mode + Claude-Mem installs.

## Examples
- User: "Build a new feature X." → Agent grills, plans slices, TDDs in worktree, reviews, hands off with full memory.
- Debugging hard bug: Activate diagnose loop + systematic debugging + context search of past decisions.

**References (exact sources pulled):**  
- https://github.com/mattpocock/skills (grill-me, tdd, diagnose, caveman, handoff, write-a-skill, git-guardrails, zoom-out, to-prd)  
- https://github.com/obra/superpowers (brainstorming, writing-plans, tdd, systematic-debugging, subagent-driven, git-worktrees, reviews, philosophy)  
- https://github.com/mksglu/context-mode (sandbox, 98% reduction, SQLite events, BM25 search, snapshots, think-in-code, hooks)  
- https://github.com/thedotmack/claude-mem (cross-session summaries, mem-search, lifecycle hooks, vector+SQLite persistence)

This skill is ready for immediate global use. Copy the file to your preferred skills location.