# Adventure Validation Checklist

Run this checklist after generating an adventure and BEFORE saving. Each check addresses issues found in evaluated adventures.

## How to Use

1. Complete all checks in order
2. Mark each as PASS, WARN, or FAIL
3. Fix all FAIL items before saving
4. Address WARN items if possible
5. Document any exceptions in the adventure notes

---

## 1. Mechanical Validation

### 1.1 DC Calculation Check
**Issue caught**: "DCs are wrong", "DCs are too high, even for 15th level"

For each DC in the adventure:
- [ ] Calculate expected DC: Easy = 8 + level, Medium = 10 + level, Hard = 12 + level
- [ ] Verify each DC falls within appropriate range for stated difficulty
- [ ] Add difficulty label in parentheses: "DC 15 (Medium) Dexterity saving throw"

**Validation table** (for 4 common levels):

| Level | Easy | Medium | Hard |
|-------|------|--------|------|
| 3 | 11 | 13 | 15 |
| 5 | 13 | 15 | 17 |
| 10 | 18 | 20 | 22 |
| 15 | 23 | 25 | 27 |

FAIL if: Any DC is 5+ points outside expected range without justification

### 1.2 Encounter Balance Check
**Issue caught**: "Imps at 12th level is a walkover"

For each combat encounter:
- [ ] Calculate XP budget from [monsters.md](monsters.md): Budget = (per-character value) × 4
- [ ] Sum XP of all monsters in encounter
- [ ] Verify total is within Low/Moderate/High range for party level
- [ ] Flag if main encounter uses less than 30% of Moderate budget

**Quick reference** (Moderate difficulty, 4 PCs):

| Level | XP Budget | Example Valid Encounter |
|-------|-----------|------------------------|
| 3 | 900 | 1 Wight (700) + 2 Skeletons (100) |
| 5 | 3,000 | 1 Troll (1,800) + 2 Ogres (900) |
| 10 | 9,200 | 1 Young Red Dragon (5,900) + 2 Veterans (1,400) |
| 12 | 14,800 | 1 Beholder (10,000) + 4 Spectators (2,800) |
| 15 | 21,600 | 1 Adult Blue Dragon (15,000) + 2 Wyverns (4,600) |

FAIL if: Main combat encounter XP is less than 50% of Low difficulty budget

### 1.3 Monster Selection Check
**Issue caught**: Regional/thematic mismatch

For each monster:
- [ ] Verify monster exists in [monsters.md](monsters.md) or official source
- [ ] Check regional fit matches adventure location
- [ ] Confirm CR is within ±3 of party level (±5 for minions)

FAIL if: Monster doesn't exist or is wildly inappropriate for region

---

## 2. Lore Validation

### 2.1 Location Accuracy Check
**Issue caught**: "I don't think there is even a dragon hatchery in Cormyr"

- [ ] Verify main location exists in [faerun-lore.md](faerun-lore.md) or established canon
- [ ] Check that location features match canon (e.g., Waterdeep has Undermountain, not volcanoes)
- [ ] Verify regional culture is appropriate (Calimshan = genies/pashas, Cormyr = Purple Dragons)

FAIL if: Invented major location presented as canonical, or major feature contradicts canon

### 2.2 Deity Accuracy Check
- [ ] Verify deity exists in [deities.md](deities.md)
- [ ] Check deity's portfolio matches their role in adventure
- [ ] Verify temple locations are plausible for the region
- [ ] Confirm ally/enemy relationships are accurate

FAIL if: Deity used with wrong portfolio or impossible temple location

### 2.3 Faction Accuracy Check
- [ ] Verify faction exists in [faerun-lore.md](faerun-lore.md)
- [ ] Check faction goals match their actions in adventure
- [ ] Confirm faction presence is plausible in adventure location

FAIL if: Faction acts completely against their established goals without explanation

### 2.4 Monster Lore Check
**Issue caught**: "You can't make a dracolich from a dragon egg!"

- [ ] Verify monster creation/origin follows established lore
- [ ] Check monster behavior matches canon (e.g., beholders are paranoid, mind flayers eat brains)
- [ ] Confirm monster ecology makes sense for location

FAIL if: Monster origin or behavior directly contradicts Monster Manual lore

---

## 3. Story Validation

### 3.1 Villain Motivation Check
**Issue caught**: "Why are the yuan-ti tunneling?", "Why does Tam offer a gift?"

- [ ] Identify the main villain/antagonist
- [ ] State their motivation in one sentence: "The villain wants _____ because _____"
- [ ] Verify at least one encounter directly relates to this motivation
- [ ] Check that villain actions logically follow from motivation

FAIL if: Cannot state villain motivation, or actions don't match stated goal

### 3.2 Story Arc Completion Check
**Issue caught**: "The rat doesn't seem to do anything. My group would feel left hanging."

- [ ] Hook presents a clear problem or mystery
- [ ] Encounters progress toward resolution
- [ ] Adventure has a satisfying conclusion (not a cliffhanger)
- [ ] All introduced elements pay off (no dangling Chekhov's guns)

Checklist for dangling elements:
- [ ] Every mentioned NPC serves a purpose or is encountered
- [ ] Every introduced item/artifact is used or explained
- [ ] The main threat is resolved, not just delayed

FAIL if: Major plot element introduced but never resolved

### 3.3 Logic Consistency Check
**Issue caught**: "If the PCs have the contract already, why would the bone devil offer a deal?"

- [ ] Read through adventure as a player would experience it
- [ ] Check: Does the villain's offer make sense given what PCs already have/know?
- [ ] Check: Would PCs have reason to continue after each encounter?
- [ ] Check: Are there obvious solutions the adventure ignores?

FAIL if: Clear logical hole that players would immediately notice

---

## 4. NPC Validation

### 4.1 Key NPC Detail Check
**Issue caught**: "Would have liked details about the three sons"

For each NPC mentioned more than once:
- [ ] NPC has a name (not just "the guard" or "the merchant")
- [ ] NPC has at least one distinguishing detail (appearance, mannerism, or motivation)
- [ ] If NPC group mentioned (e.g., "three sons"), at least 2 individuals described

WARN if: Key NPC lacks distinguishing details

### 4.2 Name Quality Check
**Issue caught**: "Pip is a very cliche name for a halfling"

- [ ] No overly cliche names (Pip, Bramble for halflings; Thorin, Gimli for dwarves)
- [ ] Names fit the regional culture (Calimshan = Arabic-inspired, Cormyr = European)
- [ ] Villain names are memorable but not cartoonish

WARN if: Names feel lazy or cliche

---

## 5. Originality Validation

### 5.1 Published Adventure Overlap Check
**Issue caught**: "Xanathar heist adventure feels duplicative of Dragon Heist"

Review for similarity to major published adventures:
- [ ] **Dragon Heist**: Waterdeep treasure hunt, Xanathar/Cassalanters/Jarlaxle villains
- [ ] **Curse of Strahd**: Gothic horror, vampire lord, Barovia
- [ ] **Tomb of Annihilation**: Chult, death curse, Acererak
- [ ] **Storm King's Thunder**: Giant uprising, Ordning broken
- [ ] **Descent into Avernus**: Baldur's Gate, hellish road trip
- [ ] **Rime of the Frostmaiden**: Icewind Dale, eternal winter, Auril

WARN if: Adventure closely mirrors a published module's core premise

---

## 6. Format Validation

### 6.1 Length Check
- [ ] Adventure fits on one page when formatted
- [ ] Hook is 2-3 sentences maximum
- [ ] Each encounter bullet is 1-2 sentences
- [ ] Room descriptions are 1-3 sentences each

WARN if: Adventure runs significantly over one page

### 6.2 Mechanics Format Check
- [ ] Monster names are bolded
- [ ] DCs include skill/ability: "DC 14 Wisdom (Perception) check"
- [ ] Saving throws include damage: "DC 15 Dexterity saving throw, taking 3d10 fire damage on a failed save"
- [ ] Level is clearly stated in header

FAIL if: Mechanics are ambiguous or incomplete

---

## Validation Summary Template

After running all checks, summarize:

```
VALIDATION SUMMARY
==================
Adventure: [Title]
Level: [X]
Validator: [Claude/Human]
Date: [Date]

MECHANICAL
- DC Check: [PASS/WARN/FAIL] - [notes]
- Encounter Balance: [PASS/WARN/FAIL] - XP: [X] vs Budget: [Y]
- Monster Selection: [PASS/WARN/FAIL] - [notes]

LORE
- Location: [PASS/WARN/FAIL] - [notes]
- Deity: [PASS/WARN/FAIL] - [notes]
- Faction: [PASS/WARN/FAIL] - [notes]
- Monster Lore: [PASS/WARN/FAIL] - [notes]

STORY
- Villain Motivation: [PASS/WARN/FAIL] - Motivation: "[statement]"
- Story Arc: [PASS/WARN/FAIL] - [notes]
- Logic: [PASS/WARN/FAIL] - [notes]

NPC
- Key NPCs: [PASS/WARN/FAIL] - [notes]
- Names: [PASS/WARN/FAIL] - [notes]

ORIGINALITY
- Published Overlap: [PASS/WARN/FAIL] - [notes]

FORMAT
- Length: [PASS/WARN/FAIL]
- Mechanics Format: [PASS/WARN/FAIL]

OVERALL: [PASS - Ready to save / NEEDS FIXES / MAJOR REVISION REQUIRED]
Fixes needed: [list]
```

---

## Quick Pre-Save Checklist

Before saving, confirm these critical items:

1. [ ] Villain has clear motivation stated or implied
2. [ ] Main combat encounter XP is appropriate for level
3. [ ] All DCs have difficulty labels (Easy/Medium/Hard)
4. [ ] Story has a resolution, not a cliffhanger
5. [ ] No major lore violations
6. [ ] All mentioned NPCs/items serve a purpose
