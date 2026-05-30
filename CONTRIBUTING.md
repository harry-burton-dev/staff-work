# Maintenance Guide

This is a personal skills library. It is not open for external contributions.

---

## Adding a skill

1. Choose or create a category directory (`analysis/`, `style/`, etc.)
2. Create a subdirectory: `category/skill-name/`
3. Add a `SKILL.md` with the required frontmatter and body
4. Add a row to the table in `README.md`
5. Commit and push

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

The `description` field is the most important line. If it is vague or too narrow, the skill will not trigger reliably.

---

## Category guide

| Category | For skills that... |
|----------|-------------------|
| `analysis/` | Help think through problems, plan, or decide |
| `style/` | Improve how something is written or communicated |

---

## Maintaining skills

- **Trigger not firing** — expand the `description` trigger list with more phrases
- **Output drifting** — tighten the output spec in the skill body and add a negative example
- **Deprecating a skill** — delete the directory and remove its row from the README

---

## Testing

Test any new or edited skill with at least three inputs: a normal case, an edge case, and an ambiguous one. See `bluf-writer-workspace/` for the eval pattern.
