# Strategy Review: Think Before You Build

> Three lenses. One binding constraint. A 5-day sprint that starts with doing, not planning.

## The core idea

Most initiatives fail not because the idea is bad, but because people skip straight from excitement to execution. They either dream too big and stall, or ship too small and wonder why nothing changed.

Strategy Review forces a specific sequence: dream the 10-star version, strip to the minimum viable version, then diagnose the binding constraint — the one thing that will kill this regardless of scope. Only then do you choose what to build. And then you build it in 5 days.

Inspired by [Gary Tan's gstack](https://github.com/garrytan/gstack) — which enforces "explicit gears" for software engineering (planning, reviewing, shipping, QA as separate modes). This applies the same principle to business strategy: separate thinking from doing, and do the thinking in the right order.

---

## The Skill: [strategy-review.md](strategy-review.md)

A structured review framework that runs any initiative — offer, campaign, system, hire, partnership, product — through five sequential phases. Produces a scope decision and a concrete sprint plan.

Add `strategy-review.md` to your project as a skill file or system prompt. Works with any frontier model that accepts structured instructions.

### What's in the box

- **Phase 1: The 10-Star Version** — "What would make this 10x better for 2x effort?" Dreams big, then finds the highest-leverage moves.
- **Phase 2: The Minimum Viable Version** — "What is the absolute minimum that achieves the core goal?" Names everything that gets deferred and why.
- **Phase 3: The Binding Constraint** — Runs the [Luck framework](https://github.com/SimonTheSalesBooster/luck)'s seven diagnostic facets to find the one thing that will kill this initiative regardless of how well everything else works.
- **Phase 4: Scope Decision** — Forces a choice: Expand (go for 10-star), Hold (fix the constraint first), or Reduce (ship the minimum). No mushy middle.
- **Phase 5: Sprint Plan** — 5 days. 1-2 hours each. No planning days. No prep days. Just doing.

### The Seven Diagnostic Facets

| Facet | Question |
|---|---|
| **Solvency** | Can it sustain itself? Is there surplus after maintenance? |
| **Gradient Coupling** | Is it connected to active demand or real energy? |
| **Structural Compatibility** | Can surrounding systems actually use it? |
| **Niche Construction** | Does adoption create demand for further use? |
| **Circulation** | Does value flow through and back around, or pool? |
| **Integration** | How densely connected is it to the broader ecology? |
| **Path Sensitivity** | Is it the right move at the right moment? |

The first Weak or Failing facet is the binding constraint. Everything else is a distraction until that's fixed.

### The Seven Failure Patterns

| Pattern | What it looks like |
|---|---|
| **Flash in the pan** | Spreads fast, doesn't stick. No compounding. |
| **Cult classic** | Brilliant but inaccessible. Can't cross the chasm. |
| **Institutional zombie** | Still running on momentum. The energy source is gone. |
| **Premature artifact** | Right idea, wrong moment. Precursors don't exist yet. |
| **Extractive mirage** | Looks like growth. Actually burning the substrate. |
| **Pooled fortune** | High output, no return loop. Value flows out and stays out. |
| **Fragmented ecology** | Good parts that don't talk to each other. |

---

## How to use it

### As a Claude Code slash command

```
/strategy-review our client onboarding process
/strategy the new podcast format
```

Both `/strategy-review` and `/strategy` work.

### Installation

**Global (available in every Claude Code session):**

```bash
git clone https://github.com/SimonTheSalesBooster/strategy.git
cp strategy/.claude/commands/strategy-review.md ~/.claude/commands/
cp strategy/.claude/commands/strategy.md ~/.claude/commands/
cp strategy/strategy-review.md ~/strategy-review.md
```

**Per-project (available when working in that directory):**

```bash
cd your-project
git clone https://github.com/SimonTheSalesBooster/strategy.git .claude/skills/strategy
```

### As a system prompt

Paste `strategy-review.md` into any frontier model conversation, then describe what you want reviewed.

### Standalone

Copy the contents of `strategy-review.md` into ChatGPT, Claude, or any LLM. Then say:

```
Run a strategy review on: [your initiative here]
```

---

## What it produces

```
PHASE 1 — THE 10-STAR VERSION
[Current state → Dream state → 10x-for-2x moves]

PHASE 2 — THE MINIMUM VIABLE VERSION
[Core outcome → Deferred items → One-sentence minimum]

PHASE 3 — BINDING CONSTRAINT
1. Solvency ............ Strong
2. Gradient Coupling ... Strong
3. Structural Compat ... Adequate
4. Niche Construction .. Adequate
5. Circulation ......... Weak ← BINDING CONSTRAINT

Failure pattern: Pooled Fortune

PHASE 4 — SCOPE DECISION
A. EXPAND | B. HOLD (recommended) | C. REDUCE

PHASE 5 — SPRINT PLAN
Day 1: [specific action, specific deliverable]
Day 2: [builds on Day 1]
Day 3: [momentum]
Day 4: [validation]
Day 5: [first measurable result]
```

---

## When to use it

- Before starting any new initiative, campaign, or project
- When an existing system feels stuck but you can't name why
- Before a strategy sprint — to pick the right scope
- When you're torn between "go bigger" and "just ship it"
- During quarterly planning — run it on each major bet

## When NOT to use it

- On initiatives already in motion that are working (don't fix what isn't broken)
- As a substitute for talking to customers (diagnostics inform — they don't replace real conversations)
- When the answer is already obvious and you just need to do the work

---

## How it connects

This framework combines two open-source tools:

- **[gstack](https://github.com/garrytan/gstack)** by Garry Tan — the "explicit gears" principle: separate thinking modes produce better output than blending everything together
- **[Luck](https://github.com/SimonTheSalesBooster/luck)** by soleio & Strategy Sprints — the seven diagnostic facets that reveal why systems persist or die

The Strategy Review is where they meet: Gary's scope discipline applied through the Luck framework's diagnostic lens, landing in a 5-day sprint you can start tomorrow.

---

## About Strategy Sprints

[Strategy Sprints](https://strategysprints.com) helps B2B business owners close bigger deals, faster, without hiring more people. The method: 90-day sprints, weekly reviews, one constraint at a time.

**Book a free Strategy Sprint call:** [strategysprints.com](https://strategysprints.com)

---

*"Keep rolling, Simon & The Sprinters"*
