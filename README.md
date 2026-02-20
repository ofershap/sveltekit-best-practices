# SvelteKit Best Practices

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Skills](https://img.shields.io/badge/skills.sh-sveltekit--best--practices-blue)](https://skills.sh/ofershap/sveltekit-best-practices)

SvelteKit and Svelte 5 done right. Runes (`$state`, `$derived`, `$effect`), `$props()`,
`$bindable()`, load functions, form actions, `+page.server.ts`, `+layout.server.ts`,
`hooks.server.ts`, snippets, and SSR patterns.

> AI coding assistants generate Svelte 4 code - `writable()` stores, `export let` props, `$:`
> reactive declarations, `onMount` data fetching. Svelte 5 replaced all of these with runes. This
> plugin stops your agent from writing dead syntax.

## Install

### Cursor / Claude Code / Windsurf

```bash
npx skills add ofershap/sveltekit-best-practices
```

Or copy `skills/` into your `.cursor/skills/` or `.claude/skills/` directory.

## What's Included

| Type    | Name                       | Description                                                              |
| ------- | -------------------------- | ------------------------------------------------------------------------ |
| Skill   | `sveltekit-best-practices` | 14 rules for Svelte 5 runes, load functions, form actions, SSR, and more |
| Rule    | `best-practices`           | Always-on behavioral rule that enforces Svelte 5 / SvelteKit patterns    |
| Command | `/audit`                   | Scan your codebase for Svelte 4 anti-patterns                            |

## What Agents Get Wrong

| What the agent writes (Svelte 4)  | What Svelte 5 uses                   |
| --------------------------------- | ------------------------------------ |
| `writable()`, `readable()` stores | `$state()`, `$derived()` runes       |
| `export let name` for props       | `let { name } = $props()`            |
| `$: doubled = count * 2`          | `let doubled = $derived(count * 2)`  |
| `$: { sideEffect() }`             | `$effect(() => { sideEffect() })`    |
| Data fetching in `onMount`        | `load()` in `+page.server.ts`        |
| API routes for form mutations     | Form actions in `+page.server.ts`    |
| `<slot />` for children           | Snippets with `{@render children()}` |
| `$app/stores` for page data       | `$app/state` (Svelte 5)              |

## Related Plugins

- [tailwind-best-practices](https://github.com/ofershap/tailwind-best-practices) - Tailwind CSS v4
  patterns
- [typescript-best-practices](https://github.com/ofershap/typescript-best-practices) - TypeScript
  5.x strict patterns
- [vibe-guard](https://github.com/ofershap/vibe-guard) - Security guardrails for SvelteKit endpoints

## Author

[![Made by ofershap](https://gitshow.dev/api/card/ofershap)](https://gitshow.dev/ofershap)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/ofershap)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github&logoColor=white)](https://github.com/ofershap)

## License

MIT
