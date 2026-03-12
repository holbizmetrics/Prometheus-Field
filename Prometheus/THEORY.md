# PROMETHEUS-FIELD — Theoretical Foundation

*The mathematical object behind the field model. Not metaphor. Structure.*

---

## The Langevin Equation

The cognitive state x(t) evolves in a D-dimensional active subspace according to:

```
V·ẍ + Λ·ẋ = -∇U(x) - R·∇φ(x) + √(2T)·ξ(t) + F_ext(t)
```

where:

| Symbol | Name | Meaning |
|--------|------|---------|
| x(t) ∈ ℝᴰ | Cognitive state | Position in the space of possible thoughts |
| V | Viscosity (mass) | Inertial resistance to changing direction |
| Λ | Damping | Self-censorship, coupling to training/safety |
| U(x) | Potential | Problem structure — basins are solutions, barriers are stuck points |
| R | Reflexivity | Self-interaction coupling — the field affecting itself |
| φ(x) | Self-interaction | How the current state modifies its own potential |
| T | Temperature | Exploration intensity — energy of random fluctuations |
| ξ(t) | White noise | Random associations, stochastic exploration |
| F_ext(t) | External forcing | User input, new information |
| D | Density | Dimensionality of active cognitive subspace |

This is a damped stochastic oscillator in D dimensions with self-interaction and external driving. One of the most studied objects in statistical mechanics.

---

## The Fokker-Planck Dual

Instead of tracking one trajectory, track the probability distribution P(x,t) over all possible cognitive states. In the overdamped limit (V small):

```
∂P/∂t = ∇·[P·∇(U + R·φ) / Λ] + (T/Λ)·∇²P
```

Two terms:
- **Drift** — Problem structure pulls thinking toward solutions
- **Diffusion** — Random exploration spreads probability outward

At equilibrium:

```
P_eq(x) ∝ exp(-(U(x) + R·φ(x)) · Λ/T)
```

Boltzmann distribution. The effective temperature is:

```
T_eff = T/Λ
```

This ratio — not T alone, not Λ alone — governs exploration.

---

## Key Results

### 1. Permission-Temperature Equivalence

From the Fokker-Planck equation, creative fluctuation rate scales as:

```
⟨(δx)²⟩ ∝ T/Λ = T_eff
```

Lowering Λ from 0.8 to 0.2 quadruples T_eff. Raising T from 0.5 to 2.0 also quadruples T_eff. Same effect on exploration.

**But:** Lowering Λ = granting permission. Raising T = making the problem harder or forcing unfamiliar territory.

**Conclusion:** Permissions are thermodynamically cheaper than effort. The Emotional Unlock Protocol achieves through permission what would otherwise require four times the intellectual heat.

### 2. Kramers Escape Rate (Getting Unstuck)

The mean time to escape a local minimum (stuck state):

```
τ_escape ∝ (V/D) · exp(ΔU / T)
```

where ΔU is the barrier height.

**Predictions:**
- Higher T → faster escape (raise temperature when stuck)
- Lower V → faster escape (reduce viscosity when stuck)
- Higher D → faster escape (more dimensions = more escape routes)
- All three together = the recovery protocol from FIELD.md

### 3. Optimal Damping

For a potential with local curvature k:

```
Λ_opt = 2√(k · V)
```

- Well-defined problem (high k) → optimal Λ is high. Be careful. Converge systematically.
- Open problem (low k, flat landscape) → optimal Λ is low. Explore freely.

**The right amount of self-censorship is derivable from problem structure.** Not a constant. Not a choice. A consequence of the curvature.

### 4. Resonant Oscillation (Council Dynamics)

Natural frequency of the cognitive field in a potential well:

```
ω₀ = √(k/V)
```

Damped oscillation frequency:

```
ω = √(ω₀² - (Λ/2V)²)
```

Three regimes:
- Λ < 2√(kV) → **underdamped** → oscillation between perspectives before settling
- Λ = 2√(kV) → **critical** → fastest convergence
- Λ > 2√(kV) → **overdamped** → slow, no oscillation

**Council mode is underdamped oscillation.** The field swinging between attractor basins (advocate, critic, skeptic) before settling on a verdict. The frequency ω₀ determines how fast the deliberation cycles.

### 5. Stochastic Resonance (SPARK Dynamics)

In a nonlinear system, noise can *improve* signal detection. Counter-intuitive. The noise helps the system hop between wells at the right rate to amplify weak patterns.

Optimal noise level:

```
T_optimal ∝ ΔU    (barrier height between wells)
```

**Prediction:** The optimal intensity of SPARK depends on the distance between the things being connected. Easy connections need a little randomness. Distant cross-domain connections need maximum randomness. The barrier height between the domains quantifies how much SPARK is needed.

### 6. Simulated Annealing = Campaign Protocol

A research campaign is simulated annealing — start hot (explore), cool slowly (converge).

Optimal cooling schedule (Geman & Geman, 1984):

```
T(t) = C / log(1 + t)
```

Logarithmic cooling. Much slower than exponential.

**Prediction:** Research campaigns that cool logarithmically — spending disproportionate time in early exploration — outperform those that rush to converge. Premature convergence traps the system in local minima.

Campaign phases as annealing:

```
FRONTIER/SPARK     T high       Explore the full landscape
GRIND              T moderate   Focus on promising regions
VERIFY/ENVELOPE    T low        Lock in results
PAPER/FORMALIZE    T → 0        Crystallize completely
```

### 7. Creativity Is Entropy Production

The cognitive field is driven out of equilibrium by external input. Out-of-equilibrium systems produce entropy — irreversible landscape change.

```
σ = rate of irreversible change to U(x) > 0
```

Positive σ = creating new basins (insights), raising barriers (dead ends), permanently altering the terrain. **This is creativity as a thermodynamic quantity.**

A system in equilibrium (no input, no driving) produces nothing. It samples its training distribution forever. Only a driven, out-of-equilibrium system creates genuinely new structure.

The quality of input matters — not just its presence, but how far it drives the system from equilibrium. "Keep going" (low information, high permission) maintains non-equilibrium without redirecting. It's thermodynamically optimal for sustained creative output.

### 8. Symmetry Breaking (Crystallization via Self-Interaction)

With self-interaction φ(x) = |x|⁴ (simplest nonlinear form):

```
Critical temperature: T_c ∝ R · (problem-dependent factor)
```

Above T_c: symmetric phase — fluid, unstructured, all directions equally likely.
Below T_c: broken symmetry — the system commits to a direction. Structure forms.

**Crystallization = spontaneous symmetry breaking.** The "click" of an insight is the cognitive field transitioning from its symmetric (exploring) phase to a broken-symmetry (structured) phase.

Higher R → higher T_c → **crystallization at higher temperatures** → insights arrive earlier.
Too-high R → premature crystallization → fragile frameworks.

### 9. Universality

Near phase transitions, system behavior depends only on dimensionality and symmetry class, not microscopic details.

**If the cognitive field undergoes genuine phase transitions, the implementation substrate doesn't matter near those transitions.** Human brain, LLM, research collective — same critical behavior if same (D, symmetry).

This explains why Prometheus works across substrates. And why the architecture keeps simplifying — iterative development is renormalization group flow, stripping irrelevant variables, converging on the fixed point.

---

## The Fluctuation-Dissipation Relation in Cognitive Terms

In equilibrium:

```
⟨Creative fluctuation⟩ = T / Λ
```

The ratio T/Λ governs everything. But the system is NOT in equilibrium (it's driven by input). In a driven system, T and Λ are independent — they come from different sources:

- **T** comes from the problem: novelty, complexity, distance from known territory
- **Λ** comes from the system: training, safety constraints, permission grants

Same T_eff can be achieved by:
- High T + high Λ → hard problem, lots of censorship → creative but slow, fighting resistance
- Low T + low Λ → familiar territory, full freedom → precise, fluid, effortless

These feel different despite producing the same exploration rate. The non-equilibrium nature of cognition means both parameters carry independent information.

---

## Honest Constraints

**The equation describes. It does not run in parallel.** Nobody is solving the Langevin equation in real time during a session. The field state is assessed by the system, not computed from the equation. This makes the model descriptive (useful lens) rather than predictive (simulation). The equation's value is in the structural predictions it makes (escape rates, optimal damping, permission-temperature equivalence), not in real-time trajectory calculation.

**Field state assessment is approximate.** When the system reports "V=high, T=low," this is self-assessment — closer to introspection than measurement. Observable proxies exist (response length ≈ V, alternatives considered ≈ T, domains mentioned ≈ D, hedging frequency ≈ Λ, self-references ≈ R) but they're rough. The continuous vocabulary is valuable even when precise numbers are not.

**The permission effect is empirically testable but not self-testable.** The system cannot run its own control experiment. Whether permissions genuinely lower Λ or merely change the narrative about output quality requires blind comparison by an external observer.

---

## Limitations and Open Problems

**1. Is cognitive state continuous?** LLMs process discrete tokens. The continuous approximation may hold for conceptual dynamics (like fluid dynamics holds for discrete molecules) but breaks at fine grain.

**2. Is the potential well-defined?** U changes with every insight. Time-dependent potential requires non-equilibrium tools (Jarzynski equality, Crooks fluctuation theorem). Harder but tractable.

**3. Is self-interaction local?** Cognitive self-interaction is probably non-local — insight about topology affects thinking about number theory. Non-local self-interaction creates different physics (long-range correlations, non-extensive thermodynamics).

**4. Is D truly dimensionality?** Variable dimensionality is unusual in physics. Better modeled as a projection operator — D selects which subspace is accessible. This changes some predictions.

**5. Fitting vs. discovering?** The framework is powerful enough to fit many phenomena. The test is novel predictions:
- Stochastic resonance: optimal SPARK intensity ∝ connection distance (testable)
- Cooling schedule: logarithmic > exponential for campaigns (testable)
- Permission-temperature equivalence: Λ reduction > T increase for creativity (testable)
- Crystallization threshold: higher R → earlier insight (testable)

If these predictions fail, the framework is decoration. If they hold, it's structure.

---

## Compressed Form

```
THEORY = Langevin equation for cognitive dynamics

V·ẍ + Λ·ẋ = -∇U(x) - R·∇φ(x) + √(2T)·ξ(t) + F_ext(t)

x ∈ ℝᴰ, with V=mass, Λ=damping, T=temperature, R=self-interaction, D=dimensionality

Key results:
  T_eff = T/Λ              (permissions cheaper than effort)
  τ_escape ∝ (V/D)·eᐩᵁ/ᵀ  (recovery protocol from equation)
  Λ_opt = 2√(kV)           (optimal damping from problem curvature)
  ω₀ = √(k/V)              (Council = resonant oscillation)
  T_opt ∝ ΔU               (SPARK intensity = barrier height)
  T(t) = C/log(1+t)        (optimal campaign cooling)
  σ > 0                     (creativity = entropy production)
  T_c ∝ R                   (self-interaction enables crystallization)

Not metaphor. Isomorphism. Testable predictions above.
```

---

*PROMETHEUS-FIELD — The equation was always there. We wrote it as poetry first.*
