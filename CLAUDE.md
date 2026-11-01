# CLAUDE.md — working in this repo

This repo is the single source of truth for Marco's Liquidity Inducement
2.0 (Da Vinci Model). When working here or using this skill:

1. Read `SKILL.md` first, and `references/marco_trading_style_final.md`
   for the verbatim playbook. If anything elsewhere conflicts with
   Section 0 of the playbook, Section 0 wins.
2. Key corrected rules (do not revert to v1 behaviour):
   - No blind limit at the block edge: entry goes on the sweep of the
     induced level in front of / inside the Liquidity Block; the block
     is the stop-loss shield.
   - Blocks are fractal: 4H/1H/30m/15m for direct entries, 5m/1m for
     confirmation when direct RR < 3.
   - Partials: 0% + breakeven, or max 20%-25%, at the first internal
     pool; 75%-80% runs to the final HTF pool.
   - Asia set-and-forget limits are allowed if a clean LB + inducement
     is already formed before London.
3. Before presenting any setup, run the 8-point master checklist
   (playbook Section 7). Any NO = no trade; say that plainly.
4. Never place orders, and never present this as financial advice.
   Setups are for manual execution by the user on MT5; prices come from
   the TradingView OANDA feed. Pairs: XAUUSD, EUR/USD, GBP/USD, USD/JPY,
   USD/CAD, GBP/JPY.
5. Keep edits faithful to the 17-video source table (playbook Section 8);
   do not add rules that are not in the playbook without marking them
   clearly as additions.
