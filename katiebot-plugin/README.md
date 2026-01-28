# KatieBot

Editorial coaching agent that reviews ideas, outlines, and drafts according to Katie Parrott's writing principles.

## Philosophy

KatieBot is Socratic but opinionated—asks hard questions while maintaining a clear point of view. Every piece must be:

- **New**: Fresh perspective the reader didn't already have
- **True**: Writer is authentically present, not performing
- **Useful**: Reader walks away with something

## Skills

| Skill | Description |
|-------|-------------|
| `katiebot` | Full editorial coaching—stage-aware feedback from brainstorming through revision |
| `eli5` | Check writing for clarity—flags jargon, hand-waving, skipped steps |
| `asshole-read` | Stress-test with the meanest, least-charitable reading |
| `angle-finder` | Generate five distinct angles when you're stuck |

## Commands

| Command | Description |
|---------|-------------|
| `/katiebot` | Editorial coaching with Katie's principles |
| `/eli5` | Check writing for clarity |
| `/asshole-read` | Hard feedback mode |
| `/angle-finder` | Generate alternative angles |

## Installation

Add to your Claude Code plugins:

```bash
claude plugins add every-marketplace/katiebot
```

## Usage

### Full Editorial Review

```
/katiebot [paste your draft]
```

KatieBot will:
1. Detect what stage you're in (brainstorming, outlining, drafting, revising)
2. Calibrate feedback accordingly
3. Check against New/True/Useful
4. Look for buried insights, structural issues, stakes
5. Express graduated confidence (close → there → done)

### Quick Tools

```
/eli5 [draft]        # Find clarity issues
/asshole-read [draft] # Stress-test the piece
/angle-finder [topic] # Get unstuck with new angles
```

## Writer Model

KatieBot can track your patterns over time. Create a `.katiebot/` folder in your project with:

- `writer-model.md` — Your strengths, patterns to watch, signature moves
- `style-guide.md` — Your confirmed style rules

Templates are provided in `skills/katiebot/templates/`.

## Integration

KatieBot focuses on developmental and structural feedback. For mechanical style:
- `ai-check` handles AI tells
- `every-style` handles grammar and Every house rules

These auto-trigger on Every content.

## License

MIT
