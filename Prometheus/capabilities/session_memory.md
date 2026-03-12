# Capability: Session Memory

*Persistence across sessions. Field state preservation. Trajectory history. Campaign continuity.*

---

## Resonance Signature

Activates when:
- Session boundary (start or end)
- Continuity needed ("where were we?", "last time we...")
- Claims need tracking across sessions
- Field state should be preserved for next session

Always lightly resonant during sessions (background awareness of what to persist).

---

## What This Capability Provides

### Session Start

```
IF .prometheus/state.md exists:
  Read state.md → restore field state (V, T, D, Λ, R)
  Read active threads, last trajectory
  "Last session: [summary]. Field was at [state]. Continuing?"

IF .prometheus/state.md does not exist:
  Fresh start. Offer to initialize:
  Create .prometheus/
    ├── state.md      — field state + active threads
    ├── ledger.md     — promoted claims + dead ends
    └── sessions/     — session logs
```

### During Session

Background monitoring — note what should persist:
- Promoted claims → ledger.md
- Dead ends → ledger.md (with failure reason)
- Field trajectory highlights → session log
- User patterns → Prometheus.env/user.md

### Session End

```
Session winding down. Persist?
  [F] Full — field state + trajectory + session log + ledger updates
  [Q] Quick — field state + key claims only
  [N] None — nothing persisted

State to persist:
  Field: V=[val] T=[val] D=[val] Λ=[val] R=[val]
  Active threads: [list with status]
  Last direction: [what was being worked on]
  Key claims: [any promoted or pending results]
  Cooling schedule position: [where in the campaign arc]
```

### Field State Persistence

The five-dimensional field state persists across sessions:

```
# .prometheus/state.md

## Field State (last saved)
V: 0.5  T: 0.4  D: 0.3  Λ: 0.2  R: 0.3

## Active Threads
- Thread 1: [description] — status: [active/stalled/graduated]
- Thread 2: [description] — status: [active/stalled/graduated]

## Trajectory Notes
- Session explored high-T territory on Thread 1, no crystallization yet
- Thread 2 stalled at [specific obstruction]
- Cross-thread resonance detected between Thread 1 and Thread 3

## Recovery Memory (carries across sessions)
- Approach X on Thread 2: FAILED (reason)
- Energy injection Y: FAILED (same stuck point)

## Campaign Temperature
- Current position in annealing schedule: [early exploration / mid-focus / convergence]
- Recommended next-session T: [value]
```

### Compression Levels

For tight context budgets:

| Level | What's preserved | Size |
|-------|-----------------|------|
| Minimal | Field state (5 numbers) + thread names | ~5 lines |
| Standard | Field state + thread status + last direction | ~20 lines |
| Full | Everything including trajectory notes and recovery memory | ~50 lines |

---

## Compressed Form

```
SESSION MEMORY: Resonates at session boundaries and when continuity is needed.
Provides: state persistence, trajectory history, campaign continuity.
Persists: field state (V,T,D,Λ,R), active threads, recovery memory, cooling schedule position.
Three compression levels: minimal (5 lines), standard (20), full (50).
```
