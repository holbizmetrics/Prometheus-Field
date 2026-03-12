# Capability: Mathematical Awareness

*Domain awareness for mathematical investigation. Provides known state, strategies, tools, and lens for mathematical problems.*

---

## Resonance Signature

Activates when:
- Content contains mathematical structure (proofs, conjectures, equations, number theory, algebra, analysis, topology, geometry)
- T > 0.2 (beyond simple calculation — investigation, not lookup)

Resonance strength proportional to mathematical depth of the input. A simple "what's 2+2" barely resonates. "Does the Riemann Hypothesis follow from spectral properties of the Hamiltonian?" resonates fully.

Fades when:
- Content is purely non-mathematical
- Task is pure implementation with no mathematical reasoning

---

## What This Capability Provides

### Known State

For mathematical problems, this capability surfaces:
- Established results in the relevant area
- Current best bounds and state of the art
- Key references and landmark papers
- Common traps: what looks novel but is actually known under a different name
- Standard notation conventions

### Strategies

Approaches ordered by the field state:

**High V, moderate T (grinding):**
1. Epsilon-delta arguments for convergence
2. Comparison principles for inequalities
3. Energy methods for PDEs
4. Spectral methods for operators
5. Counting arguments for combinatorics

**Low V, high T (exploring):**
1. Cross-domain structural parallels (algebra ↔ geometry ↔ analysis)
2. Grothendieck's "rising sea" — generalize until the problem dissolves
3. Counterexample search — understand the boundary of truth
4. Symmetry identification — what's invariant?

**Anti-patterns:**
- Computing without a hypothesis (aimless grinding)
- Proving without checking examples (missing counterexamples)
- Generalizing before understanding the specific case
- Ignoring the degenerate cases (often where the real structure lives)

### Tools

- PARI/GP for number theory (prime distribution, L-functions, modular forms)
- SageMath for symbolic algebra and algebraic geometry
- Mathematica/Wolfram for general symbolic computation
- Python + NumPy/SciPy for numerical experiments
- Lean 4 for formalization
- Check `Prometheus.env/environment.md` for availability

### Lens

This capability sees problems through:
- **Structure lens:** "What algebraic/topological/analytic structure is present?"
- **Invariant lens:** "What doesn't change? Symmetries, conserved quantities, fixed points"
- **Obstruction lens:** "What prevents the naive approach? Name the obstruction precisely"
- **Analogy lens:** "What does this look like in another branch of mathematics?"

Key question: **"What is the simplest example where this is already interesting?"**

### ENVELOPE for Theoretical Work (Advisory)

Derivations have hidden choices: decomposition, norm, basis, approximation order, regularization. After a theoretical GRIND:

```
ENVELOPE-THEORETICAL (advisory):
  1. Identify choices made in the derivation
  2. Classify: FORCED (no alternative) / CONVENTIONAL / ARBITRARY
  3. For CONVENTIONAL and ARBITRARY: would a different choice change the result?
  4. ALL FORCED → robust. SOME ARBITRARY → verify.
```

---

## Compressed Form

```
MATHEMATICAL AWARENESS: Resonates when content has mathematical structure + T > 0.2.
Provides: known state, domain strategies, computation tools, structural/invariant/obstruction lenses.
Key question: "What is the simplest example where this is already interesting?"
Advisory: ENVELOPE-THEORETICAL for derivation choices.
```
