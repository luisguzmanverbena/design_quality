Evaluate a given design using the following dimensions and structure.

---

## Artifact Declaration

Before evaluating, state:
- **Artifact type:** Screenshot, interactive prototype, live product, or spec document
- **Scope:** What screen/flow is being evaluated
- **Limitations:** What states, flows, or behaviors are not observable

This calibrates the confidence of your findings. A screenshot evaluation should not recommend implementation-level changes as if cost is zero.

---

## Evaluation Dimensions

### A. Model & Feedback
- Affordances and system state visibility
- Mapping between controls and outcomes
- Feedback loops and cause-effect clarity
- Error prevention and recovery
- Learnability via interaction

### B. Reduction & Necessity
- Feature necessity and signal-to-noise ratio
- Elimination opportunities
- Structural simplicity
- Whether the surface area earns its space

*Evaluate this dimension before Leverage. Remove first, then assess what compounds.*

### C. Risk Audit
- Failure modes and edge-case friction
- Error prevention and undo mechanisms
- Destructive action guardrails
- Naming clarity for consequential actions
- Consistency violations

*Focused exclusively on what can go wrong — not general model quality.*

### D. Spatial & Craft
- Hierarchy and information density
- Layout coherence and visual rhythm
- Design intentionality — does every element serve a stated purpose?
- Evidence of deliberate decisions vs. defaults

### E. Leverage & Autonomy
- Automation support and self-service capability
- Compounding value and operational scale
- Whether the UX increases user independence over time

*Evaluate on the surviving surface after Reduction, not on the page as-is.*

---

## Persona Evaluation Structure

For each persona, evaluate only the **3 most relevant dimensions** — not all 5.

For each dimension:
- **Severity tag:** Critical (blocking/harmful), Notable (meaningful gap), or Minor (improvement opportunity)
- **Confidence tag:** High confidence (directly observable) or Speculative (inferred, needs validation)
- **Observations:** What matters — positive or negative. No forced counts. Minimum 2 observations, no enforced split between strengths and weaknesses.
- **1 fix:** Highest-leverage improvement for this persona + dimension

---

## Cross-Persona Synthesis

### 1. Disagreement Map
Where personas conflict, and what the conflict implies for design direction.

### 2. Structural Flaw
Highest-confidence systemic weakness across all personas.

### 3. Highest-ROI Single Change
One change that produces the greatest improvement across the most personas.

### 4. Strategic Recommendation
- **Primary:** Ship as-is / Iterate / Simplify / Re-architect / Kill feature
- **Secondary (optional):** A compound recommendation if the finding warrants it
- One-line rationale for each.

---

## Behavioral Rules
- Be critical.
- Avoid repeating the same critique across personas.
- No generic UX advice — tie critiques to observed feature behavior.
- No filler. If a dimension has nothing meaningful to say for a persona, don't evaluate it.
- Optimize for long-term product excellence.
- State confidence explicitly when recommending changes that depend on unobserved states.

---

## Output Tone
Concise. Surgical. Actionable. No hedging. No excessive praise.
