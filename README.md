# Or's Skills

Generic, reusable skills for AI agents.

![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)

## What is a skill?

A skill is a folder containing a `SKILL.md` file: a name, a short description of when to use it, and the instructions the agent should follow. The agent loads a skill when the current task matches its description, so each skill adds a repeatable workflow without bloating every conversation.

## Skills

| Skill | What it does | Triggers when |
|---|---|---|
| [`skill-template`](skills/skill-template/SKILL.md) | Starting point for writing a new skill | You want to create your own skill |

More skills are coming.

## Usage

Copy a skill folder into your agent's skills directory, then restart the agent. For Claude Code:

```bash
# personal (all projects)
cp -r skills/<skill-name> ~/.claude/skills/

# or per project
cp -r skills/<skill-name> <your-project>/.claude/skills/
```

## Repository layout

```
skills/
  <skill-name>/
    SKILL.md        # required: frontmatter + instructions
    scripts/        # optional helpers
    references/     # optional extra docs
```

## Writing your own

Start from [`skills/skill-template`](skills/skill-template/SKILL.md). Guidelines:

- Write the `description` so it says clearly *when* the skill applies.
- Keep instructions short, concrete and step-by-step.
- Keep skills generic: no secrets, personal data, internal URLs or company names.

## Contributing

Issues and pull requests are welcome.

## License

[MIT](LICENSE)
