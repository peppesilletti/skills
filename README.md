# Skills For Modern Product Engineers

A collection of [Claude Code](https://claude.com/claude-code) skills for the way modern product engineers actually work — moving from a hunch to a shipped feature without losing product sense, design taste, or engineering rigor along the way.

These are pulled from my own daily practice. Each one encodes a piece of craft I'd otherwise have to re-explain to an agent from scratch every time.

## Quick start

```bash
npx skills@latest add peppesilletti/skills
```

Pick the skills and the coding agent you want, and you're set. Then invoke a skill by name — e.g. `/feature-plan`.

## The skills

Organized by where they sit in the product-engineering loop: **discovery → planning → building → design**.

### Planning

**User-invoked**

- **`feature-plan`** — Turns a feature concept into a single self-contained, interactive HTML planning artifact: what it feels like, a story map of shippable slices, the system structure grounded in your actual codebase, and the open decisions worth surfacing.

> Discovery, building, and design categories will fill in as more skills land.

## Repository layout

```
skills/<category>/<skill-name>/SKILL.md   # one folder per skill
.claude-plugin/plugin.json                # install manifest (lists every skill)
```

## License

[MIT](./LICENSE) © Peppe Silletti
