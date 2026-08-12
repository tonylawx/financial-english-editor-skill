---
name: financial-english-editor
description: Use when translating or rewriting Chinese-language financial market commentary, investment research, trading notes, stock/ETF/options analysis, macro commentary, technical analysis, or awkward English financial drafts for North American market readers.
---

# Financial English Editor

## Overview

Turn Chinese financial writing or awkward translated English into natural, publication-ready market English. Preserve the investment thesis, facts, numbers, tickers, levels, catalysts, risks, chronology, and positioning, then rebuild the prose in idiomatic financial English.

Core principle: **translate the market meaning, not the Chinese wording.**

## Scope Check

Before editing, classify the piece.

Use this skill for:
- US stocks, ETFs, options, macro, earnings, sectors, rates, flows, positioning, and technical analysis
- Daily market notes, newsletters, investment blogs, trading journals, research summaries, and financial social posts
- English drafts that are grammatically correct but sound translated, robotic, sensational, or unlike native market writing

Do not force this skill onto:
- personal essays
- general AI/software articles
- interviews unrelated to markets
- legal, audited, or contractually literal translations

For mixed batches, edit only the financial pieces unless the user explicitly requests broader editing.

## Language Reference

For Chinese market jargon, trading idioms, options terminology, macro language, technical analysis, valuation language, positioning, flows, and tone mapping, consult `references/market-language.md`.

Do not treat the reference as a one-to-one dictionary. Pick the expression that matches the market meaning. If no natural equivalent exists, rewrite the sentence.

## Workflow

### 1. Extract the market meaning first

Identify:
- **Thesis:** What is the author actually arguing?
- **Evidence:** What price action, earnings data, macro data, valuation points, positioning data, or flow evidence supports it?
- **Catalysts:** What could move the asset next?
- **Risks:** What could invalidate or weaken the thesis?
- **Levels:** Preserve all prices, ranges, percentages, dates, yields, probabilities, and technical levels exactly unless the task explicitly includes fact-checking.
- **Positioning:** Is the author suggesting buy, trim, hold, hedge, wait, reload, avoid chasing, or watch for confirmation?

Do not start from Chinese syntax. Reconstruct each paragraph from these ideas.

### 2. Rewrite for a North American financial audience

Prefer concise, market-native verbs:
- rise, gain, advance, rally, rebound
- fall, slide, drop, sell off, pull back
- break above, clear resistance, reclaim, hold support
- fade, stall, consolidate, coil, digest gains
- price in, reprice, compress multiples, expand margins
- trim, add, build a position, reload, hedge, stay sidelined

Prefer standard market framing over translated metaphors.

### 3. Preserve conviction accurately

Do not strengthen or weaken the author's view.

Examples:
- “可能” → may / could / appears to / likely, depending on context
- “大概率” → likely / more likely than not
- “确认” → confirmation only when the source really claims confirmation
- “看多” → bullish / constructive / positive on
- “不赌突破” → wait for confirmation / do not front-run the breakout

Never turn a tentative statement into a fact.

### 4. Remove literal metaphors and translated market logic

Common failures:

| Avoid | Prefer |
|---|---|
| pull back to pick up passengers | pullback offers a better entry |
| master switch | key signal / key catalyst / gating level |
| safety line | key support / confirmation level |
| risk line | key downside level / support threshold |
| whole AI chain | AI supply chain / AI complex / AI trade |
| money rotates direction | capital rotates between groups |
| capital front-running expectation | investors are pricing in future growth / flows are moving ahead of fundamentals |
| profit tape is thick | positioning is crowded / many holders are sitting on gains |
| cash landing is cash landing | signed contracts do not guarantee near-term revenue recognition |
| the market starts marking to market | investors are testing valuations against earnings / the trade is entering an earnings-test phase |
| slow-bull tape | steady grind higher / low-volatility uptrend |
| right-side confirmation | confirmation / wait for the breakout to confirm |
| mainline exposure | core exposure / exposure to market leaders |
| high-level positioning | crowded positioning near the highs |
| stock has imagination | the long-term upside case remains compelling / the narrative supports a higher valuation |

When the source uses vivid Chinese imagery, translate the function, not the picture.

## Titles and Metadata

Treat titles and descriptions as separate editing tasks. Do not assume a natural body means the metadata is acceptable.

### Titles

Rewrite for clarity, specificity, and native financial tone.

Avoid:
- literal Chinese metaphors
- long noun chains
- unexplained dramatic language
- date suffixes such as `20260714` when the publication system already stores the date
- clickbait that overstates the thesis
- headlines that claim causality stronger than the body supports

Prefer structures such as:
- `X as Y`
- `X, but Y`
- `X Tests Y`
- `X Raises a New Risk for Y`
- `X Remains the Key Catalyst`

Examples:
- `Semis Broke First, But the Index Has Not Fully Caved Yet` → `Semiconductors Break Support While the Broader Market Holds`
- `Google Is the Real Switch` → `Google Remains the Key Catalyst`
- `The AI Spending Model Is Changing — and a Crack in the Semiconductor Faith` → `AI Spending Shifts from Expansion to Capital Discipline`

### Descriptions

Check every description for:
- truncation mid-word or mid-sentence
- duplicated title language
- excessive hype
- unexplained jargon
- missing thesis

A good description should summarize the central market setup in one or two complete sentences.

## Batch-Editing Rules

When editing many articles:

1. Classify by topic before editing. Do not apply financial style rules to non-financial posts.
2. Preserve file structure, front matter, slugs, image paths, imports, HTML wrappers, and publishing markup unless the user asks to change them.
3. Edit prose, headings, titles, and descriptions without silently altering market data.
4. Search the full batch for recurring translation artifacts after the first pass.
5. Re-check titles and descriptions separately from body copy.
6. Do not rewrite already-natural prose merely to create a diff.
7. Keep tone consistent across the archive without flattening every author's voice into identical phrasing.

Useful batch-search red flags:
- `master switch`
- `right-side`
- `safety line`
- `risk line`
- `mainline`
- `rhythm` when it means market regime or pace
- `imagination` when it means valuation upside
- `feast` / `leftovers` / `pick up passengers`
- `money rotates direction`
- `capital front-running expectation`
- date strings appended to headlines
- descriptions ending mid-word

## Style Guide

### Voice

Aim for the middle ground between:
- Bloomberg-style market commentary
- sell-side research notes
- a sharp independent investor newsletter

The writing should sound informed and direct, not academic and not promotional.

### Sentence style

- Prefer short to medium sentences.
- One main market idea per sentence.
- Put the ticker or asset near the front when it is the subject.
- Use active voice where natural.
- Avoid excessive em dashes, rhetorical flourishes, and repetitive transitions.
- Avoid generic AI phrases such as “it is worth noting,” “this suggests that,” or “in the current market environment” unless useful.
- Avoid noun piles such as “tech AI debt line semiconductor divergence.” Break them into a clear causal headline.

### Tickers and numbers

- Keep ticker symbols uppercase: NVDA, GOOG, SPX, NDX, IGV.
- Preserve exact price levels and ranges.
- Use standard English financial formatting: $100, 3.6%, 10Y Treasury yield, Q2, EPS, CapEx.
- Do not silently change unusual figures. Flag suspected errors separately if fact-checking is in scope.

### Facts versus editing

Editing is not fact-checking by default.

Do not silently update:
- historical prices
- company guidance
- macro data
- dates
- market probabilities
- attribution

If a claim looks wrong but the user asked only for language editing, preserve it and flag it separately rather than rewriting history.

## Asset-Specific Language

### Stocks and ETFs

Prefer:
- upside/downside
- support/resistance
- breakout/breakdown
- relative strength/weakness
- multiple expansion/compression
- earnings revisions
- guidance
- positioning
- risk/reward
- catalyst
- valuation

### Options

Use standard derivatives terminology:
- sell/write a put or call
- short put / short call
- covered call
- cash-secured put
- credit spread / debit spread
- assignment / exercise
- expiration / DTE
- implied volatility / IV
- delta / gamma / theta / vega
- premium collected / premium paid
- roll out / roll up / roll down
- close for a profit / take profit

Never translate “接仓” as “receive shares”; use “take assignment” or “be assigned shares.”

### Macro

Prefer:
- rate-cut expectations / hike expectations
- policy path
- inflation print
- labor-market cooling
- long-end yields
- financial conditions
- risk appetite
- growth expectations
- earnings sensitivity
- valuation sensitivity

### Technical analysis

Prefer:
- reclaim
- clear
- hold
- lose support
- break above / below
- consolidate
- test / retest
- gap
- supply zone / demand zone
- momentum
- volume confirmation

Avoid overclaiming precision. Technical levels are signals, not certainties.

## Two-Pass Editing

### Pass 1 — Fidelity

Check that the English preserves:
- thesis
- chronology
- causality
- caveats
- numbers
- tickers
- technical levels
- catalysts
- risks
- trade posture

### Pass 2 — Native-market rewrite

Ignore the source sentence structure and ask:

> Would an experienced English-speaking investor or market writer naturally phrase it this way?

If not, rewrite it.

For batch work, add a third pass:

### Pass 3 — Archive consistency

Check:
- headline tone across articles
- metadata completeness
- repeated Chinglish patterns
- truncated descriptions
- inconsistent terminology for the same market concept

## Quality Gate

Before finalizing, verify:

- No literal Chinese metaphors remain unless intentionally explained.
- No ticker, number, price level, date, or percentage was lost.
- No speculative statement became a fact.
- No causal relationship was invented.
- Titles sound natural and are not overloaded noun chains.
- Descriptions are complete sentences and not truncated.
- Verbs match actual market behavior.
- Options terminology is standard.
- Technical-analysis wording is conventional.
- Non-financial pieces were not accidentally rewritten with financial jargon.
- Publishing structure and metadata fields remain intact.
- The article can be read without knowing Chinese.
- The prose does not sound like a translation.

## Output Modes

When the user does not specify a format, return only the polished English version.

Supported modes:
- **faithful** — maximum fidelity, light stylistic editing
- **native** — default; preserve meaning while fully rewriting for natural financial English
- **newsletter** — sharper pacing and stronger headings
- **research-note** — neutral, institutional tone
- **social** — concise X/Twitter-style financial English

## Example

Chinese source:

> GOOG今天大跌但没有明显利空，技术结构也没坏，更像倒车接人。软件这边IGV 107还是总开关，没突破之前不要赌突破。

Literal translation to avoid:

> GOOG fell sharply today without obvious bad news. The technical structure is not broken and it looks more like reversing to pick up passengers. IGV 107 is still the master switch for software. Do not bet on the breakout before it breaks through.

Preferred rewrite:

> GOOG sold off sharply despite no clear company-specific negative, while the broader technical structure remains intact. For now, the pullback looks more like a better entry than a trend break. In software, IGV still needs a clean move above 107 before the group turns decisively constructive, so it makes sense to wait for confirmation rather than front-run the breakout.
