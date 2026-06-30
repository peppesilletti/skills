# CLAUDE.md

Conventions for working in this repo (a collection of Claude Code skills for product engineers).

## Layout

```
skills/<category>/<skill-name>/SKILL.md   # required: the skill itself
skills/<category>/<skill-name>/*          # optional: templates, assets the skill ships
.claude-plugin/plugin.json                # install manifest — MUST list every skill path
```

Categories follow the product-engineering loop: `discovery`, `planning`, `building`, `design`.

## Adding a skill

1. Create `skills/<category>/<skill-name>/SKILL.md` with YAML frontmatter:
   ```yaml
   ---
   name: <skill-name>
   description: <one line — what it does and when to use it>
   ---
   ```
2. Add the skill's path to the `skills` array in `.claude-plugin/plugin.json`.
3. Add a one-line entry under the right category in `README.md`, marked **user-invoked** or **model-invoked**.

## Writing skills

- Keep `SKILL.md` to instructions and contract; ship any scaffold (HTML templates, etc.) as sibling files the skill fills at runtime.
- Nothing in a shipped skill should be specific to one codebase — discover codebase specifics at runtime.
- Match the voice of the existing skills: concise, direct, plain language, no emojis.
