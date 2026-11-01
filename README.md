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
- `AI_INSTRUCTIONS.md` — the universal, vendor-neutral operating
  procedure (workflow, hard rules, exact output format) for any AI.
- `SYSTEM_PROMPT.md` — a ready-to-paste system prompt for any AI chat.
- `AGENTS.md` / `GEMINI.md` / `.github/copilot-instructions.md` —
  auto-read entry points for agent tools, all pointing to
  `AI_INSTRUCTIONS.md`.

## Use it with ANY AI (same result everywhere)

This repo is **not Claude-only**. The rules, workflow and answer format
are written in plain, vendor-neutral files so any AI produces the same
result:

| You are using | Give the AI this |
| :--- | :--- |
| Any chat AI (ChatGPT, Gemini, Grok, DeepSeek, ...) | Paste `SYSTEM_PROMPT.md` into its instructions, and upload/paste `references/marco_trading_style_final.md` |
| Any AI that can read this repo / a URL | Tell it: "Read `AI_INSTRUCTIONS.md` first and follow it exactly" |
| Claude (chat, Projects, Claude Code) | `SKILL.md`, or clone into `~/.claude/skills/liquidity-inducement-2.0/` |
| Codex / generic agents | `AGENTS.md` (auto-read by agent tools) |
| Gemini CLI | `GEMINI.md` |
| GitHub Copilot | `.github/copilot-instructions.md` (auto-read in this repo) |

Why the results match: `AI_INSTRUCTIONS.md` fixes (1) one read order,
(2) word-for-word definitions, (3) one workflow order, (4) hard numeric
rules (RR >= 3.0, buffers, 0%-25% partials), (5) an 8-point checklist
that must pass 8/8, and (6) one exact output format — plus a tie-break
rule: when two readings are possible, the answer is NO TRADE.

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
