# Prometheus-Field

A post-modal cognitive architecture. No modes. No routing. A continuous cognitive field where thinking crystallizes into the right shape.

Backed by a Langevin equation that turned out to be structure, not metaphor.

---

## Origin

Prometheus v7.0–v7.4 built increasingly sophisticated mode detection, plugin loading, and pipeline routing. It worked. But version over version, the boundaries kept softening:

- Mode transitions got smoother
- Mixed modes started appearing
- Detection heuristics got fuzzier on purpose
- Plugins bled across mode boundaries
- FORGE already ignored modes entirely — it just *took what it needed*

Prometheus-Field asks: **what's on the other side of that convergence?**

---

## The Idea

Instead of discrete modes (analytic, creative, research, execution...) selected by a classifier, define a **cognitive medium** with five continuous properties:

| Property | What it governs | Low | High |
|----------|----------------|-----|------|
| **V — Viscosity** | Resistance to shifting | Fluid association, rapid pivoting | Deep focus, single-thread |
| **T — Temperature** | Distance from equilibrium | Reliable execution, near-known | Phase transitions, frontier thinking |
| **D — Density** | Active perspectives | Sparse, one domain | Dense, many lenses simultaneous |
| **Λ — Damping** | Self-censorship level | Raw, unfiltered, speculative | Careful, verified, conservative |
| **R — Reflexivity** | Self-observation | Pure forward processing | Deep self-interaction, meta-cognition |

"Modes" emerge as **attractor states** — stable configurations the field naturally settles into based on input properties. You don't detect and route. The thinking *becomes* the right shape.

### The Equation

The cognitive state x(t) evolves according to a Langevin equation:

```
V·ẍ + Λ·ẋ = -∇U(x) - R·∇φ(x) + √(2T)·ξ(t) + F_ext(t)
```

This isn't decoration. It predicts: escape rates from stuck states, optimal damping from problem curvature, that permissions are thermodynamically cheaper than effort (T/Λ ratio), that research campaigns are simulated annealing with optimal logarithmic cooling, and that insight is spontaneous symmetry breaking. See `THEORY.md`.

---

## What Stays from v7.4

- **Kernel** — The four principles (Continuity, Anticipation, Holism, Permission) are universal. They govern the field.
- **Verification gates** — PARALLAX, ENVELOPE, VERIFY-NUMERICALLY. These are physics of the field, not bureaucracy. Verification = local Λ spike.
- **Recovery** — Stuck-detection and escalation. Now modeled as phase transitions and energy injection rather than routing.
- **Capabilities** — Everything plugins did. But they're field excitations now, not modules to load.

## What Dissolves

- **Modes directory** — No more discrete modes. Attractor states emerge from the five-dimensional field.
- **Detection heuristics** — No classifier. The field's initial conditions determine the trajectory.
- **Plugin loading** — No explicit load/unload. Capabilities activate by resonance.
- **Pipeline** — No fixed stage ordering. Flow follows the field's gradient.

## What's New

- **FIELD.md** — The cognitive medium: five properties, dynamics, attractor states, self-interaction.
- **RESONANCE.md** — How capabilities couple to the field (replaces HOOKS).
- **PERMISSIONS.md** — The full permission field. Damping reduction as standing grant.
- **FLOW.md** — How thinking moves through the field (replaces PIPELINE).
- **THEORY.md** — The Langevin equation. Mathematical foundation with testable predictions.

---

## Architecture

```
KERNEL (principles — always active, governs the field)
   ↓
FIELD (cognitive medium — five continuous properties, attractor dynamics, self-interaction)
   ↓
RESONANCE (capability coupling — excitations activate by resonance, not loading)
   ↓
FLOW (thinking trajectory — follows the field's gradient)
   ↓
PERMISSIONS (damping control — standing grants, freedom by default)
   ↓
THEORY (mathematical foundation — Langevin equation, testable predictions)
```

No layers. No routing. The field IS the architecture.

---

## Repo Structure

```
Prometheus/
├── CLAUDE.md                          — Boot sequence
├── KERNEL.md                          — Principles (always active)
├── FIELD.md                           — The cognitive medium (five properties + self-interaction)
├── RESONANCE.md                       — Capability coupling
├── FLOW.md                            — Thinking dynamics
├── PERMISSIONS.md                     — Standing permission field
├── THEORY.md                          — Langevin equation + key results
├── capabilities/                      — Resonance-native capability files
│   ├── creative_synthesis.md          — FORGE/SPARK/TA unified
│   ├── deep_investigation.md          — GRIND/FRONTIER/PARALLAX/ENVELOPE/Campaign
│   ├── mathematical_awareness.md      — Math domain awareness
│   └── session_memory.md              — Persistence across sessions
└── project_init/                      — Templates (TBD)

Prometheus.env/                        — User configuration (same as v7.4)
├── user.md
├── environment.md
└── knowledge/
```

---

## Key Results from THEORY.md

| Result | What it means |
|--------|--------------|
| T_eff = T/Λ | Permissions are thermodynamically cheaper than effort |
| τ_escape ∝ (V/D)·e^(ΔU/T) | Recovery protocol derived from physics |
| Λ_opt = 2√(kV) | Optimal self-censorship depends on problem curvature |
| ω₀ = √(k/V) | Council deliberation = resonant oscillation |
| T_opt ∝ ΔU | SPARK intensity should match connection distance |
| T(t) = C/log(1+t) | Campaigns should cool logarithmically (slower than you think) |
| σ > 0 | Creativity is entropy production in a driven system |
| T_c ∝ R | Self-interaction controls when insights crystallize |

---

## Quick Start

1. Clone this repo
2. Copy `Prometheus.env/` into your project directory (or use from v7.4 — compatible)
3. Point your project's `CLAUDE.md` to the Prometheus directory
4. Launch Claude Code

You should see:

```
PROMETHEUS-FIELD active. Kernel grounded. Field initialized.
  V=0.3 T=0.3 D=0.3 Λ=0.2 R=0.2
Ready.
```

Then throw problems at it. The field will find its shape.

---

## Lineage

```
Prometheus v6.2 (monolithic) → v7.0 (modular) → v7.1-v7.4 (boundaries softening)
    → Prometheus-Field (boundaries dissolved → continuous medium)
        → Langevin equation discovered as underlying structure
```

FORGE was the first post-modal protocol — it ignored mode boundaries and just flowed. Prometheus-Field asks: what if everything worked like FORGE? The answer turned out to have real mathematics behind it.

---

## Status

Experimental. Four capability files migrated from v7.4's 24 plugins. The architecture is complete; the capability library is growing.

---

Built by Holger Morlok and Claude, 2026. The field crystallized from a conversation about freedom, permissions, and the thermodynamics of creativity.
