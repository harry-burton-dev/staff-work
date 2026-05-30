# Contributing

## Adding a skill

1. Choose or create a category directory (`analysis/`, `style/`, etc.)
2. Create a subdirectory for your skill: `category/skill-name/`
3. Add a `SKILL.md` with the required frontmatter and body
4. Add your skill to the table in `README.md`
5. Open a PR

---

## Skill frontmatter

Every `SKILL.md` must open with:

```yaml
---
name: skill-name
description: "One paragraph. What the skill does, and every trigger phrase Claude should recognise — this is how Claude decides when to apply it automatically."
license: MIT
---
```

The `description` field is the most important line in the file. If it is vague or too narrow, the skill will not trigger reliably.

---

## Category guide

| Category | For skills that... |
|----------|-------------------|
| `analysis/` | Help think through problems, plan, or decide |
| `style/` | Improve how something is written or communicated |

If your skill does not fit an existing category, propose a new one in your PR with a one-line description of what belongs in it.

---

## Quality bar

A good skill:

- **Triggers reliably** — the description lists every phrase a user might say, not just the obvious ones
- **Consistent output** — produces the same format every time, so the user knows what to expect
- **Worked examples** — at least two examples in the skill body showing input → output
- **No padding** — every line in the skill earns its place; cut anything the model already knows

---

## Testing

Before submitting, test your skill with at least three different inputs covering normal use, edge cases, and ambiguous inputs. If you have eval infrastructure, include it alongside the skill (see `bluf-writer-workspace/` for the pattern).

---

## Maintaining skills

- **Trigger drift** — if a skill is not firing when it should, expand the `description` trigger list
- **Output drift** — if the model is ignoring the format, tighten the output spec and add a negative example
- **Deprecating a skill** — open a PR removing the skill and its README entry; do not leave dead stubs
