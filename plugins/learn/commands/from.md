---
description: Learn from a mistake and add a rule to CLAUDE.md
---

The user encountered an issue with code you generated. Your job is to analyze what went wrong and propose a rule for CLAUDE.md so this mistake doesn't happen again.

## Step 1: Understand the mistake

If `$ARGUMENTS` is provided, that describes the mistake or contains the error.

If not, ask: "What went wrong? Paste the error or describe the issue."

## Step 2: Investigate

- Run `git diff` to see recent changes
- Look at the relevant files
- Understand the pattern that caused the issue

## Step 3: Propose a rule

Write a concise rule that would prevent this mistake. Good rules are:
- Specific, not vague ("Use `satisfies` instead of `as` for type objects" not "Be careful with types")
- Short (1-2 sentences max)
- Actionable (tells what TO do, not just what not to do)

## Step 4: Check for duplicates

Read the existing `## Learned Rules` section in CLAUDE.md.

If a similar rule already exists, tell the user:
```
A similar rule already exists:

> [existing rule]

Your new rule:

> [proposed rule]

Still add it? (yes/no)
```

If the user says no, stop here.

## Step 5: Present for approval

Show the user:
```
Proposed rule:

> [the rule]

Add to CLAUDE.md? (yes/no)
```

## Step 6: If approved

Add the rule to the `## Learned Rules` section in CLAUDE.md.

If the section doesn't exist, create it at the end of the file:
```markdown
## Learned Rules

Rules added via `/learn:from` after mistakes:

- [the rule]
```

If it exists, append the new rule as a bullet point.

Confirm: "Added to CLAUDE.md. This mistake won't happen again."