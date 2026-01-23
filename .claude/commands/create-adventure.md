# Create Faerun Adventure

Generate a one-page D&D adventure set in Faerun. Follow these steps in order:

## Step 1: Gather Requirements

Ask the user for the following (if not already provided):
- **Target level**: What level party is this for? If not specified, pick a random level 1-20
- **Theme preference**: Combat-heavy, investigation, social intrigue, exploration, or balanced?
- **Location preference**: Specific region/city, or "surprise me"
- **Any specific elements**: Faction, deity, monster type, or story element they want included?

**Note:** If the user doesn't specify a level, randomly select one from 1-20 and announce it at the start.

## Step 2: Consult Lore References

Before writing, review:
- `.claude/skills/faerun-adventure-reference/faerun-lore.md` for locations, factions, and cultural details
- `.claude/skills/faerun-adventure-reference/deities.md` for deity-specific hooks and themes

Select elements that work together:
1. Pick a **location** appropriate for the adventure
2. Choose a **faction** (ally or villain)
3. Select a **deity** for thematic connection
4. Identify **monsters** appropriate to the region and level

## Step 3: Design the Adventure Structure

Follow the template from SKILL.md:

### Header
- Create an evocative title (e.g., "The Whispers of Thornhold")
- Write a tagline with level indicator
- State the target level clearly

### Hook (2-3 sentences)
- Establish the immediate problem
- Connect to chosen Faerun lore elements
- Create urgency

### Encounters (3-5 bullets)
Design a mix of:
- 1 main combat encounter (level-appropriate)
- 1-2 investigation/exploration moments
- 1 trap or puzzle
- 1 social or story element

### Location Details
- Name and describe the adventure location
- Create room-by-room breakdown with:
  - Room names and descriptions
  - Encounters with full mechanics
  - Interactables and connections

## Step 4: Apply Mechanical Guidelines

Use level-appropriate values:

**DCs:**
- Easy: 8 + level
- Medium: 10 + level
- Hard: 12 + level

**Damage (per tier):**
- Levels 1-4: 1d10 nuisance / 2d10 deadly
- Levels 5-10: 2d10 nuisance / 4d10 deadly
- Levels 11-16: 4d10 nuisance / 10d10 deadly
- Levels 17-20: 10d10 nuisance / 18d10 deadly

**Format mechanics inline:**
- "DC 14 Wisdom (Perception) check"
- "DC 12 Dexterity saving throw, taking 2d10 fire damage on a failed save"
- Bold monster names: "A **Specter** guards the entrance"

## Step 5: Write the Adventure

Compose the full adventure using:
- **Concise language**: Every word counts
- **Active voice**: "A cultist stands guard" not "There is a cultist"
- **Evocative details**: Atmosphere in few words
- **Clear mechanics**: No ambiguity

## Step 6: Run Validation Checklist

Before saving, run through `.claude/skills/faerun-adventure-reference/validation-checklist.md`:

### Critical Checks (must PASS)
- [ ] **Villain Motivation**: Can state "The villain wants _____ because _____"
- [ ] **Encounter Balance**: Main combat XP is within budget (see [monsters.md](../skills/faerun-adventure-reference/monsters.md))
- [ ] **DC Labels**: All DCs include difficulty label: "DC 15 (Medium) Dexterity saving throw"
- [ ] **Story Resolution**: Adventure ends, not cliffhangs
- [ ] **Lore Accuracy**: No invented locations, correct deity portfolios, valid monster origins
- [ ] **Chekhov's Gun**: Every introduced element (NPC, item, mystery) pays off

### Quick Calculations
1. **DCs**: Easy = 8 + level, Medium = 10 + level, Hard = 12 + level
2. **XP Budget** (Moderate, 4 PCs): Look up level in monsters.md, multiply by 4
3. **Main encounter**: Should use 50-70% of budget

### Format Checks
- [ ] Fits one-page format
- [ ] Monster names bolded
- [ ] Mechanics complete (DC + skill + damage + save effect)
- [ ] Level clearly stated

If any critical check fails, fix before proceeding to Step 7.

## Step 7: Save the Adventure

Save the completed adventure as a markdown file:
- **Location**: `generated-adventures/` folder in the project root
- **Filename**: Use kebab-case of the adventure title (e.g., `the-obsidian-sundial.md`)
- Create the `generated-adventures/` folder if it doesn't exist

## Output Format

Save the adventure using this format:

```
# [Adventure Title]
**[Tagline]** | Level [X]

## Hook
[2-3 sentence hook]

## Encounters
- [Encounter 1]
- [Encounter 2]
- [Encounter 3]
- [etc.]

## [Location Name]
[Brief location description]

### [Room 1 Name]
[Description, encounters, interactables]

### [Room 2 Name]
[Description, encounters, interactables]

[etc.]
```

After saving, inform the user of the file path.
