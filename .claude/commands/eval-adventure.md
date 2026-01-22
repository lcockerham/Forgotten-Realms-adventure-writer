# Evaluate Adventures

Rate generated adventures for quality. This tool helps build a dataset of human evaluations.

## Rating Scale

| Score | Label | Description |
|-------|-------|-------------|
| 1 | Trash | Non-sensical, incoherent, unusable |
| 2 | AI Slop | Generic, formulaic, obviously machine-generated |
| 3 | Passable | Something a green DM would come up with, functional but uninspired |
| 4 | Good | Meets the bar for actually running at a table, solid adventure |
| 5 | Excellent | WotC publication quality, creative, polished, memorable |

## Evaluation Process

### Step 1: Find Unevaluated Adventures

1. Read the existing evaluations from `evaluations/ratings.json`
2. List all adventures in `generated-adventures/`
3. Identify adventures that haven't been evaluated yet
4. If all adventures are evaluated, inform the user and ask if they want to re-evaluate any

### Step 2: Display Adventure

For each unevaluated adventure:
1. Read the full adventure markdown file
2. Display it to the user in a readable format
3. Wait for their review

### Step 3: Collect Rating

Use AskUserQuestion to ask:
- **Rating (1-5)**: Using the scale above
- Then ask for **free-form feedback** (optional)

### Step 4: Save Evaluation

Save the evaluation to `evaluations/ratings.json` with:
```json
{
  "adventure_file": "the-adventure-name.md",
  "adventure_title": "The Adventure Name",
  "rating": 4,
  "feedback": "User's feedback here",
  "evaluated_at": "2024-01-15T10:30:00Z",
  "level": 7
}
```

### Step 5: Continue or Stop

After each evaluation, ask if the user wants to:
- Evaluate another adventure
- Stop and see summary statistics

## Summary Statistics

When requested or after completing all evaluations, display:
- Total adventures evaluated
- Average rating
- Rating distribution (how many 1s, 2s, 3s, etc.)
- List of adventures by rating tier

## File Structure

```
evaluations/
  ratings.json       # Array of all evaluations
```

## Notes

- Always read the current ratings.json before adding new evaluations
- Append new evaluations to the existing array
- If ratings.json doesn't exist, create it with an empty array
- Extract the adventure title and level from the adventure file when saving
