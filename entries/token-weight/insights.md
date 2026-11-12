# Eval of "token weight" observation

**Core claim holds up.** The asymmetry described is real and is essentially
a form of entropy reduction: planning is where uncertainty gets collapsed
into decisions, and execution is just applying already-resolved decisions.
Once ambiguity is gone, the LLM isn't solving anything anymore — it's
pattern-matching a known shape onto new surface area. That's why it's cheap.
This isn't new in software engineering generally (cost-of-change-over-time,
"measure twice cut once") — what's new is that AI-assisted work makes the
asymmetry *literally measurable in tokens*, not just felt as time/effort.

**Weak point: the Matt Pocock example as evidence.** It's suggestive, not
demonstrative. "He doesn't mention token cost" could equally be explained by
him not tracking cost explicitly, optimizing for teaching clarity, or using
a provider/plan where cost isn't salient — rather than his workflow provably
shaping the planning/execution split the way described. Treat it as an
illustrative anecdote, not a proof point. The insight should stand on its
own reasoning, independent of whether that one example actually confirms it.

**Missing caveat: the ratio is a workflow property, not a law.** It only
holds when the planning phase actually produces a correct, sufficiently
specified plan. If the plan is wrong or underspecified, the "cheap execution"
phase inverts — debugging loops, re-reads of context, backtracking, exactly
where agentic workflows blow up token budgets. So the real implication isn't
"planning costs more, that's fine" — it's that errors in the planning phase
get amplified downstream, so disproportionate investment in getting the plan
*right* (not just made) is what makes the 5:2 ratio hold rather than
collapse into something much worse. This is the actionable half of the
insight — what to *do* with the observation, not just what to notice.
