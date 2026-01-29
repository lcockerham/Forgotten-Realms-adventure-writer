# Faerun Adventure Writer - Project Summary

## What It Is
A Claude Code skill for generating one-page D&D adventures set in the Forgotten Realms. Includes commands for adventure generation and quality evaluation.

## Repository
`https://github.com/lcockerham/Forgotten-Realms-adventure-writer`

## Current State
- **20 adventures evaluated** across two batches
- **Overall avg: 3.1/5**, up from 2.6/5 in batch 1
- **Batch 2 results**: avg 3.6/5, 70% pass rate (7/10 rated "Good"), zero failures
- **8 adventures rated "Good" (4/5)**, none yet at "Excellent" (5/5)

## Key Files
```
.claude/commands/
  create-adventure.md    # /create-adventure - generates adventures
  eval-adventure.md      # /eval-adventure - rates adventures 1-5

.claude/skills/faerun-adventure-reference/
  SKILL.md               # Main skill definition
  faerun-lore.md         # Locations, factions, NPCs
  deities.md             # 30+ deities with temples, allies, hooks
  monsters.md            # Monster reference with CR, regions, XP
  validation-checklist.md # Pre-save quality checks
  names.md               # Canonical Faerunian names by 22 cultures

evaluations/ratings.json # 20 rated adventures with feedback
tasks.md                 # Improvement roadmap
generated-adventures/    # 10 generated adventures from batch 2
```

## Batch Comparison
| Metric | Batch 1 | Batch 2 |
|--------|---------|---------|
| Avg Rating | 2.6 | 3.6 |
| Pass Rate (4+) | 10% | 70% |
| Fail Rate (2-) | 40% | 0% |

## Improvements Made Since Batch 1
- monsters.md with CR, regions, XP values
- validation-checklist.md with critical checks (villain motivation, encounter balance, DC labels, story resolution, lore accuracy, Chekhov's gun)
- names.md with canonical names organized by 22 cultures/languages
- Encounter building rules using XP budget
- DC labels (easy/medium/hard) required

## Next Steps (from tasks.md)
**High Priority:**
- Fix eval rating option order (keyboard shortcuts don't match rating numbers)

**Medium Priority:**
- Monster reskinning guidance
- PC integration hooks (tie to backstories)

## Recurring Issues Still to Address
- Em dashes signal AI writing style; need style rule to ban them
- Encounter math calculated across whole adventure, not per-encounter; bosses often under-CR for party level
- Hallucinated locations (e.g., Mount Sulaer)
- Monster naming confusion (multiple names before actual stat block)
- Other-setting terms leak in ("The Dreaming Dark" is Eberron)
- Punishing entry mechanics (DC 22 + 2 exhaustion levels can break adventures)
- Avoid the word "slaves" in adventures
- Consider published adventure crossover handling (Gralhunds from Dragon Heist)

## Top Performers
- "The Drowned Grove" (Level 4, Moonshae Isles) - 4/5, good regional flavor and balanced encounters
- "The Clockwork Inheritance" (Level 4, Waterdeep) - 4/5, reminiscent of Keys from the Golden Vault
- "The Serpent's Masquerade" (Level 10, Waterdeep) - 4/5, strong Dendar lore and Gralhund crossover
- "The Last Crusade" (Level 12, Thunder Peaks) - 4/5, compelling redemption arc
