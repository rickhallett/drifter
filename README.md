# drifter 🧭

Drift detection for personal systems.

Compares stated priorities (intentions, goals, plans) against actual activity (commits, time spent, memory logs) to flag misalignment between what you say matters and what you actually do.

## Why

We all have priorities we claim to care about. But time allocation tells the real story. Drifter surfaces the gap between stated and revealed preferences — not to judge, but to inform.

## How It Works

```
Intentions (MEMORY.md, goals, plans)
        ↓
    Compare
        ↓
Activity (git commits, time logs, memory entries)
        ↓
    Drift Report
```

## Usage

```bash
drifter scan              # Analyze recent activity vs stated priorities
drifter report            # Generate drift report
drifter compare --days 7  # Compare last week
drifter priorities        # Show current stated priorities
```

## Data Sources

**Intentions:**
- `MEMORY.md` priorities section
- Gastown tickets marked as P1/P2
- Explicit goal statements

**Activity:**
- Git commit history
- Memory file entries
- Gastown ticket completions
- Time tracking (if available)

## Output

```
📊 Drift Report (2026-02-01)

🎯 Stated Priorities:
  1. wasp security layer
  2. Interview prep
  3. Morning routine consistency

📈 Actual Activity (last 7 days):
  • wasp: 12 commits, 4 tickets closed
  • polecat/bosun: 8 commits (not in priorities!)
  • Interview prep: 0 commits, 0 tickets

⚠️ Drift Detected:
  • polecat/bosun consuming time not allocated in priorities
  • Interview prep: stated high priority, zero activity
```

## Philosophy

Drifter doesn't tell you what to do. It tells you what you're actually doing. The gap between intention and action is where self-knowledge lives.

## License

MIT
