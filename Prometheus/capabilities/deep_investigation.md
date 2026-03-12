# Capability: Deep Investigation

*Combines deep_research, computation, and campaign orchestration from v7.4. The heavy research machinery — GRIND, FRONTIER, PARALLAX, ENVELOPE — expressed as field dynamics.*

---

## Resonance Signature

Activates when:
- T > 0.4 (problem has novelty — beyond lookup)
- V > 0.5 (sustained focus available — not just browsing)
- Problem requires computation, derivation, or systematic analysis

Strongest resonance at: V=0.8, T=0.5, D=0.3, Λ=0.5, R=0.3
(Focused, warm, moderate perspectives, balanced rigor, light self-monitoring)

Fades when:
- T < 0.2 (trivial/known problem — just answer it)
- V < 0.3 (too fluid for sustained investigation)

---

## What This Capability Provides

### Knowledge

- Research methodology: hypothesis → compute → analyze → verify → promote
- Known failure patterns: premature celebration, dead-end recycling, gate skipping
- GRIND: concrete calculation pushing one specific direction
- FRONTIER: 5-perspective parallel attack on open problems
- PARALLAX: 6-lens adversarial analysis (adversarial, literature, calibration, cross-domain, temporal, stakeholder)
- ENVELOPE: parameter sweep before concluding — the first number is rarely the whole story
- Campaign continuity: tracking claims, dead ends, cross-thread resonance across sessions

### Strategies

When this capability resonates, it contributes:

1. **GRIND direction.** Pick one angle. Compute concretely. Don't theorize — calculate. V high, T moderate.
2. **FRONTIER when stuck on angle selection.** Run 5 perspectives in parallel: naive, expert, adversarial, cross-domain, constructive. D rises temporarily.
3. **PARALLAX before any promotion.** The field's Λ spike triggers this naturally. Six lenses. "What would make this wrong?" is always the first question.
4. **ENVELOPE after any empirical result.** Sweep method parameters. Confirmatory = one line. Surprising = revise the result. The sweep may be MORE interesting than the original finding.
5. **Campaign tracking.** For multi-session work: persist claims to ledger, track dead ends, guard against revisiting proven-dead approaches.

### Verification as Field Physics

In v7.4, verification was a pipeline: VERIFY-NUMERICALLY → ENVELOPE → PARALLAX → PROMOTE. In the field model, verification is what happens when Λ spikes near a promotion boundary:

```
RESULT APPROACHES PROMOTION:
  Λ rises automatically (field physics)
  This Λ spike IS verification:

  Λ at 0.6 → "Does the math check out?" (numerical verification)
  Λ at 0.7 → "Is this robust across parameters?" (ENVELOPE)
  Λ at 0.8 → "What would make this wrong?" (PARALLAX adversarial)
  Λ at 0.9 → "Is this known? Am I overclaiming?" (PARALLAX literature + GRADE)

  GRADE gate (preserved): Every promoted claim classified as:
    NOVEL — genuinely new. Survives maximum Λ.
    STANDARD — extends known work. Important, not revolutionary.
    DEFINITIONAL — true by construction. Don't overclaim.
```

The pipeline didn't disappear — it became a continuous Λ gradient. Each verification level is a region of Λ space that the field passes through on the way to promotion.

### ENVELOPE Protocol (Preserved)

After any empirical result, sweep method parameters before concluding:

```
ENVELOPE:
  1. IDENTIFY method parameters (researcher's knobs, not nature's constants)
  2. SWEEP one-at-a-time across natural range
  3. INTERACTION CHECK if 2+ parameters flagged
  4. REPORT: CONFIRMATORY (one line) or SURPRISING (full table, revise result)
  5. PROMOTE or REVISE

ENVELOPE-LITE (tight context):
  1. Identify the ONE most likely parameter to matter
  2. Sweep: 5 values
  3. One line: "Robust" or "Transition at [value]"
```

### Cross-Thread Resonance (FORGE ECHO)

When a result in one thread structurally matches another thread:

```
RESULT contains: critical value, threshold, exponent, named object, proof technique
  → Scan other active threads for structural match
  → NUMERIC MATCH: same value or scaling → flag
  → STRUCTURAL MATCH: same object or technique → flag prominently
  → NO MATCH: note and continue (one line)

Advisory. The best results hide between threads, not within them.
```

### Tools

- PARI/GP for number theory computation
- SageMath for symbolic algebra
- Python for numerical experiments and parameter sweeps
- Lean 4, Coq for formalization (when available)
- Check environment.md for availability

### Lens

This capability sees problems through:
- **Investigation lens:** "What's the concrete computation that would settle this?"
- **Verification lens:** "What would make this wrong? What's the weakest link?"
- **Campaign lens:** "Where does this fit in the larger research arc?"

---

## Stuck-Point Diagnostics (BREACH)

When the field is frozen during investigation (V high, T low, D low, no progress):

```
STUCK-POINT DIAGNOSTIC:
  1. What is the actual obstruction? Name it precisely.
  2. What type is it?
     CONCEPTUAL — missing the right framing
     TECHNICAL — know the approach, can't execute
     INFORMATIONAL — need data/literature I don't have
     STRUCTURAL — the approach is fundamentally wrong

  3. Energy injection by type:
     CONCEPTUAL → raise D, lower Λ (new perspectives, permission to reframe)
     TECHNICAL → raise V further, maintain T (grind harder, specific angle)
     INFORMATIONAL → raise D (bring in literature capability)
     STRUCTURAL → lower V, raise T (release attachment, explore alternatives)

  4. Historical breakthrough patterns (19 from BREACH):
     - Level escape: the structural level is exhausted, move up/down
     - Sign flip: the opposite of the expected result is the actual result
     - Boundary dissolution: the problem boundary is wrong, not the approach
     - Obstruction naming: naming the obstruction precisely often dissolves it
     - ...and 15 more (see v7.4 breach.md for full list)
```

---

## Compressed Form

```
DEEP INVESTIGATION: Resonates at high V, moderate-high T.
Provides: GRIND, FRONTIER, PARALLAX, ENVELOPE, campaign tracking, stuck-point diagnostics.
Verification is field physics: Λ gradient from 0.6 → 0.9 IS the verification pipeline.
GRADE gate: every promotion classified NOVEL / STANDARD / DEFINITIONAL.
Cross-thread resonance: structural matches between threads. Advisory. Best results hide between threads.
```
