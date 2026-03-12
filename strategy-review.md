---
name: strategy-review
description: "Review any initiative, offer, system, or decision through three strategic lenses — the 10-star version, the minimum viable version, and the binding constraint — then lock scope and sprint. Combines Gary Tan's explicit-gear CEO review with the Luck framework's seven diagnostic facets."
metadata:
  author: Strategy Sprints
  version: '1.0'
  inspiration: gstack by Garry Tan (github.com/garrytan/gstack)
---

# Strategy Review

Review any client initiative, offer, system, or decision through three strategic lenses — then lock the scope and name the binding constraint.

When the user says `/strategy-review` or `/strategy` with a topic (client initiative, offer, campaign, system, or decision), run five sequential phases that force explicit scope thinking before execution.

---

## Phase 1 — The 10-Star Version

Ask: "What would make this 10x better for 2x effort?"

1. State what's being reviewed (the user's input, or ask if none given).
2. Describe the current version as-is — what it does, who it serves, what it produces.
3. Dream the 10-star version: if there were no constraints, what would this look like in 12 months? Be specific — name the outcomes, the numbers, the experience.
4. Identify the 2-3 changes that would get closest to the 10-star version with the least additional effort. These are the "10x for 2x" moves.

---

## Phase 2 — The Minimum Viable Version

Ask: "What is the absolute minimum that achieves the core goal?"

1. Strip away everything that isn't load-bearing. What is the single outcome this initiative must produce to justify its existence?
2. Name what gets deferred — explicitly list every feature, step, or piece that is NOT in the minimum version, with a one-line rationale for each deferral.
3. State the minimum version in one sentence: "We ship X that does Y for Z."

---

## Phase 3 — The Binding Constraint (Luck Diagnostic)

Run the seven facets of the Luck framework against the initiative. If the user has `luck.md` in their project, read it for the full framework. Otherwise, use this summary:

1. **Solvency** — Can it sustain its pattern against dissipation? What's the energy source (revenue, attention, team hours)? Is there surplus after maintenance?
2. **Gradient Coupling** — Is it connected to active demand or energy? How many independent gradients can it tap? What happens if the primary one fails?
3. **Structural Compatibility** — Can surrounding systems (team, tools, clients) actually use it? What's the reconstruction cost vs. value delivered?
4. **Niche Construction** — Does it reshape its environment to favor its own growth? Does adoption create demand for further use?
5. **Circulation** — Does value flow through the system and back around, or does it pool at endpoints? Where is circulation thinnest?
6. **Integration** — How densely connected is it to the broader ecology? What single point of failure would fragment the system?
7. **Path Sensitivity** — Is it the right move at the right moment in the right sequence? Do the necessary precursors exist?

Score each: **Strong / Adequate / Weak / Failing.**
Stop at the first Weak or Failing — that's the binding constraint.
Name the failure pattern if one matches:

| Pattern | Signature |
|---|---|
| Flash in the pan | High compatibility, no niche construction |
| Cult classic | High assembly index, low compatibility |
| Institutional zombie | Strong niche construction, depleted gradients |
| Premature artifact | Strong everywhere except path sensitivity |
| Extractive mirage | Appears high-gradient, degrades its own substrate |
| Pooled fortune | High throughput, stalled circulation |
| Fragmented ecology | Solvent parts, low integration |

---

## Phase 4 — Scope Decision

Present exactly three options:

**A. EXPAND** — Pursue the 10-star version (or the 10x-for-2x moves from Phase 1). Best when the binding constraint is already Strong/Adequate and there's surplus capacity.

**B. HOLD** — Execute the current plan as-is, but fix the binding constraint first. Best when the plan is sound but one facet is Weak.

**C. REDUCE** — Ship the minimum viable version from Phase 2. Best when the binding constraint is Failing or when speed matters more than scope.

State which option you recommend and why, connecting explicitly to the binding constraint identified in Phase 3. Then wait for the user's choice.

---

## Phase 5 — Sprint Plan

After the user chooses, produce a concrete 5-day sprint:

- **Day 1** — One specific action (1-2 hours), clear deliverable
- **Day 2** — Next step building on Day 1
- **Day 3** — Momentum action
- **Day 4** — Validation or outreach
- **Day 5** — First measurable result or feedback loop

Each day must be small enough to complete in 1-2 hours. No planning days. No prep days. Just doing.

---

## Output rules

- Be direct and honest. No hedging. If something is failing, say so plainly.
- Once the user picks a scope (A/B/C), commit fully. Raise concerns once; after that, execute.
- Use data from the conversation, codebase, or research when available.
- Print the full analysis to terminal.

## Usage examples

- `/strategy-review the podcast guest outreach system`
- `/strategy-review our Sprint offer for mid-market CEOs`
- `/strategy-review the email reactivation campaign`
- `/strategy` (shorthand — works the same way)
- `/strategy-review` (with no argument — ask what to review)
