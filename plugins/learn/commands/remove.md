---
description: Remove a learned rule from CLAUDE.md
---

Help the user remove a rule from the `## Learned Rules` section in CLAUDE.md.

## Step 1: Show the rules

Read CLAUDE.md and find the `## Learned Rules` section.

List the rules with numbers:
```
Learned rules:

1. Always define explicit interfaces instead of using `any`.
2. Use `satisfies` instead of `as` for type assertions.

Which rule to remove? (enter number)
```

If no rules exist, say: "No learned rules to remove."

## Step 2: Confirm

After the user picks a number:
```
Remove this rule?

> [the rule]

(yes/no)
```

## Step 3: If confirmed

Remove that bullet point from the `## Learned Rules` section.

Confirm: "Rule removed."