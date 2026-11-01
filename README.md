# Liquidity Inducement 2.0

Marco's liquidity-inducement trading playbook — the **Da Vinci Model**
edition, rebuilt from all **17 Marco videos** (the 16 core playlist videos
plus the 1h 10m Chart Fanatics *Da Vinci Model* interview), updated
**1 November 2026**.

This is an independent synthesis of publicly shared trading concepts. It is
not an official Marco product, and it is not financial advice. It never
places an order; any trade is placed manually by the user on their own
broker (MT5), with prices read from the TradingView OANDA feed.

> This repo **replaces** the older `liquidity-inducement-trading` (v1,
> 16 videos) and `The-Da-Vinci-Trading` repos, which have been deleted.
> Section 0 of the playbook lists what changed and why.

## What is inside

- `SKILL.md` — the complete, Claude-ready skill: frontmatter + the full
  playbook. This is the file to load when you want an AI to work in
  Marco's style.
- `references/marco_trading_style_final.md` — the playbook exactly as
  delivered (verbatim source document).
- `CLAUDE.md` — working instructions for Claude / Claude Code in this repo.
- `skill.yaml` — skill metadata (name, title, description).

## The model in one paragraph

Every trade needs 3 pillars: **True Liquidity** (a level price respected
repeatedly, so stops sit beyond it), **Engineered Liquidity** (a respected
level just short of the HTF target that traps traders and confirms the
draw), and a **Liquidity Block** (a zone that already swept liquidity to
its left, so it holds no liquidity anymore — it is the stop-loss shield,
not a blind entry). Frame direction and targets on Daily/4H (PDH/PDL,
breadcrumbs, untaken pools), stay out of No Man's Land, wait for early
buyers/sellers to be **induced** in front of or inside the block, and place
the entry **on the sweep of that induced level**, with the stop beyond the
whole block. Direct entries use 4H/1H/30m/15m blocks when RR to the final
HTF pool is at least 1:3; if direct RR is under 3, drop to 5m/1m and wait
for a fresh mini Da Vinci confirmation block. At the first internal pool,
take 0% partial and move to breakeven, or take at most 20%-25% — and let
the remaining 75%-80% run to the final HTF target.

## Pairs in scope

`XAUUSD`, `EUR/USD`, `GBP/USD`, `USD/JPY`, `USD/CAD`, `GBP/JPY`
(TradingView OANDA feed → manual execution on MT5).

## Use it with Claude

- **Claude (chat / projects):** add this repo or upload `SKILL.md` to your
  project, then ask for a Marco-style / Da Vinci setup check. Claude
  should work through the 8-point checklist in Section 7 of the playbook
  and refuse the trade if any point fails.
- **Claude Code:** clone this repo into `~/.claude/skills/liquidity-inducement-2.0/`
  (user scope) or `<project>/.claude/skills/liquidity-inducement-2.0/`
  (project scope), then restart Claude Code or run `/skills` to verify it
  appears.
- **Muse:** copy this folder to
  `~/workspace/custom-skills/liquidity-inducement-2.0/` and the skill
  becomes available through skill search.
