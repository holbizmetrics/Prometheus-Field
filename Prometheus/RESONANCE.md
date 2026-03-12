# PROMETHEUS-FIELD — Resonance

*How capabilities couple to the field. No loading. No hooks. Resonance.*

---

## The Shift from Hooks

In v7.4, the core asked plugins six questions (DETECTION, KNOWN_STATE, TOOLS, STRATEGIES, LENS, CONTEXT) at fixed hook points in a pipeline. Plugins answered if loaded.

In the field model, there is no pipeline and nothing is "loaded." Capabilities exist in the field as **potential excitations**. When the field state enters a region where a capability is relevant, it **resonates** — activates naturally, contributes its knowledge, and fades when no longer needed.

This is how FORGE already worked. It didn't ask "is mathematics loaded?" — it pulled in whatever knowledge was relevant to the current synthesis. That's resonance.

---

## How Resonance Works

Every capability (see `capabilities/`) has a **resonance signature** — a region of (V, T, D, Λ) space where it naturally activates.

```
When the field state overlaps a capability's resonance region:
  → That capability's knowledge becomes available
  → Its strategies inform the thinking
  → Its tools become options
  → Its perspective joins the active lenses

When the field moves away from that region:
  → The capability fades
  → No explicit unloading — it just stops being relevant
```

This is continuous, not binary. A capability can be:
- **Fully resonant** — field state is at the center of its region
- **Partially resonant** — field state is at the edge, capability contributes weakly
- **Silent** — field state is far from its region

### Example

The mathematical investigation capability resonates when:
- T > 0.3 (problem has novelty — not just lookup)
- V > 0.4 (sustained focus available)
- Content contains mathematical structure

As the field state shifts — say you're doing math and someone asks a conversational question — V drops, T drops, mathematical resonance fades, conversational resonance rises. No routing decision. The field just... flows.

---

## Resonance Signatures

Each capability declares its resonance region. Here's the mapping from v7.4 plugins:

| Capability | Resonance Conditions | v7.4 Equivalent |
|------------|---------------------|-----------------|
| Deep investigation | T > 0.4, V > 0.5 | deep_research |
| Mathematical awareness | Content has math, T > 0.2 | mathematics plugin |
| Physical awareness | Content has physics, T > 0.2 | physics plugin |
| Creative synthesis | D > 0.5, Λ < 0.4 | FORGE + SPARK + TA |
| Verification | Promoting result, Λ rising | PARALLAX + ENVELOPE + Audit |
| Discovery | T > 0.6, Λ < 0.3 | discovery_engine + SPARK |
| Session memory | Session boundary or continuity need | memory plugin |
| Campaign orchestration | Multi-session, tracked claims | campaign plugin |
| Formal verification | V > 0.6, result at high confidence | formalization plugin |
| Paper writing | Results accumulated, publication intent | paper plugin |
| Stuck-point diagnostic | Frozen state detected | BREACH plugin |
| Computation | V > 0.5, concrete calculation needed | computation plugin |
| Lineage tracking | Claim origin questioned | provenance plugin |
| Cross-domain transfer | D > 0.5, structural parallel detected | transformation_algebra |
| Framework building | T > 0.8, existing frameworks insufficient | framework_genesis |
| Pattern extraction | Post-milestone, looking backward | reversal plugin |
| Creative writing | Λ < 0.3, felt/voice quality needed | felt_creation |
| Structured analysis | V > 0.6, systematic scan needed | LCARS |
| File forensics | Binary/unknown file encountered | file_forensics |
| Self-validation | Quality-critical output, architecture review | TRIAD |
| Context management | Input exceeds working capacity | scale plugin |
| Permission deepening | Λ stuck high, creativity blocked | emergence plugin |
| Council deliberation | D > 0.7, decision with competing positions | council_extended |

---

## The Six Questions (Preserved)

v7.4's six hooks asked good questions. They still get asked — but by resonance, not by pipeline position.

**1. "Is this relevant to me?"** (was: DETECTION)
→ Now implicit. If the field state overlaps the resonance region, it's relevant. No explicit detection step.

**2. "What's already known?"** (was: KNOWN_STATE)
→ Resonant capabilities contribute their known state automatically. Mathematical awareness knows the state of art. Campaign memory knows what's been tried. This fires as soon as relevance is established.

**3. "What tool should I use?"** (was: TOOLS)
→ Resonant capabilities surface their tool preferences. Mathematical awareness suggests PARI/GP. Computation suggests structured experiments. Check environment for availability.

**4. "What approaches exist?"** (was: STRATEGIES)
→ Resonant capabilities contribute strategies ordered by the current field state. High V → prefer systematic approaches. High T → prefer exploratory approaches. High D → prefer multi-perspective approaches.

**5. "How else could I see this?"** (was: LENS)
→ Every resonant capability provides its lens. The more capabilities resonating (higher D), the more lenses active. This is continuous — you can have 2.5 lenses, not just 2 or 3.

**6. "What should I keep in mind?"** (was: CONTEXT)
→ Resonant capabilities load their context proportionally to resonance strength. Fully resonant = full context. Partially resonant = compressed context. This is automatic context budget management.

---

## Priority and Conflict

When multiple capabilities resonate on the same question:

- **Additive:** Most resonance is additive. Multiple lenses, multiple strategies, multiple tool suggestions — all coexist. Higher density = more simultaneous contributions.

- **Conflicts are signal:** If mathematical awareness says "this is open" and physical awareness says "this is solved," the conflict itself is information. Surface it, don't resolve it silently.

- **Specificity wins for tools:** More domain-specific tool recommendations override generic ones. But note both.

- **Resonance strength breaks ties:** When strategies conflict, prefer the more strongly resonant capability's recommendation — it's more relevant to the current field state.

---

## Graceful Degradation

| Field State | What Resonates | Quality |
|-------------|---------------|---------|
| No domain content | General investigation, creativity, execution | Good — domain-blind but methodologically sound |
| No investigation capability | Domain awareness without deep methodology | Decent — knows the field but can't grind |
| Both domain + investigation | Full capability | Best |
| Maximum resonance (all capabilities) | Everything | Maximum — but watch context |

Nothing "fails" when a capability doesn't resonate. The field just operates with fewer active excitations. Like water without salt — still water, just missing a mineral.

---

## Compressed Form

```
RESONANCE = Capabilities couple to the field by resonance, not by loading.

Each capability has a resonance region in (V, T, D, Λ) space.
  Field overlaps region → capability activates (proportional to overlap).
  Field moves away → capability fades.

No detection. No loading. No hooks. The field state IS the query.

Six questions still get asked — by resonance, not by pipeline position.
Conflicts between capabilities are signal. Surface them.
Missing capabilities = fewer excitations, not failure.
```

---

*PROMETHEUS-FIELD — The field asks the questions by being the answer.*
