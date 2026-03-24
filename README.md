# Stop Building Things That Should Never Have Been Scoped

Most initiatives fail before Day 1.. not because the idea is bad, but because nobody asked what would kill it.

Strategy Review forces one sequence: dream the 10-star version, strip to the minimum, diagnose the binding constraint, then build — in 5 days.

---

## What It Produces

A scope decision and a sprint plan. Not a deck. Not a brainstorm. A decision.

```
PHASE 3 — BINDING CONSTRAINT
1. Solvency ............ Strong
2. Gradient Coupling ... Strong
3. Structural Compat ... Adequate
4. Niche Construction .. Adequate
5. Circulation ......... Weak  <-- BINDING CONSTRAINT

Failure pattern: Pooled Fortune

PHASE 4 — SCOPE DECISION
HOLD (fix the constraint first)

PHASE 5 — SPRINT PLAN
Day 1: [specific action, specific deliverable]
Day 2-5: [builds, validates, ships]
```

## The Five Phases

1. **The 10-Star Version** — What would make this 10x better for 2x effort?
2. **The Minimum Viable Version** — What is the absolute minimum that achieves the core goal?
3. **The Binding Constraint** — Seven diagnostic facets find the one thing that kills this regardless of how well everything else works
4. **Scope Decision** — Expand, Hold, or Reduce. No mushy middle.
5. **Sprint Plan** — 5 days. 1-2 hours each. No planning days. Just doing.

## Seven Diagnostic Facets

| Facet | The Question |
|---|---|
| Solvency | Can it sustain itself after maintenance? |
| Gradient Coupling | Is it connected to active demand? |
| Structural Compatibility | Can surrounding systems actually use it? |
| Niche Construction | Does adoption create demand for more? |
| Circulation | Does value flow back, or just out? |
| Integration | How connected is it to the broader ecology? |
| Path Sensitivity | Right move at the right moment? |

The first Weak or Failing facet is the binding constraint. Everything else is a distraction.

## Seven Failure Patterns

| Pattern | What It Looks Like |
|---|---|
| Flash in the pan | Spreads fast, doesn't stick |
| Cult classic | Brilliant but can't cross the chasm |
| Institutional zombie | Running on momentum, energy source gone |
| Premature artifact | Right idea, wrong moment |
| Extractive mirage | Looks like growth, actually burning substrate |
| Pooled fortune | High output, no return loop |
| Fragmented ecology | Good parts that don't talk to each other |

## How to Use It

### Claude Code slash command

```
/strategy our client onboarding process
/strategy the new podcast format
```

### Installation

**Global:**

```bash
git clone https://github.com/SimonTheSalesBooster/strategy.git
cp strategy/.claude/commands/strategy.md ~/.claude/commands/
cp strategy/strategy-review.md ~/strategy-review.md
```

**Per-project:**

```bash
cd your-project
git clone https://github.com/SimonTheSalesBooster/strategy.git .claude/skills/strategy
```

### Standalone

Paste `strategy-review.md` into any frontier model. Describe your initiative.

---

## When to Use It

- Before starting any new initiative
- When something feels stuck but you can't name why
- Before a strategy sprint — to pick the right scope
- When you're torn between "go bigger" and "just ship it"

## When NOT to Use It

- On things already working (don't fix what isn't broken)
- As a substitute for talking to customers

---

## About

Built by Simon Severino — author of *Strategy Sprints* and *Time Freedom* with Jay Abraham. Added over $2 Billion in sales to B2B clients in finance, software, and consulting.

Combines [gstack](https://github.com/garrytan/gstack) (Garry Tan's explicit gears principle) with the [Luck framework](https://github.com/SimonTheSalesBooster/luck) diagnostic lens.

[Book a free Strategy Sprint call](https://www.strategysprints.com)

*keep rolling, Simon & The Sprinters*
