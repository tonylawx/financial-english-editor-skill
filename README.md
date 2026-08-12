# Financial English Editor Skill

A reusable agent skill for turning Chinese-language market commentary into natural, professional English for North American financial readers.

## What it solves

This skill is designed for Chinese writing about:

- US stocks and ETFs
- options and volatility
- macro and rates
- earnings and valuation
- sector rotation
- technical analysis
- daily market notes and investment newsletters

It focuses on **rewriting market meaning rather than translating Chinese syntax literally**.

Typical fixes include:

- `倒车接人` → `the pullback offers a better entry`
- `总开关` → `key signal / gating level`
- `不赌突破` → `wait for confirmation rather than front-run the breakout`
- `缩量横盘` → `consolidate on light volume`
- `接仓` → `take assignment`

## Installation

This repository follows the standard agent-skill layout. The main skill is [`SKILL.md`](./SKILL.md).

For runtimes that support shared agent skills, copy or symlink this repository into the runtime's skills directory, for example:

```bash
git clone https://github.com/tonylawx/financial-english-editor-skill.git
```

Then place it under the appropriate skills directory for your agent runtime.

## Suggested usage

Ask the agent to use the `financial-english-editor` skill when translating or rewriting Chinese financial content into English.

Example prompt:

```text
Use the financial-english-editor skill to rewrite this Chinese market note into native English. Use newsletter mode. Preserve every ticker, number, price level, catalyst, risk, and degree of conviction.
```

## Editing modes

- `faithful` — maximum fidelity, minimal stylistic change
- `native` — default; natural North American market English
- `newsletter` — sharper pacing and headings
- `research-note` — neutral institutional tone
- `social` — concise financial English for X/Twitter

## Core rule

> Translate the market meaning, not the Chinese wording.

## License

Use and adapt freely for your own agent workflows.
