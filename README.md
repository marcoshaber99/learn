# Learn

A Claude Code plugin that turns mistakes into rules.

When Claude makes a mistake, you can tell it what went wrong. This plugin investigates the error, comes up with a rule to prevent it, and saves it to your `CLAUDE.md`.

## Commands

**`/learn:from`** — After Claude makes a mistake
```
/learn:from
```

Paste the error or describe what went wrong. The plugin investigates, proposes a rule, and adds it to your CLAUDE.md.

**`/learn:list`** — See what your project has learned

**`/learn:remove`** — Remove a rule that's outdated or wrong

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

Boris Cherny (creator of Claude Code) mentioned that his team manually adds rules to CLAUDE.md after mistakes:

> "Anytime we see Claude do something incorrectly we add it to the CLAUDE.md, so Claude knows not to do it next time."

This plugin turns that into a command.


## Contributing
Issues/PRs welcome!
