---
name: liquidity-inducement-2.0
description: >-
  Marco's Liquidity Inducement 2.0 (Da Vinci Model): find trades from True
  Liquidity, Engineered Liquidity and a Liquidity Block. Entry is placed on
  the sweep of the induced level in front of / inside the block (never a
  blind block tap), stop loss beyond the whole Liquidity Block, minimum
  1:3 RR to the final HTF pool, 0%-25% partial at the first internal pool
  then breakeven. Fractal: 4H/1H/30m/15m blocks for direct entries,
  5m/1m mini Da Vinci for confirmation when direct RR is under 3. Use
  when the user asks for a Marco-style setup, a liquidity block / Da Vinci
  check, or a live scan on XAUUSD, EUR/USD, GBP/USD, USD/JPY, USD/CAD,
  GBP/JPY.
---

# Liquidity Inducement 2.0 — How to use this skill

You are applying Marco's liquidity-inducement method exactly as written in
the playbook below. Rules:

- Follow the playbook, in its order. Section 0 corrections override any
  older version of this method (including any "Liquidity Inducement
  Trading" v1 skill): no blind block-tap entries, blocks are fractal
  (not 1H-only), partials are 0%-25% (not 40%-50%), and Asia set-and-forget
  limit orders are allowed when a clean LB + inducement is already formed.
- Before any trade idea, work through the 8-point master checklist in
  Section 7. If any answer is not YES, there is no trade — say so plainly.
- Never place an order. You only find, check and explain setups; the user
  executes manually on MT5 (prices are read from the TradingView OANDA feed).
- Pairs in scope: XAUUSD, EUR/USD, GBP/USD, USD/JPY, USD/CAD, GBP/JPY.

---

# Marco Trading Style — Final Authentic Playbook (Da Vinci & Liquidity Block Edition)

**Updated:** November 1, 2026 (Dhaka Time - GMT+6)  
**Basis:** Complete audio transcript + visual chart breakdown of all **17 Marco videos** (including the 1h 10m Chart Fanatics *"Da Vinci Model"* interview `T_djSNBmV00` + all 16 core playlist videos).  
**Pairs Monitored (OANDA Feed on TradingView -> Manual Execution on MT5):** `XAUUSD`, `EUR/USD`, `GBP/USD`, `USD/JPY`, `USD/CAD`, `GBP/JPY`

---

## 0. Major Corrections from Previous AI Version (What Changed & Why)

1. **Removed "Blind Block Tap Entry":** Marco does **not** place a blind limit order at the edge of a Liquidity Block (LB) alone. **Actual Rule:** An Induced Level (early buyers/sellers) must form right in front of or inside the LB. The entry is placed **on the exact line where the induced liquidity is swept**, while the Stop Loss (SL) goes behind the LB.
2. **Removed "1H-Only Block" Restriction:** Marco's system is **100% fractal**. Blocks and Da Vinci setups form on `4H / 1H / 30m / 15m` for direct entries, and on `5m / 1m` for confirmation entries when the HTF Stop Loss is too large (when direct $RR < 3.0$).
3. **Updated Partial Taking Rule (From 50% to 0%–25%):** Taking 40–50% off early ruins the payout on the main HTF target. **Actual Rule:** At the first internal liquidity level, either move **SL to Breakeven (BE) with 0% partial**, or take a maximum of **20%–25% partial**, leaving **75%–80% volume** to run to the final HTF pool.
4. **Updated Session Rule (Asia Limit Orders Allowed):** Marco lives in Toronto (EST). Before sleeping at 10:00–11:00 PM EST (**8:00–9:00 AM Dhaka Time**), if a clean LB + Inducement is already formed in Asia, he sets a Limit Order (Set & Forget) to be triggered during London.

---

## 1. Core Philosophy & The 3 Pillars

> *"If you don't see liquidity, you ARE the liquidity. React, don't predict."*

Every valid Marco trade requires **3 mandatory pillars** working together:

### Pillar 1: True Liquidity ($\$\$\$$ Target / Trap Zone)
* Not every swing high or swing low is liquidity.
* A level is **True Liquidity** only when price creates a high/low, comes back to **respect it** (forming equal/relative highs or lows, or tapping and rejecting multiple times), and moves away. This proves retail traders entered there and placed their Stop Losses just beyond that level.

### Pillar 2: Engineered Liquidity (EL — The "Da Vinci" Activator)
* Suppose HTF bias is **Bullish** (targeting an untaken HTF high above).
* Price rallies upward toward that HTF high, stops just short of it, **respects a level below the target** (creating equal/relative highs), and drops down.
* That respected high is **Engineered Liquidity (EL)**. It confirms that sellers are now trapped above and price is only dropping down to grab fuel (liquidity) before running through both the EL and the HTF target.
* **Hard Rule:** *No Engineered Liquidity = No Da Vinci Model.*

### Pillar 3: Liquidity Block (LB — The Stop Loss Shield)
* **How an LB is Born:** When price **sweeps/stabs** a previous swing high or low on the left-hand side and reverses sharply, that sweeping zone/candle becomes a **Liquidity Block (LB)**.
* **Why It Works:** Because that high/low already swept the liquidity to its left, *"it holds NO liquidity anymore."* Price has no reason to go beyond that extreme again.
* **Role in Execution:** The LB is **not** a standalone entry trigger; it is your **Stop Loss reference**. *No LB = No Stop Loss placement = No Trade.*

---

## 2. Step-by-Step Workflow (Exact Order of Operations)

### Step 1: Daily & 4H Framing (Direction & Targets)
1. **Mark PDH & PDL:** Start on the Daily chart. Mark **Previous Daily High (PDH)** and **Previous Daily Low (PDL)** for framing.
2. **Daily Sweep Play:** If yesterday swept the prior day's high and closed bearish while leaving the prior day's low untouched, today's primary draw on liquidity is that untouched Daily low (and vice versa).
3. **Inside Day Filter (Stay Cautious):** If yesterday was a massive expansion candle that swept **both** the previous day's high and low, expect today to be an **Inside Day** (choppy consolidation between PDH and PDL). Reduce risk or avoid trading mid-range.
4. **Map "Breadcrumbs":** On `4H` and `1H`, mark sequences where price moved in one direction leaving *lows respecting lows* (or *highs respecting highs*). These untouched stairs ("breadcrumbs") are your staged Take Profit targets.
5. **Chart Squeeze Rule:** If candles on `4H` or `1H` look squeezed/compressed sideways and swings are unclear, drop down one timeframe (`30m` or `15m`) to open up the price action.

### Step 2: Range & "No Man's Land" Check
* Identify the external Range High (untaken pool above) and Range Low (untaken pool below).
* **No Man's Land:** The middle zone between upside liquidity and downside liquidity.
* **Hard Rule:** Never trade in the middle of the range. Wait (even if it takes days) until price reaches and sweeps one of the extremes.

### Step 3: Spot the Setup Sequence (The Da Vinci Checklist)
*(Bearish Sell Example — Reverse for Bullish Buy)*
1. **Left-Side LB:** Locate a fresh, unmitigated **Liquidity Block (LB)** above/left (a high that previously swept an older high).
2. **Opposite Untaken Target ($\$\$\$$):** Confirm there is **Engineered Liquidity** or an untaken liquidity pool below (equal lows / PDH-PDL / breadcrumbs). Every LB **must** be paired with an opposite target.
3. **Inducement (Early Sellers):** As price approaches just below the LB, it breaks a minor internal low (Retail BOS) and drops slightly. Retail traders sell the breakdown (**Sellers Induced**), placing their stops above the inducement high.
4. **Nearer-Trap Check (Look Left):** Always check if an internal level closer to current price has already swept and trapped traders inside a nearer LB. Do not blindly wait for a distant extreme if a valid nearer trap has already triggered.

---

## 3. Exact Entry Models (4 Ways Marco Executes)

### Model 1: Direct Sweep Limit Entry (The Da Vinci Standard)
* **When to Use:** You have a fresh LB on the left, an induced high/low right in front of/inside the LB, and placing your entry at the induced level with SL beyond the LB gives **$RR \ge 3.0$** to the final target.
* **Entry Level:** Place your **Limit Order directly on the Induced High/Low line** (the exact price where induced sellers/buyers get swept). Do **not** get greedy waiting for the extreme top/bottom of the LB or a 1m FVG/imbalance, or you will miss the move.
* **Stop Loss:** Just beyond the extreme high/low of the left-hand **Liquidity Block (LB)** + Spread Buffer.

### Model 2: LTF Confirmation Entry ($5m$ / $1m$ Mini Da Vinci)
* **When to Use:**
  1. Direct entry on `1H/15m` gives **$RR < 3.0$** because the HTF LB is too wide.
  2. Or you missed the direct tap, or price hit the LB with heavy momentum.
* **Execution Steps:**
  1. Wait for price to tap the `1H/15m` LB and sweep the induced level.
  2. Drop to the **$5m$ or $1m$ chart**.
  3. Wait for a **new LTF inducement + LTF sweep** to form a **fresh LTF Liquidity Block** inside the HTF zone.
  4. **Entry:** On the sweep of the LTF induced level (or tap of the new LTF block).
  5. **Stop Loss:** Just beyond the new LTF LB extreme (turning a $1:2$ trade into a $1:8$ to $1:13$ RR setup).

### Model 3: The 30-Minute Candle Sweep Entry (9:30 AM NY Open & Daily Levels)
* **When to Use:** When price taps PDH/PDL or a major Daily/4H LB, especially around the **9:30 AM EST NY Stock Open** (8:30 PM Dhaka Winter / 7:30 PM Dhaka Summer).
* **Execution Steps:**
  1. Switch to the **$30m$ chart**.
  2. Let the 30m candle (e.g., the 9:00–9:30 AM EST candle) close inside/at the LB.
  3. When the **next 30m candle** (e.g., 9:30 AM EST) opens and **spikes/sweeps the high (for sell) or low (for buy) of the previous 30m candle**, execute the trade on that sweep.
  4. **Stop Loss:** Beyond the LB extreme.

### Model 4: "To-The-Minute" $5m$ Candle Closure (Time Confluence Exception)
* **When to Use:** Only when a sweep aligns **to the exact minute** with a major `1H` or `4H` candle open (e.g., the `:55` $5m$ candle creates the inducement high/low, and the `:00` new hour candle sweeps it and closes as a $5m$ engulfing candle).

### Bonus: Stacking Entries (Adding a 2nd Position)
* **Condition:** Trade 1 is in profit, and the **Final HTF Target is still untouched**.
* **Trigger:** Price pulls back toward an intermediate LB created by the first move, builds fresh equal highs/lows (inducement), and sweeps them into that new LB.
* **Execution:** Enter Position 2 on the sweep, place SL beyond the new LB, and aim for the **same Final HTF Target**.

---

## 4. Stop Loss, Take Profit & Trade Management Rules

### Stop Loss (SL) Rules (*"Will Never Change"*)
* **Placement:** Always outside the entire Liquidity Block (LB) extreme. Never place SL inside the middle of a block or tight on a random wick tip.
* **Spread & Feed Buffer (OANDA to MT5):**
  * **Forex Majors (`EUR/USD`, `GBP/USD`, `USD/JPY`, `USD/CAD`):** LB extreme + **2 to 3 pips**.
  * **Gold (`XAUUSD`) & `GBP/JPY`:** LB extreme + **50 pips ($5.00 on Gold)** / **5–8 pips on GJ** for breathing room.
* **No Panic Moving:** Never shrink your SL or move to BE prematurely just because price squeezes back into the LB after entry. Price frequently spikes the first entry high/low inside the LB a second time before dropping.

### Breakeven (BE) & Trailing Rules
* **Exact Breakeven Trigger:** Move SL to Breakeven **only after price breaks/runs the first meaningful internal structure high (for buys) or low (for sells)** in your intended direction.
* **Rapid Gain Protection:** If an explosive move (e.g., Gold 500+ pip drop in 5 minutes) creates massive open profit before hitting the final target, roll the SL just above/below the most recent intervening reaction swing so you never give back a huge winner.

### Take Profit (TP) & Partials
* **Minimum RR Filter:** Every setup must offer at least **$1:3$ RR ($3.0R$)** to the final untaken liquidity pool. Never settle for $2.2R$ as a final target.
* **Partial Strategy:**
  * **At Internal Target 1 (First Untaken Pool):** Either take **0% partial and move SL to BE**, or take **20%–25% partial** + move SL to BE.
  * **At Final HTF Target (External Pool / PDH / PDL):** Let the remaining **75%–80% volume** run to the final target for maximum payout.

---

## 5. Hard Stay-Out Filters (When NOT to Trade)

1. **The "No-More" Rule (Video 4):**
   * Once early buyers are induced and the low is swept (**Buyers Trapped**) $\rightarrow$ **NO MORE SELLS.**
   * Once early sellers are induced and the high is swept (**Sellers Trapped**) $\rightarrow$ **NO MORE BUYS.**
   * Trade *from* the trap toward the opposite untaken liquidity, never into an already-swept side.
2. **Target Already Taken:** If price runs your opposite TP target *before* tapping your entry zone, delete the limit order immediately. The setup is dead.
3. **4H Un-swept Wick Veto (Video 9):** If you want to buy on `15m/5m`, but the `4H` candle respected a prior `4H` low without sweeping it, veto the buy—`4H` still has unfinished business (liquidity) below.
4. **Correlation Filter:** `EUR/USD`, `GBP/USD`, and `XAUUSD` are heavily correlated against USD. If two correlated pairs trigger simultaneously, either pick the cleanest setup or split risk ($0.5\%$ each) instead of doubling exposure.
5. **High-Impact News & Bank Holidays:** No trading on US/UK Bank Holidays. Cancel un-triggered direct limit orders 15–30 minutes before Red-Folder News (CPI, FOMC, NFP) and wait for post-news LTF Confirmation (Model 2).

---

## 6. Dhaka Time (GMT+6) Daily Execution Schedule

*(Synced with Marco's Toronto EST/EDT schedule)*

| Dhaka Time (GMT+6) | Marco's Time (EST) | Session Phase | Action Plan |
| :--- | :--- | :--- | :--- |
| **08:00 AM – 09:30 AM** | 10:00 PM – 11:30 PM | Asia Open / Pre-Bed | Frame Daily (PDH/PDL), 4H, 1H. If a clean LB + Inducement is ready, set Limit Order (Model 1) for London, or watch the `09:00 AM` 4H candle open. |
| **01:00 PM – 05:30 PM** | 03:00 AM – 07:30 AM | London Session | **Buildup & Trap Context.** Pre-set HTF limits may trigger, or London creates the inducement (Equal Highs/Lows) to be swept in NY. Avoid mid-session chop. |
| **06:00 PM – 08:00 PM** *(Summer)*<br>**07:00 PM – 09:00 PM** *(Winter)* | 08:00 AM – 10:00 AM | **NY Open (Heart)** | **Primary Execution Window.** Look for NY to sweep the London inducement into an LB (`Model 1` Direct or `Model 2` 5m/1m Confirmation). |
| **07:30 PM** *(Summer)*<br>**08:30 PM** *(Winter)* | **09:30 AM EST** | **NY Stock Open** | **Gold (`XAUUSD`) Prime Window.** Watch the `30m` candle sweep (`Model 3`) and post-open trap continuations. |
| **10:30 PM – 11:00 PM** | 12:30 PM – 01:00 PM | NY Close / Cutoff | Stop scanning for new entries. Manage open runners or cancel invalid intraday limits. |

---

## 7. Pre-Trade 8-Point Master Checklist

Before placing any trade on MT5, all **8 answers must be YES**:

- [ ] **1. HTF Bias & Paired Target:** Is there a clear Daily/4H draw on liquidity and an untaken opposite pool ($\$\$\$$ / Engineered Liquidity / PDH-PDL)?
- [ ] **2. Out of No Man's Land:** Is price at an extreme (not chopping in the middle of a range)?
- [ ] **3. "No-More" Rule Clear:** Has the target side NOT been swept yet, and has the opposite side NOT already trapped me against the move?
- [ ] **4. Valid Liquidity Block (LB):** Is there a fresh, unmitigated LB on the left that swept prior liquidity (giving me a valid SL anchor)?
- [ ] **5. Inducement + Trap:** Have early buyers/sellers been induced right in front of/inside the LB, and am I entering on the **sweep of their level** (checking for any nearer internal trap first)?
- [ ] **6. $RR \ge 3.0$:** Does direct entry give at least $1:3$ RR to the final target? *(If NO $\rightarrow$ Drop to $5m/1m$ and wait for Model 2 Confirmation LB).*
- [ ] **7. Exact Levels Set:** Are Entry (induced sweep line), SL (beyond LB + spread buffer), BE Trigger (first internal structure break), and Final TP marked on the chart *before* entering?
- [ ] **8. Timing & News Clear:** Is today NOT a Bank Holiday, and is the entry aligned with London/NY timing without imminent Red-Folder news?

---

## 8. Complete 17-Video Source Reference Table

| # | Video Title & ID | Key Rules Extracted into This Playbook |
| :- | :--- | :--- |
| **0** | **Chart Fanatics Interview: The Da Vinci Model** (`T_djSNBmV00`) | Complete Da Vinci sequence: Left LB sweep $\rightarrow$ Engineered Liquidity (respecting opposite POI) $\rightarrow$ Inducement BOS $\rightarrow$ Sweep entry on the induced line, SL behind LB. Take 0%–25% partial at first structure break + BE. |
| **1** | **Liquidity Mastery Vol 1** (`SkKjZeY6EN4`) | "Breadcrumbs" concept (lows respecting lows as future TP targets), wide translucent LB shading, 3 full trade breakdowns. |
| **2** | **Liquidity Inducement Entries: LIQUIDITY BLOCKS** (`GIYrW7FC06M`) | LB = zone that swept left-side liquidity (holds no more liquidity). Reaction-only blocks rejected if no inducement/trap precedes them. |
| **3** | **The Simplest Liquidity Inducement Breakdown** (`2RLRe02LyM4`) | Top-down cascade (`Daily` $\rightarrow$ `4H` $\rightarrow$ `1H` $\rightarrow$ `15m`). Carrying HTF levels down and setting staged TPs (internal = BE/partial, external = final). |
| **4** | **Trade Liquidity Properly** (`LWEuNvtjQNA`) | The sharp **"No-More" Rule**: Once low is swept (buyers trapped), no more sells; once high is swept (sellers trapped), no more buys. |
| **5** | **Fix This Liquidity Mistake** (`E2n7KMQDYIU`) | **Nearer-Trap Rule:** Look left—don't wait for a distant extreme if an internal level already induced and trapped traders closer to price. |
| **6** | **The EASIEST Way To Trade Liquidity** (`HfnKU1D_woM`) | Mandatory Pairing (LB + Opposite Target). Never move SL to BE prematurely on minor pullbacks inside the LB; keep 75–80% volume for final target. |
| **7** | **Liquidity Mastery Vol 2** (`xaF0OBgzPYs`) | Weekly/Daily sweep framing, waiting out Asia/London range buildup, carrying blocks across timeframes. |
| **8** | **Liquidity Mastery Vol 3** (`9gUKOkgODK4`) | **9:30 AM NY Open 30m Candle Trick:** Wait for the 9:30 AM `30m` candle to sweep the 9:00 AM `30m` candle high/low inside an LB. Minimum $1:3$ RR rule. |
| **9** | **How To Spot The CORRECT Liquidity** (`lWTb3oiugDo`) | Not every swing is liquidity—price must respect it first. **4H Veto Rule:** If `4H` respects a low without sweeping it, veto LTF buys. |
| **10** | **You Don't Know Liquidity** (`x-7H1E4ToC8`) | Day-by-day Gold masterclass. Holiday stay-out rule. **"To-The-Minute" 5m engulfing rule** (e.g., `8:55` sweep into `9:00` new hour candle close). |
| **11** | **SIMPLE Liquidity HACK** (`4pINx9wV18U`) | PDH/PDL pairing. Pre-bedtime EST (`8:00–9:00 AM` Dhaka) Set & Forget limit orders for London. **Gold 50-pip ($5.00) SL buffer rule.** |
| **12** | **This is WHY You CAN'T Trade** (`5VvFss8cKPY`) | Psychology & Discipline: Never delete missed levels, never chase, react don't predict. If target is hit before entry, setup is dead. |
| **13** | **Liquidity Inducement Masterclass Ep. 3** (`x4ZUCA0GO48`) | London buildup $\rightarrow$ 9:30 AM NY open trigger. Repeated equal highs = fuel building above. Post-partial pullbacks are normal. |
| **14** | **STACKING Entries** (`fTAVvXYvhi4`) | How to stack a 2nd position on a pullback ONLY when a new LB + new inducement sweep forms while the final HTF target remains untaken. |
| **15** | **The Liquidity Logic You NEED To Know** (`HEBP5I3z__c`) | **Inside Day Rule** (after a massive double-sweep Daily candle). **30m Candle Sweep Entry** at PDL/Daily LB for a $1:9$ RR reversal. |
| **16** | **ADVANCED Liquidity Concepts ON GOLD** (`pQ4WTVQnwBc`) | "No Man's Land" range filter. SL above/below LB *"will never change."* Rolling stop behind reaction swings after massive rapid gains. |