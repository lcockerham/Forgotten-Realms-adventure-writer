# Adventure Evaluations

Human evaluations of generated Faerun adventures.

## Rating Scale

| Score | Label | Description |
|-------|-------|-------------|
| 1 | Trash | Non-sensical, incoherent, unusable |
| 2 | AI Slop | Generic, formulaic, obviously machine-generated |
| 3 | Passable | Something a green DM would come up with, functional but uninspired |
| 4 | Good | Meets the bar for actually running at a table, solid adventure |
| 5 | Excellent | WotC publication quality, creative, polished, memorable |

## Files

- `ratings.json` - Array of all adventure evaluations

## Evaluation Schema

```json
{
  "adventure_file": "the-adventure-name.md",
  "adventure_title": "The Adventure Name",
  "rating": 4,
  "feedback": "Optional user feedback",
  "evaluated_at": "ISO 8601 timestamp",
  "level": 7
}
```

## Usage

Run `/eval-adventure` to start evaluating adventures.
