# Faerun Adventure Writer

**⚠️ Early Development Notice**: This project is in very early stages. Expect significant changes to the skill structure, templates, and generation logic as the tool evolves.

A Claude Code skill for generating high-quality one-page D&D adventures set in the Forgotten Realms (Faerun). Create ready-to-run adventures with proper mechanics, lore integration, and table-ready format.

## Features

- **One-Page Format**: Adventures designed to fit on a single page for easy reference at the table
- **Faerun Integration**: Built-in lore references for deities, factions, locations, and NPCs
- **Complete Mechanics**: Proper DCs, damage ranges, and encounter balance by level
- **Room-by-Room Details**: Clear location breakdowns with monsters, traps, and treasure
- **Quality Guidelines**: Structure templates and evaluation rubrics for consistent quality

## Installation

This is a Claude Code skill. To use it:

1. Clone this repository into your Claude Code skills directory:
   ```bash
   cd ~/.claude/skills  # or your skills directory
   git clone <your-repo-url> faerun-adventure-reference
   ```

2. The skill will be available as `/faerun-adventure-reference` in Claude Code

## Usage

In Claude Code, invoke the skill to:

- **Generate adventures**: `use the faerun-adventure-reference skill to generate an adventure`
- **Evaluate adventures**: Provide an adventure text and ask for evaluation
- **Check lore accuracy**: Verify Faerun details in your content

## Adventure Structure

Each generated adventure includes:

- **Hook**: 2-3 sentence setup tied to Faerun lore
- **Key Encounters**: Bulleted list of 3-5 main challenges
- **Location Details**: Room-by-room breakdown with mechanics
- **Treasure & Rewards**: Appropriate loot for the level

## Project Structure

```
.claude/skills/faerun-adventure-reference/
├── SKILL.md              # Main skill definition and instructions
├── faerun-lore.md        # Reference for Forgotten Realms content
├── examples.md           # Sample adventures with annotations
└── evaluation-rubric.md  # Quality assessment criteria

generated-adventures/     # Output folder (gitignored)
```

## Customization

The skill can be modified to:
- Add new location templates
- Include additional Faerun lore references
- Adjust mechanical guidelines for different play styles
- Create adventures for specific campaigns or themes

## Contributing

This project is in active development. Contributions, suggestions, and feedback are welcome as the skill evolves.

## License

MIT License - See LICENSE file for details

## Acknowledgments

Inspired by "Adventures in Faerun" and the rich lore of the Forgotten Realms setting.
