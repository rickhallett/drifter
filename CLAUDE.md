# drifter

> **Drift detection for personal systems.** Compares stated priorities (intentions, goals, plans) against actual activity (commits, time spent, memory logs) to flag misalignment between what you say matters and what you actually do. CLI + LLM hybrid approach, integrating with memory files and Gastown for continuous self-accountability.

---

## Quick Orient

```bash
./bin/bootstrap   # Fix environment
./bin/gate        # Verify your work
./bin/docs        # Dump context
```

---

## Architecture

See `.agent/architecture.md` for full rules.

```
src/
├── api/         # HTTP handlers
├── services/    # Business logic
├── models/      # Data types
└── utils/       # Helpers
```

---

## Current Focus

**Active:** 
**Next:** 
**Blocked:** 

---

## The Gate

Before any task is "done":
```bash
./bin/gate
```

Exit code 0 = ready. Non-zero = fix it first.

---

## Reference Code

When implementing, follow patterns in:
- `src/services/` — business logic style
- `src/api/` — interface patterns

---

## Prompts

Reusable prompts in `.prompts/`:
- `refactor.md` — refactoring guidelines
- `feature_spec.md` — spec before implementation
- `review.md` — audit checklist

---

## Known Gotchas

- 
