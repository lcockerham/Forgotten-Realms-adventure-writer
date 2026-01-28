# Faerun Adventure Writer - Project Summary

## What It Is
A Claude Code skill for generating one-page D&D adventures set in the Forgotten Realms. Includes commands for adventure generation and quality evaluation.

## Repository
`https://github.com/lcockerham/Forgotten-Realms-adventure-writer`

## Current State
- **Just pushed** commit `b01c268` with commands, deities reference, and evaluation system
- **Baseline established**: 10 adventures evaluated, avg 2.6/5, 10% pass rate (only 1 rated "Good")

## Key Files
```
.claude/commands/
  create-adventure.md    # /create-adventure - generates adventures
  eval-adventure.md      # /eval-adventure - rates adventures 1-5

.claude/skills/faerun-adventure-reference/
  SKILL.md               # Main skill definition
  faerun-lore.md         # Locations, factions, NPCs
  deities.md             # 30+ deities with temples, allies, hooks

evaluations/ratings.json # 10 rated adventures with feedback
tasks.md                 # Improvement roadmap
```

## Next Steps (from tasks.md)
**High Priority:**
- Fix DC calculation guidance (add easy/medium/hard labels)
- Add villain motivation requirement
- Complete story arcs (no cliffhangers)
- Create monsters.md with CR, regions, sourcebooks
- Add encounter building rules using XP budget

**Medium Priority:**
- Create names.md to avoid cliche names
- Avoid duplicating published adventures
- Add NPC detail requirements

## Key Issues Found in Evals
- Lore errors (dracolich from eggs, fictional locations)
- Missing villain motivations
- Encounter balance off (too easy or too hard)
- Incomplete stories / cliffhangers
- Cliche names ("Pip the halfling")

## What Worked
"The Drowned Grove" (Level 4, Moonshae Isles) got a 4 - good regional flavor, logical consistency, balanced encounters.
