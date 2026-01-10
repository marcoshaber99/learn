# Learn

A Claude Code plugin that turns mistakes into CLAUDE.md rules.

## The Idea

Claude makes the same mistakes until you tell it not to. This plugin captures those lessons with a single command.

## Commands

**`/learn:from`** — After Claude makes a mistake
```
/learn:from You used any instead of a proper TypeScript interface
```

Investigates the mistake, proposes a rule, adds it to your CLAUDE.md.

**`/learn:list`** — See what your project has learned

## Installation
```bash
/plugin marketplace add marcoshaber99/learn
/plugin install learn@marcoshaber99-learn
```

## What Happens

Your CLAUDE.md grows a `## Learned Rules` section:
```markdown
## Learned Rules

- Always define explicit interfaces instead of using `any`.
- Use `satisfies` instead of `as` for type assertions on objects.
```

Every mistake becomes a rule. Your project gets smarter over time.

## Inspiration

Boris Cherny (creator of Claude Code) on his team's workflow:

> "Anytime we see Claude do something incorrectly we add it to the CLAUDE.md, so Claude knows not to do it next time."

This plugin turns that into a command.

## License

MIT