---
name: skill-template
description: Use when the user wants to create a new agent skill. Scaffolds a SKILL.md with frontmatter and clear, generic instructions.
---

# Skill template

Use this as a starting point for a new skill.

## Steps

1. Pick a short kebab-case name, e.g. `code-review-checklist`.
2. Create `skills/<name>/SKILL.md` with frontmatter:
   - `name`: same as the folder name.
   - `description`: one or two sentences saying *when* to use the skill. This is what the agent matches against, so be specific.
3. Write the body as concrete, ordered steps. Say what to do, what to check, and what the output should look like.
4. Add optional `scripts/` or `references/` only if the skill needs them.
5. Review for privacy: remove secrets, personal data, internal URLs and company names.
6. Add a row to the skills table in the root `README.md`.

## Checklist

- [ ] Description states the trigger clearly
- [ ] Instructions are short and actionable
- [ ] Nothing private or environment-specific
