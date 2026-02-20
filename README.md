# SvelteKit Best Practices

SvelteKit and Svelte 5 done right. Runes ($state, $derived, $effect), load functions, form actions, SSR patterns, and modern Svelte your AI agent should follow.

## Install

### Cursor IDE

```
/add-plugin sveltekit-best-practices
```

### Claude Code

```
/plugin install sveltekit-best-practices
```

### Skills only (any agent)

```bash
npx skills add ofershap/sveltekit-best-practices/sveltekit-best-practices
```

Or copy `skills/` into your `.cursor/skills/` or `.claude/skills/` directory.

## What's Included

### Skills

- **sveltekit-best-practices** - SvelteKit and Svelte 5 done right. Runes, load functions, form actions, SSR patterns, and modern Svelte.

### Rules

- **best-practices** - Always-on rules that enforce current SvelteKit / Svelte 5 patterns

### Commands

- `/audit` - Scan your codebase for SvelteKit / Svelte 5 anti-patterns

## Why This Plugin?

AI agents are trained on data that includes outdated Svelte 4 patterns. This plugin ensures your agent uses current Svelte 5 and SvelteKit best practices:

- Agents generate Svelte 4 stores (writable, readable) instead of Svelte 5 runes ($state, $derived, $effect)
- Agents use export let instead of $props() and $bindable()
- Agents use $: reactive declarations instead of $derived and $effect
- Agents fetch data in onMount instead of using load functions in +page.server.ts
- Agents create API routes for form submissions instead of using form actions

## License

MIT
