# Faerun Adventure Writer

A Claude Code skill for generating one-page D&D adventures set in the Forgotten Realms. Create ready-to-run adventures with proper mechanics, lore integration, and table-ready format.

## Features

- **One-Page Format**: Adventures designed to fit on a single page for easy table reference
- **Faerun Integration**: Built-in lore references for deities, factions, locations, and NPCs
- **Mechanical Guidelines**: Level-appropriate DCs, damage ranges, and encounter balance
- **Room-by-Room Details**: Clear location breakdowns with monsters, traps, and treasure
- **Evaluation System**: Rate and track adventure quality with structured feedback

## Commands

| Command | Description |
|---------|-------------|
| `/create-adventure` | Generate a new one-page adventure with guided prompts |
| `/eval-adventure` | Rate generated adventures and collect feedback |

## Installation

Clone this repository and copy the `.claude` folder to your project:

```bash
git clone https://github.com/YOUR_USERNAME/faerun-adventure-writer.git
cp -r faerun-adventure-writer/.claude /your/project/
```

Or add as a git submodule for easy updates.

## Usage

### Generate an Adventure

```
/create-adventure
```

You'll be prompted for:
- **Level** (1-20, or random)
- **Theme** (combat, investigation, social, balanced)
- **Location** (specific region or surprise)

The adventure is saved to `generated-adventures/`.

### Evaluate Adventures

```
/eval-adventure
```

Rate adventures 1-5:
| Score | Label | Description |
|-------|-------|-------------|
| 1 | Trash | Non-sensical, unusable |
| 2 | AI Slop | Generic, obviously machine-generated |
| 3 | Passable | Functional but uninspired |
| 4 | Good | Would run at a table |
| 5 | Excellent | Publication quality |

Evaluations are saved to `evaluations/ratings.json`.

## Project Structure

```
.claude/
├── commands/
│   ├── create-adventure.md    # Adventure generation command
│   └── eval-adventure.md      # Evaluation command
└── skills/
    └── faerun-adventure-reference/
        ├── SKILL.md           # Main skill definition
        ├── faerun-lore.md     # Locations, factions, NPCs
        ├── deities.md         # Detailed deity reference
        ├── examples.md        # Sample adventures
        └── evaluation-rubric.md

generated-adventures/          # Output folder (gitignored)
evaluations/                   # Rating data (gitignored)
tasks.md                       # Improvement roadmap
```

## Lore References

The skill includes curated Faerun lore for authentic adventures:

- **Regions**: Sword Coast, Dalelands, Calimshan, Chult, Thay, and more
- **Cities**: Waterdeep, Neverwinter, Baldur's Gate, Calimport, Suzail
- **Factions**: Harpers, Zhentarim, Emerald Enclave, Cult of the Dragon
- **Deities**: 30+ deities with temples, allies, foes, and adventure hooks

## Roadmap

See `tasks.md` for planned improvements including:
- Monster reference with CR and regional data
- Encounter building rules
- Name generation tables
- Logical consistency checks

## Contributing

Contributions welcome! Key areas:
- Lore accuracy improvements
- Additional regional content
- Mechanical balance feedback
- Example adventures

## License

MIT License - See LICENSE file

## Acknowledgments

Inspired by the Forgotten Realms setting and one-page adventure format.
