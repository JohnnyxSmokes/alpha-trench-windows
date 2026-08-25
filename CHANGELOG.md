# Alpha Trench — Changelog

Collapsible history (all drops + era map): **[BUILD_HISTORY.md](BUILD_HISTORY.md)** · where we are going: **[ROADMAP.md](ROADMAP.md)**

## 0.9.284 — 2026-08-25

### Paper Wallets — Single-Line Balance Toggle
- **Select All With Balance** / **Unselect All With Balance** stay on one line in the header (no wrap padding).

## 0.9.283 — 2026-08-25

### Paper Wallets — Unselect All Restored
- **Unselect All With Balance** again turns off every book with SOL (no active-book exception).

## 0.9.282 — 2026-08-25

### Wallet Bar — Cash vs Equity Clarity
- Paper wallet rows now show **3-decimal** SOL balances to match the header sum.
- Wallet bar tooltip breaks out **Cash** vs **Equity (Incl. Open Positions)** when you have open bags.

## 0.9.281 — 2026-08-25

### Paper Wallets — Balance Select In Header
- **Select All With Balance** (green) / **Unselect All With Balance** (red) now live in the Paper Wallets header beside the tips pill — no full-width row under the wallet list.

## 0.9.280 — 2026-08-25

### Trade History — Inline View Selectors
- **All Trades** / **Closed Trades** pills now live in the Trade History header row beside the close button — larger tap targets, no extra row pushing the list down.

## 0.9.279 — 2026-08-25

### Chart — Average Lines vs Fill Pins
- **Buy / Sell Average Lines** (Buy / Sell tab) now controls **horizontal avg lines only** — no longer pulls in B/S fill pins.
- **Show Chart Marks** (Behavior tab) remains the toggle for B/S bubbles on the chart.

### Wallet Panel — Tighter Stack Layout
- **Quick Buy Rotation** and **Enable Multi Wallet** sit directly under **Unselect All With Balance**; removed the dead flex gap in the stack overlay.

### Settings — Buy / Sell Tab
- Shorter panel body so **Save Fee Settings** sits closer to the toggles above it.

## 0.9.278 — 2026-08-25

### Chart Marks — Current Round Only
- B/S chart pins now match **Average Buy** scope: only fills from wallets with an **open position** on this token, after that round's `openedAt` (no lifetime journal replay).
- Switching tokens on Axiom clears stale native TV marks/lines immediately.

## 0.9.277 — 2026-08-25

### Wallet + Trades — Buy/Sell Stack Overlay
- With **Side Panel Menus** off, Wallet and Trades now drop over the **Buy/Sell** button area (widget height stays fixed).
- Scroll trade history and paper wallets inside the overlay; **×** or clicking the bar chevron closes it and restores Buy/Sell.
- Coin info footer (PnL card) stays pinned below.

## 0.9.276 — 2026-08-25

### Settings Gear — Toggle + Active State
- Settings gear turns **red** while the settings panel is open.
- Clicking the gear again **closes** settings (toggle on/off).

## 0.9.275 — 2026-08-25

### Wallet + Trades — In-Panel Mode
- With **Side Panel Menus** off, **Wallet** and **Trades** expand inside the widget again (drop-in panels below the bar row) instead of doing nothing.

## 0.9.274 — 2026-08-25

### Settings — Behavior
- Removed **Show Currency Switcher** toggle (dead setting). PnL row still toggles SOL ↔ USD when you click **Invested**, **Sold**, **Remaining**, **Fees**, or **PnL**.

## 0.9.273 — 2026-08-25

### Wallet + Trades Bar — Independent Of PnL Row
- **Show PnL Row** off still keeps **Wallet** and **Trades** side-by-side; trades bar no longer disappears.

## 0.9.272 — 2026-08-25

### Settings — Tabs-Only Chrome
- Removed **Instant Trade Settings** title row and **×** close button; tab bar is now the top of the panel (close via settings gear or click-away).

## 0.9.271 — 2026-08-25

### Settings — Buy / Sell Field Centering
- Paired fee labels and input values are centered in each column.

## 0.9.270 — 2026-08-25

### Settings — Buy / Sell Tab Compact Pairs
- Fee inputs paired side-by-side: **Buy/Sell Slippage**, **Buy/Sell Priority**, **Buy/Sell Gas** (3 rows instead of 6).

## 0.9.269 — 2026-08-25

### Price Metric — Position Value Hover
- With an open position on selected wallets, hover **Price** morphs to **Position Value** (current holdings × live price in SOL).
- No hover affordance when there is no open position.

## 0.9.268 — 2026-08-25

### Info Footer — Compact Position Layout
- PnL SOL + % moved to top-right; token row is icon + name + X only.
- Stats row: **Invested** (SOL), **Buys / Sells** (green/red), **Avg Entry**, **Avg Exit** — four boxes, tighter padding.

## 0.9.267 — 2026-08-25

### Paper Wallets — In-Panel Info Callout
- ℹ on **Paper Wallets** now shows tips **centered inside the wallet panel** (not floating above/outside the box).

## 0.9.266 — 2026-08-25

### Settings — Side Panel Label
- Renamed **Side Panel For Wallet & Trades** → **Side Panel Menus** (single-line row on Advanced).

## 0.9.265 — 2026-08-25

### Settings — Remove Apply Brackets Button
- Dropped **Apply Brackets To Position** from Advanced — **Save Advanced** SL/TP already monitors open positions and chart markers.

## 0.9.264 — 2026-08-25

### Settings — Advanced Tab Compact
- **Side Panel For Wallet & Trades** helper text moved to ℹ hover callout (no extra padding row).
- **Stop Loss %** and **Take Profit %** sliders sit side-by-side in one row.

## 0.9.263 — 2026-08-25

### Settings — Perps Leverage Gated On HL
- **Perps Leverage** only shows on the Wallets tab when **Hyperliquid** is the selected Paper Chain.

## 0.9.262 — 2026-08-25

### Settings — Paper Wallet Tips Overlay
- **Paper Wallet Tips** opens a full-panel overview inside the Wallets settings view (no push-down scroll).
- Close via the bar, **×**, another tab, click-away, or closing settings.

## 0.9.261 — 2026-08-25

### Settings — Centered Info Callout
- Info pill (ℹ) on settings rows now shows a **centered callout** inside the Instant Trade settings panel — no edge clip, no horizontal scroll.

## 0.9.260 — 2026-08-25

### Settings — Alpha Tek Features Tooltip
- Renamed **Enable Alpha Tek Paid Features** → **Enable Alpha Tek Features**.
- Info pill tooltip anchors on the ℹ and expands **left** so copy stays inside the settings panel (no horizontal scroll / off-page clip).

## 0.9.259 — 2026-08-25

### Settings — Paper Wallet Tips Echelon
- **Paper Wallet Tips** is now a click-toggle accordion (not hover): tap again to close.
- Tips panel expands inline above the button — full width, no scrollbar, scrolls with the settings sheet.

## 0.9.258 — 2026-08-25

### Trade History — Buy/Sell Color Coding
- **Bought** SOL amounts show in **green**; **Sold** amounts in **red** (All Trades and Closed Trades).
- Closed rows label **Loss** (red) instead of **Profit** when the round lost money.

## 0.9.257 — 2026-08-25

### Settings Layout Cleanup
- Removed helper paragraphs from **Behavior** and **Buy / Sell** tabs.
- **Enable Alpha Tek Paid Features** now has an **ℹ** hover pill instead of inline hint text.
- **Quick Buy On List** moved to **Buy / Sell** tab.
- **Reset PnL Baseline** moved to **Wallets** — sits beside **Reset All Paper Wallets** in a two-button row.
- **Behavior** tab trimmed to sound settings only (no scroll clutter).

## 0.9.256 — 2026-08-25

### Trade History — Chain Badge On Rows
- **Closed Trades** rows now read **Closed Trade 1 / 2 / 3** with the **Solana mark** beside the title (matches All Trades buy/sell rows).

## 0.9.255 — 2026-08-25

### Trade History + Info Footer Polish
- Closed rows label **Trade 1 / Trade 2 / …** instead of **#1**.
- **Replay** button returns beside the wallet tag on **Closed Trades** only (not on All Trades).
- **Info footer** redesigned: larger token icon, **X** button moved into the footer (opens tweet side panel), **SOL In** label, boxed **Buys / Sells / Avg Entry / Avg Exit** grid matching the top stats row.
- Removed the **PAPER** watermark from the position footer.

## 0.9.254 — 2026-08-25

### Settings Scroll + Advanced Dock Toggle
- **Settings sheet scroll** — `.sheet.open .sheet-body` scrolls internally; wheel on tabs/header routes through `sideDockScrollTarget` so the panel captures scroll instead of the page.
- **Wallet & Trades dock mode** moved to **Advanced** as a toggle row (**Side Panel For Wallet & Trades**); removed from Behavior tab segment buttons.

## 0.9.253 — 2026-08-25

### Trades Dock — Two-Line Rows
- Trade rows use a **two-line stack**: trade #, wallet tag, and time on top; Bought / Sold / Profit on the bottom.
- **Replay button removed** — tap the row to open replay (same as before).
- Timestamps shortened to **40m**, **1h**, **4s** (no **Ago** suffix) so text no longer overlaps.

## 0.9.252 — 2026-08-25

### Trades Side Panel — Horizontal Log Layout
- Restored **horizontal row layout** for trade history (reverts the vertical card stack from 0.9.249).
- Rows now span the **full dock width** with replay, stats, and wallet tags on one line.
- Header simplified to **Trade History** only — removed duplicate **Trades** title and **Fees Paid** line.
- **All Trades / Closed Trades** tabs sit on the top row beside the header with tighter padding.

## 0.9.251 — 2026-08-25

### Alpha Tek Promo Pop (AT Logo)
- Side pop **top-aligns with the trade widget** (flush with panel top, not the header button).
- **280px width** to match other side docks.
- Centered **AlphaTek mark** logo, refreshed copy (no em dash), **For Free** on the lead line.
- Link rows with icons: AlphaTek mark, dashboard grid, Discord logo.
- **Visit AlphaTek.app** uses correct capitalization.

## 0.9.250 — 2026-08-25

### Paper Wallets — Info Pill
- Removed the two hint paragraphs from the Paper Wallets dock so wallet rows sit flush at the top.
- Added an **ℹ** info pill beside **Paper Wallets** — hover/focus shows tips above (bubble color, chart bubbles, enabled vs highlight).

## 0.9.249 — 2026-08-25

### Side Panel Polish (Sizing, Scroll, Layout Option)
- **Unified dock size:** Wallet, Trades, and Settings side panels now share **280px width** and **match the main widget height** (same footprint as Settings).
- **Trades history layout:** Trade rows stack vertically inside the Trades dock so labels/stats no longer overlap or horizontal-scroll.
- **Settings scroll fix:** Wheel events over open side docks stay inside the extension (no more scrolling the Axiom page behind Settings).
- **Behavior → Wallet & Trades Panel:** Choose **Side Panel** (default, fixed widget height) or **In Panel** (classic inline expand inside the widget).

## 0.9.248 — 2026-08-25

### Unified Side Panels (One At A Time)
- **Wallet**, **Trades**, **Settings**, **Alpha Tek**, and **Tweet** panels now dock beside the Instant Trade widget instead of stretching it taller.
- **Trades breakdown** pops out as a fixed side panel (same pattern as Paper Wallets) — no more inline list pushing Invested / Buy / Sell down.
- **Settings** opens as a side dock instead of covering the full panel height.
- **Mutex:** only one side panel can be open at a time — opening Wallet closes Trades, Settings, etc.
- Click outside a dock (or on the main panel) dismisses the active side panel.

## 0.9.247 — 2026-08-25

### Thin Instant Trade Layout (Optional Narrow Mode)
- **MIN_W stays 172** — users can still resize the panel very thin; no forced width floor bump.
- At **≤280px** panel width: **Tokens / Price / Market Cap** stack vertically as full-width rows (label left, value right).
- **Wallet** and **Trades** buttons stack vertically at the same breakpoint instead of squeezing side-by-side.
- **Head overflow menu (⋯)** exposes Settings, Paper Wallets, Lock, and Help when inline header icons hide; **Collapse** stays visible.
- Trades label splits into word + detail spans so narrow mode shows `3 · 11M Ago` without crushing the row.

## 0.9.246 — 2026-08-25

### Chart Marks Only (No Layout Changes)
- Removed TradingView **execution-shape** fallback (`createExecutionShape`) that drew square B/S pins off-chart and duplicated circular marks.
- When native `getMarks` is unavailable, fills use **SVG overlay circles** only — no square TV pins.
- **Average buy/sell chart lines opt-in only** — default off after settings migration v2; enable under **Settings → Fees → Buy / Sell Average Chart Marks** if wanted.
- **Instant Trade layout unchanged** from 0.9.244 (no MIN_W clamp, no narrow responsive CSS, no head overflow menu).

## 0.9.239 — 2026-08-24

### Axiom Price-Unit and Token Quantity Fix
- Axiom compact USD notation such as **`$0.0₃2`** is parsed as **$0.0002**, not $0.032 or 0.032 SOL.
- Removed broad body-text `* SOL` scanning that could mistake wallet balances, fees, or order sizes for SOL-per-token.
- Pending tokens only bootstrap from an explicit native-price field or a cross-checked USD/native pair with a plausible SOL/USD rate.
- Before paper execution, USD and native prices are cross-checked against trusted SOL/USD; unverified fills fail closed.
- Legacy open positions with correct Avg Entry MC but unit-corrupted quantity are repaired from cost basis, current MC, and the verified native price.

## 0.9.238 — 2026-08-24

### Wallet-Scoped Average Lines
- Chart scope now uses only enabled wallets whose eye is open; disabled/hidden wallets cannot leave lines or marks behind.
- Wallet eye, wallet enable, multi-wallet, and Select All changes clear both renderers immediately, then replay only the new scope.
- **Average Buy** (green) and **Average Sell** (red) use fills from each visible wallet's current open round—not lifetime journal history.
- Removed legacy TSL, stop-loss, and take-profit chart rendering and the obsolete popup TSL control.
- Average lines are enabled after migration and remain user-toggleable under **Settings → Fees**.
- **Avg Exit** on the position card now uses the sell/red color.

## 0.9.237 — 2026-08-24

### Hotfix: Widget Not Loading
- Fixed duplicate `avgLinesOn` declaration in `content.js` that prevented the entire content script from parsing (Instant Trade widget never mounted).

## 0.9.236 — 2026-08-24

### Closed Trades Row Compact
- Closed rows show **#11** style labels (no "Closed" prefix, no leading Sol icon) for tighter layout under **Closed Trades**.

## 0.9.235 — 2026-08-24

### Paper Wallets + Settings Polish
- **Paper Wallets menu** shrinks to content (no dead gap above rotation toggles); scroll only when the list is long.
- **Settings → Wallets:** Fill Adapter is now **Paper | DevNet | Mainnet** pill buttons (Paper only; others grayed out).
- **PnL card:** removed empty fallback circle; **token icon + name are larger**.

### Chart Lines Cleanup
- **Average buy/sell lines off by default** — enable in Settings → Fees → **Buy / Sell Average Chart Marks** if you want them.
- **TSL / stop-loss / take-profit lines removed** from the pair chart overlay (B/S bubbles only).
- TV bridge stays for native B/S marks on Axiom/Padre; only the avg/TSL line layer is gated off.

## 0.9.234 — 2026-08-24

### Chart Marks + Eye Toggle Fix
- **Eye toggle is instant:** wallet bubble show/hide flushes chart marks immediately (no 120ms debounce, no wallet-switch workaround).
- **Stale native state cleared** when visible wallet scope changes so marks/lines cannot get stuck hidden while TV thinks they are live.
- **Native overlay gate fixed:** canvas fallback still draws average lines when TV marks are live but order lines are not.
- **Settings → Fees:** new **Buy / Sell Average Chart Marks** toggle (under MEV Protect) to show/hide average buy/sell lines independently of fill bubbles.

## 0.9.233 — 2026-08-24

### Trade History View Toggle
- **Closed Trades** vs **All Trades** segmented toggle on the Trade History header (default: **Closed Trades**).
- Closed view shows completed rounds only (newest first); All Trades shows individual buy/sell fills only — no mixed list.
- Fill labels: **Bought** / **Sold** (replaces In/Out and Buy/Sell on amounts).
- SOL amounts in history rows now include an inline Solana mark beside the number.

## 0.9.232 — 2026-08-24

### Paper Wallets Panel Cleanup
- Removed **Trade Quote** and **Fill Adapter** from the Paper Wallets flyout — moved to **Settings → Wallets**.
- Paper Wallets sidebar **matches widget height** (scrollable list + fixed footer toggles).
- Settings **Wallets** tab: compact trade quote / fill adapter block; long hint list replaced with **Paper Wallet Tips** hover info bar.
- **Quick Buy Rotation** and **Enable Multi Wallet** stay in the Paper Wallets footer only.

## 0.9.231 — 2026-08-24

### Fee / Slippage Defaults + PnL Card Polish
- **Show Fee And Slippage Settings off (default):** slippage, taker fees, priority, gas, and MEV **do not affect** paper fills or PnL.
- When that toggle is **on**, profile fees apply (defaults: **3%** slippage, **0%** taker, **0.01** priority, **0.001** gas, MEV off).
- PnL card: token icon beside name, **SOL Invested** pill with Sol mark, removed Paper Ledger chip, **% under SOL PnL** (red/green, larger), bigger Buys/Sells/Avg stats, **Avg Exit** replaces TSL (sell-side MC average).

## 0.9.230 — 2026-08-24

### Chart Overlay Flicker Fix (Eye Toggle)
- Stopped **square execution-shape** buy markers from flashing when toggling wallet **Eye** on/off on Axiom — those were a stale fallback layer, not real UI.
- Wallet bubble toggles now **debounce** chart replay (no double clear/replay storm).
- When TradingView **getMarks** is hooked, execution-shape fallback is **disabled** so you get one mark system, not three fighting.
- Clearing chart scope now clears **avg lines + marks** together so ghost average lines do not linger at the wrong MC.

## 0.9.229 — 2026-08-24

### Avg Entry + Trade History MC
- Top **Avg Entry** metric now shows **market cap at fill** (same as the PnL card), not slippage-inflated token price that read like ~41K when you bought at ~36K.
- **Trade History** rows now include **MC** — the page market cap recorded on each buy/sell.

## 0.9.228 — 2026-08-24

### Chart Marks + Average Lines Fix
- Split native chart state so **B/S bubbles** and **Average Buy/Sell lines** no longer fight: when Axiom draws fill marks but order lines fail, the SVG overlay still paints avg/TSL lines (no duplicate pins).
- Chart scope always includes the **active wallet** when it holds the open mint (eye visible), even if rotation stats scope was empty.
- Collapsing the panel (−) **auto-closes** the Paper Wallets sidebar.
- Instant Trade ⚙ settings now exposes **Show Chart Marks** (same toggle as extension popup).

## 0.9.227 — 2026-08-24

### In-Place Fee Pills
- Tap **Slippage**, **Priority Fee**, or **Gas Fee** to type the value on the pill (Enter saves, Escape cancels). Buy and sell both update.
- Tap **MEV Protection** to toggle On / Off. Settings sheet still has split buy/sell if you need them different.

## 0.9.226 — 2026-08-24

### Audit Close-Out (P0 / P1)
- Share fills, chart markers, hydrate rounds, and exec charts use **scoped journal** + wallet scope (no pre-reset ghost fills).
- Dashboard replay/share paths use scoped journal + live rounds for stats.
- Post-reset closed-trade rows filtered from live breakdown UI.
- Wallet sidebar explains **Enabled vs Active vs Eye**; Multi Wallet auto-turns Rotation Off.
- CTA approve: extension polls **platform alert feed** (`cta_approved_ready`) then `lease-cta/ready`; marks alert read on Start.

### Retired Wallets + Contest (0.9.225 carry)
- Wallet reset retires book epoch — full journal retained; live stats / leaderboard use watermarks.
- Dashboard profit calendar toggle **Include Retired Wallets In Calendar**; **Retired** badges on journal rows.
- Backend stores full history; weekly contest forfeits on post-snapshot wallet reset (migration 185).

## 0.9.225 — 2026-08-24

### Retired Wallets + Journal Accountability
- Wallet reset **retires** a book epoch — journal + closed rounds stay in storage for audit (not deleted).
- Live stats, overlay PnL, profit calendar (default), and leaderboard use reset watermarks (live wallets only).
- Dashboard journal + closed trades show **Retired** badges; profit calendar toggle **Include Retired Wallets In Calendar**.
- Server sync stores full history; platform weekly leaderboard excludes forfeited users after contest snapshot lock.

## 0.9.224 — 2026-08-24

### Token Row Metrics Layout
- Price + Market Cap share the row width (no `margin-left: auto` shove off the right edge).
- Open position: hide token icon + name; Tokens / Price / Market Cap boxes split the row evenly.
- No position: icon + name stay; Price and Market Cap flex-fill remaining space without clipping MC.

## 0.9.223 — 2026-08-24

### Select All With Balance Toggle
- When every book with SOL is on, the button turns red and reads **Unselect All With Balance** — one click clears them all.

## 0.9.222 — 2026-08-24

### Wallet Reset Stats + Multi-Wallet Sell
- Invested / Sold / Remaining / Fees / PnL ignore journal + closed rounds voided by paper wallet reset (no lifetime compounding after reset).
- Reset All clears the short-lived closed-trade chip.
- Enable Multi Wallet (rotation off): 10% / 25% / 50% / 100% sell runs across every selected book with a position; sell buttons show **×N** like buys.

## 0.9.221 — 2026-08-24

### PnL Row Font Size
- Invested / Sold / Remaining / Fees / PnL labels and values keep the same fitted size when no wallet is selected (zeroed row no longer shrinks).

## 0.9.220 — 2026-08-24

### Chart Bubble Eyeballs
- All wallet eyeballs off → **no** B/S bubbles on the chart (empty wallet scope no longer shows every fill).
- Native TV marks + overlay markers clear when no books are visible; new fills skip hidden wallets.

## 0.9.219 — 2026-08-24

### Wallet Empty State + Token Identity vs Holdings
- Unselect every paper book → wallet bar **No Wallet Selected**, no SOL amount; buys disabled.
- One book → name tag; multi → square count badge (**2** / **3**), not joined names.
- Full symbol + token name when no selected book holds the mint; hide identity and show Tokens box only when a selected book has a position.
- PnL **Remaining** label still fits when the row is zeroed (label fit no longer skipped).

## 0.9.218 — 2026-08-24

### CTA Claim-On-Accept + Quiet Lease Toasts
- Admin CTA approve unlocks a **Start** grant — the +24h clock does **not** begin until the user Accepts in popup or Instant Trade.
- Instant Trade: sticky **CTA Approved — Start** toast (eye = hide for now); low-time (<30m) toast once per lease, eye hides until that lease ends.
- Requires backend migration **183** + API routes `lease-cta/ready` + `lease-cta/claim`.

## 0.9.217 — 2026-08-23

### Wallet Bar + Multi Wallet + Fee Settings
- Wallet selector: **Wallet** left, Solana mark beside the amount (replaces `SOL` text), full tag room for Main / Alt 1 / …
- **Enable Multi Wallet** under Quick Buy Rotation — select several books; Rotation On = one-at-a-time, Off = simultaneous buy (e.g. 0.1 × 2 wallets).
- **Show Fee And Slippage Settings** in Behavior (off by default). Compact one-line chips: Slippage · Priority · Gas (Solana mark) · MEV **On**/Off (green/red).

## 0.9.216 — 2026-08-23

### Lease Registry + CTA Earn + 7d AAI
- **Admin desk:** `/dashboard/admin/alpha-trench-leases` shows active leases in the wild (user, via, time left, JTI), revoke, and CTA claim approve/reject.
- Every lease mint is logged to `alpha_trench_session_leases` (migration `182`) so JWT counts are queryable.
- **Windows:** trial **1h** → CTA earn (tweet / Discord handle, admin approve) **+24h** → Insert Coin AAI **7d** → entitled/admin/tester **48h**.
- Extension Link tab: Submit For Admin Approval for tweet/Discord CTA.

## 0.9.215 — 2026-08-23

### Insert Coin + Lease Countdown
- Popup shows a live **Lease Ends In …** countdown (amber under 2h, orange under 30m, red when expired).
- **Insert Coin · Renew 24h** spends AAI on gate `alpha_trench_session_lease` (25 AAI / 24h) and mints a fresh trench lease JWT on confirm — arcade renew without waiting for the short web access token.
- If the session JWT is already dead, UI tells you to **Link From Alpha Tek Tab** first, then Insert Coin.
- Migration `181_alpha_trench_session_lease_spend_gate.sql` seeds the spend pricing row (no new Render env vars).

## 0.9.214 — 2026-08-23

### Extension Session Lease (48h / Arcade Trial)
- **Root cause:** Link From Tab copied the web `alpha_token` access JWT (~**15 minutes**). The extension cannot use the site’s HttpOnly refresh cookie, so Fusion Drilldown / Mint Intel died with **Invalid or expired token**.
- **Fix:** After Link / Probe Auth, the extension calls `POST /api/data/alpha-tools/trench/session-lease` and stores a longer **trench lease JWT** (same auth stack, `purpose: alpha_trench`).
- **Entitled 48h:** admin, `extension_tester` / `trench` / paid tiers (`alpha`, `pro`, `vip`, …), or AAI unlock hints.
- **Arcade trial 1h:** everyone else with a valid session — free window before re-link (AAI “feed the machine” renew path next).
- Admin Users page: set subscription tier to **`extension_tester`** to grant 48h leases without making someone a full admin.
- Popup shows remaining lease time after link.

## 0.9.213 — 2026-08-23

### Auto-Expand On Drilldown
- Fusion / Deep / Coach drilldown panels raise their max height (`min(55vh, 560px)` vs the old 220px clip).
- Opening or closing a drilldown **auto-refits** the Instant Trade panel height so the extra research space appears without manual resize.
- Sticky height locks clear when content outgrows them, so a previously short panel still expands for the drilldown.

## 0.9.212 — 2026-08-23

### Deep Intel Preview Open + Cleaner Research Panel
- **AAI gates (preview):** Deep Intel / Coach / depth modules open to any **linked Alpha Tek session** (`AAI_GATES_LINKED_PREVIEW`) so QA can exercise the rails before tokenization spend gates return.
- Removed the **Not Trade Signals — TG / Trending / KOL / Fusion Evidence** footer under Mint Intel.
- Probe Auth reads `isAdmin` from JWT + `/api/auth/me` so admin accounts unlock cleanly.
- Backend Coach mirrors the preview (`COACH_LINKED_PREVIEW`) for authenticated sessions.

## 0.9.211 — 2026-08-23

### Fusion Drilldown Stay Open
- **Root cause:** Every Mint Intel refresh (detect resolve, settings sync, `renderAll`) reset `drilldownOpen` and wiped `#fusionDd`, so Fusion Drilldown flashed then vanished on its own.
- Open drilldown now **persists across same-mint intel refreshes**; only clears on mint change, unlink, or **Hide Drilldown**.
- Detect-loop resolve no longer force-clears intel cache when the mint did not change.

## 0.9.210 — 2026-08-23

### Mint Intel Session Error Clarity
- **Root cause:** Fusion Drilldown / Mint Intel hit `/api/tg-calls/*`, which requires a valid Alpha Tek JWT. A stale pasted/`Link From Tab` session returned the backend string **Invalid or expired token** — easy to confuse with the Solana mint CA.
- API client + intel layer now map 401/403 JWT failures to **Alpha Tek Session Expired — re-link from the popup**.
- Empty confluence no longer silently shows **No Mint Intel Yet** when every TG call failed auth; pills say **Session Expired — Re-Link Alpha Tek**.

## 0.9.209 — 2026-08-23

### Chart Bubble Stability + Per-Wallet Hide
- **Crash fix:** When Axiom’s TradingView shell skips `getMarks`, the bridge no longer paints long black `Buy · Wallet · SOL` text stacks. Execution-shape fallback now uses **B/S** pins; the SVG overlay stays active until real native marks hook.
- **Navigation:** Token/chart context changes reset shape-fallback state and replay journal fills so page hops recover bubbles instead of leaving text-only markers.
- **Paper Wallets:** Eye icon beside **Bubble Color** toggles chart buy/sell bubbles per wallet (wallet stays on for trading/stats).

## 0.9.208 — 2026-08-23

### MTM PnL Flash Guard
- **Root cause:** On reload, a stale resolver market cap could briefly disagree with the live Axiom header MC by hundreds of times. `scaleMarkToPageMcap` scaled `priceNative` up to match, so `qty × mark` showed tens of thousands of SOL remaining until the next good tick arrived.
- Refuse MC scale ratios outside the existing tick magnitude band (20×).
- Open-position Remaining/PnL now fall back to fill cost or last fill mark when the live page mark disagrees wildly with position cost.

## 0.9.207 — 2026-08-23

### Trade Snapshot Chart Fix
- **Root cause:** B/S mark prices were taking `mcap` when USD/SOL price was missing, which blew the Y-scale to millions and crushed Birdeye candles flat along the bottom.
- Marks now use **priceUsd → priceNative only** (never mcap). Candle pane Y-scale uses candles alone.
- Pins snap to the **nearest candle bar** (same X as OHLC), with light stagger when many fills share a bar.
- Removed full-height dashed vertical lines on buys/sells.
- B/S triangles ~12% smaller with black lettering so stacked fills stay readable.
- Clips oversize Birdeye windows to the trade span so pins are not shoved to the far right.

## 0.9.206 — 2026-08-23

### Compact Cover Size + Readability
- **Vertical resize** (north/south handles): grow **taller without widening** — visual width stays fixed while scale increases.
- **Extra height** below content when you drag past natural size (helps cover Axiom’s real **Buy** button).
- Resize no longer snaps back on release — uses sticky sizing so your chosen scale/height sticks.
- **~10% larger text** in compact width (~320px layout): price, MC, wallet, PnL tiles, buy/sell buttons, fee row.
- Default compact scale **0.82 → 0.88**; max scale **1.15 → 1.22**.

## 0.9.205 — 2026-08-23

### Token Name + Viewers Layout
- **Viewer count** moved to the **top header** (beside live dot) so it no longer competes with the symbol row.
- Symbol row flexes to use available width; subtitle name line keeps more room beside price/MC metrics.

## 0.9.204 — 2026-08-23

### Fee Row Type
- Slippage, Priority Fee, Gas Fee, and MEV Protection pills are about 12% larger (8px → 9px) with taller line-height so the labels fill the extra pad.

## 0.9.203 — 2026-08-23

### Last-Used Profile Per Site
- Instant Trade remembers which of **P1 / P2 / P3** you last used on each trench host (Axiom, Padre, and the rest).
- Compact panels open on that site’s profile, not always P1. A first visit to a host falls back to your current profile.
- Uses **Remember Overlay And Profile Per Site** — turn it off and the pad stays on one global profile.

## 0.9.202 — 2026-08-23

### Origin Tweet Close
- The panel **X** now closes Origin Tweet on pointer-down (stable listener on the overlay, not a button that gets rebuilt).
- Overlay stacks above Instant Trade so the close control is not sitting under the token chip.

## 0.9.201 — 2026-08-23

### Origin Tweet Panel
- **X chip:** Reset the default gray button chrome so the X glyph actually paints next to the token.
- **Blacklisted origin:** Red box around that X chip (and the X mark in the profile card).
- **Panel layout:** Opens aligned to the top of Instant Trade, same height as the extension, with a right-hand scrollbar so the full tweet is readable.
- **Fresh Tweet:** One thin row — status on the left, age on the right. Hover for “Posted within the last 30 minutes.”
- **Profile:** Join date + follower count in the X Profile block. One **View Profile On X** button (duplicate text link removed) plus **Blacklist Profile** with a confirm step.
- **Stats:** Real heart / views / repost / bookmark glyphs instead of emoji tofu.

## 0.9.200 — 2026-08-23

### Compact Trade Profile Menu
- When Instant Trade is narrow (about 400px or less), the three P1 / P2 / P3 chips collapse into one **Trade Profiles** button.
- Click it for an opaque dropdown of P1, P2, and P3 (or your renamed labels). Pick a profile the same way as the chips.
- Stretch the panel wider and the three chips come back.

## 0.9.199 — 2026-08-23

### Trade-page-only overlay + slimmer positions bar
- **Trench panel** hides on Axiom Discover, Pulse, Portfolio, and other non-token routes — only shows when the URL has a CA (`/meme/…` or `/t/…`).
- **Positions bar** stays available for open-position chips; thinner height (30px), **AT logo** instead of “Alpha Trench” text.
- **Share PnL / Replay** on bar chips appear on hover only (chip expands when hovered).

## 0.9.198 — 2026-08-23

### Stable metrics + wallet bar label
- **PnL row:** No font-size pulse when Invested/Sold/Remaining/Fees/PnL are all zero — skips JS fit and updates cells in place.
- **Price metric:** Fixed decimal width (`fmtPriceFixed`) so SOL price ticks do not shrink the widget.
- **Holdings / MC:** Tabular min-width when a position is open; token qty uses fixed 4 decimal places.
- **Wallet bar:** Shows Solana logo + **Wallet** + wallet label + balance so the picker reads clearly.

## 0.9.197 — 2026-08-23

### Header bar UX
- Paper wallets header button shows **$** instead of **W**.
- **No hover tooltips** on the full top header row (AT logo, profiles, status dot, settings, lock, help, collapse).
- **AT logo** opens a side dropdown: promo copy, **Visit Alphatek.app**, **Log In / Dashboard**, and **Join Discord** links.

## 0.9.196 — 2026-08-23

### Chart B/S bubble letters
- Buy/sell pin letters are **bold black** on all wallet bubble colors (overlay + native TV marks + replay chart).
- Bubble fill stays wallet-colored; only the **B** / **S** glyph changes so green-on-green no longer hides the letter.

## 0.9.195 — 2026-08-23

### Solana mark — broken image fix
- Added `icons/solana.png` to `web_accessible_resources` so trench host pages can load the coin icon (was 404 / broken image).

## 0.9.194 — 2026-08-23

### Instant Trade panel resize (right-edge clip fix)
- **Sized panel** drops CSS `max-width` cap that ignored `left` position — fixes empty right gutter / clipped content when docked on terminal buy/sell column.
- Viewport fit now **shrinks width/scale** when pinned to the right instead of only sliding left past the edge.
- Resize handles cap east/west growth to available viewport width.
- Tighter edge snap (4px) so the panel can sit flush on the right.

## 0.9.193 — 2026-08-23

### Paper wallet sidebar — included highlight
- **Enabled** wallets (toggle ON) now show the teal highlight border — not only the active trade wallet.
- **Trade Focus** adds a stronger glow on the wallet used for buys/sells and bubble color.
- **Select All With Balance** refreshes full stats after enabling every wallet with cash.

## 0.9.192 — 2026-08-23

### Dashboard wallets — unrealized PnL
- **Wallets** tab shows unrealized P/L beside each wallet’s open count (e.g. `1 Open · −11.076 SOL` or `1 Open · −$2,450.00`).
- Respects Instant Trade **Display Balance Unit** (SOL vs USD). USD uses cached SOL price from trench ticks or Jupiter fallback.

## 0.9.191 — 2026-08-23

### Solana mark (wallet bar + price)
- Replaced pinched gradient SVG bars with bundled **Solana coin icon** (`icons/solana.png`, same asset family as platform `CHAIN_LOGOS`).
- Fixed sizing CSS so the mark keeps square aspect ratio at 13–15px (no forced square squash on wide SVG).

## 0.9.190 — 2026-08-23

### Multi-wallet stats + journal trade history
- **Enabled wallet toggles** again drive **combined** Invested / Sold / Remaining / Fees / PnL across all ON wallets (active wallet still controls buys/sells and bubble color).
- **Trades** header count matches bottom **Buys + Sells** — each journal fill is one trade (not one closed round).
- Expanded trade list shows **every buy/sell fill** in a scrollable panel; prior **Closed** rounds listed below with Replay.
- Chart markers and holdings header aggregate enabled wallets again.

## 0.9.189 — 2026-08-23

### Safari Mac preview (companion pack)
- New **Alpha Trench for Safari** pack under `extensions/alpha-trench/safari/` — packed from this Chrome MV3 tree, Chrome folder unchanged.
- Unsigned / temporary Safari load (Develop menu). `offscreen` permission dropped; Music Lite stays Chrome-only.
- Docs + zip: `safari/README.md`, `safari/dist/alpha-trench-safari-0.9.189.zip`.

### Paper wallet color picker + Solana mark
- **Bubble Color** grid stays open until you click away — no longer wiped by live price/widget refresh.
- **Solana logo** in wallet selector and price row: official green→purple gradient SVG (replaces thin mono glyph). **SOL** text kept beside balance for clarity.

## 0.9.188 — 2026-08-23

### Paper wallet color picker UX
- **Bubble Color** opens only on the **selected** wallet row; clicking the swatch on another wallet **selects that wallet first** (no picker).
- Removed row **opacity** dimming that washed out Alt rows and made the color grid look transparent.
- Color menu uses a solid card background.

## 0.9.187 — 2026-08-23

### Average Buy MCAP source clarity
- Chart **Average Buy** line now prefers **position avgEntryMcap** (recorded at each fill from live page MCAP) before journal gaps.
- Bottom **Avg Entry** matches the same priority order.

## 0.9.186 — 2026-08-23

### Widget stats scoped to selected wallet
- **Invested / PnL / Buys / Avg Entry** (top row + bottom card + chart avg lines) now follow the **active paper wallet** you click in Paper Wallets — not an aggregate of all enabled toggles.
- Sidebar wallet toggles only control **Quick Buy Rotation** (tooltip updated); they no longer inflate buy counts or PnL when another wallet is selected.
- **Average Buy** line uses the same active-wallet scope so the chart line matches the bottom **Avg Entry** readout.

## 0.9.185 — 2026-08-23

### Origin tweet age + profile intel
- **Fresh / Recent / Old** banner on hover pop and left panel: green (&lt;30m), yellow (30–90m), red (&gt;90m) with age readout (e.g. **12m Ago**).
- **X Profile** card in panel and hover: avatar, name, handle, followers, join date, optional Alpha label (when linked), **View Profile On X**.

## 0.9.184 — 2026-08-23

### Average Buy line on chart
- **Average Buy** native line renders again when blasting buys on MCAP charts (mint/pair alias matching + USD/MCAP axis fallbacks).
- Journal qty-weighted avg buy; **cost ÷ qty** only backs up **entry price in SOL** when journal rows lack price — then scales to MCAP via live page `token.mcap` / `fillMcapForToken` (not a substitute for current MCAP).
- Buy and sell avg lines sync independently (sell no longer blocks buy).

## 0.9.183 — 2026-08-23

### Locked fill bubble colors
- Each buy/sell journal entry stores **bubbleColor** at fill time (wallet swatch when the fill landed).
- Chart bubbles keep that locked color even if you change the wallet swatch later — use different colors across sessions to separate old vs new fills on the same coin.
- Paper Wallets hint + Wallets settings tab explain the workflow.

## 0.9.182 — 2026-08-23

### Origin tweet intel panel
- **X icon** on token header: hover shows tweet preview (author + snippet); click opens **Origin Tweet** panel on the left (wallet-menu style overlay).
- Prefetches tweet text, media, and stats via extension fetch (syndication + fallback).
- **Blacklist Profile** / **Remove Blacklist** on author; blacklisted profiles show a distrust mark on the chip.
- **Read More On X** opens the permalink when you want the full thread on X.

## 0.9.181 — 2026-08-23

### Per-wallet chart bubble colors
- **Paper Wallets** rows: compact **Bubble Color** swatch opens an 8-color preset grid.
- Bubble **background/border** uses the wallet color; **B** letter stays green, **S** stays red (native TV + SVG overlay).
- Color persists per wallet and reapplies on journal replay when you change it.

## 0.9.180 — 2026-08-23

### Advanced settings UX
- **Stop Loss** / **Take Profit**: full-width sliders (0–50% / 0–100%) with live **−10%** / **+25%** readout; Off at zero.
- **Custom Buy Amounts**: green SOL chips; **✎** edit mode with numeric-only inputs and **+** add.
- **Custom Sell %**: red percent chips; same pencil edit flow.
- **Execution Delay**: slider 0–3000 Ms (50 Ms steps).

## 0.9.179 — 2026-08-23

### Instant Trade Settings sheet
- **Close** moved to top-right (×) — no longer blocks footer text.
- Wallets tab hints compacted to a short bullet list; tighter row spacing to reduce scroll.

## 0.9.178 — 2026-08-23

### Chart buy/sell bubbles
- **Enabled paper wallets:** all buy/sell bubbles from selected wallets show on the chart; toggling a wallet off removes its bubbles.
- **Average Buy / Average Sell** lines use qty-weighted averages across enabled wallets only.
- Hover tooltips: **Buy · Main · 0.50 SOL** / **Sell · Alt 1 · 0.48 SOL** (native TV + overlay).
- Sell bubbles render when mcap is present even if native price is thin.

## 0.9.177 — 2026-08-23

### Token header metrics
- Price, Market Cap, and Tokens chips: label and value lines centered in each box (including morph hover states).

## 0.9.176 — 2026-08-23

### Buy presets
- Buy amounts above the **active** paper wallet balance are **disabled and grayed** — no insufficient-balance error bar.
- Wallet bar shows **active wallet** cash (matches the wallet name tag).
- Hover wallet tag (**MAIN**, etc.) fades in **below** the SOL amount without shifting the label.

## 0.9.175 — 2026-08-23

### Token header metrics
- **Price** and **Market Cap** chips visible again — metric stacks use grid sizing instead of absolute positioning that collapsed chip width to zero.

## 0.9.174 — 2026-08-23

### Dropdown toggle
- Fill Adapter (and other custom dropdowns): click the trigger/chevron again to **close** — fixed shadow-DOM click handling.

## 0.9.173 — 2026-08-23

### Token metric chips
- Price and Market Cap sit **tight on the far right** (no oversized equal columns).
- **Tokens** chip slides in left of Price when you have a position (Tokens · Price · Market Cap).

## 0.9.172 — 2026-08-23

### USD balance display
- **Wallets** settings: **Display Balance** toggle (SOL / USD) for spot paper wallets and PnL row.
- Click any **Invested / Sold / Remaining / Fees / PnL** cell to pin USD view (hover hint via row highlight).
- Live **SOL/USD** cached from page ticks when available.

### Hyperliquid perps paper (beta)
- Axiom **Perpetuals** routes detect `hl:` perp tokens (e.g. BTC-USD).
- USDC margin account ($10k start): long via **$ Margin** chips, close via **%** sells.
- Fee row shows HL-style slippage + taker fee labels on perps pages.
- **Wallets** tab: **Paper Chain** (Solana / Hyperliquid) + **Perps Leverage** default.

## 0.9.171 — 2026-08-23

### Token header metrics
- Horizontal **Price**, **Market Cap**, and **Tokens** cards across the token banner (not a cramped right stack).
- Hover morph: **Tokens** → **Avg Entry**; **Market Cap** → **All-Time High** (journal + live mcap).
- Click pins the alternate metric; click again restores default.
- Token qty uses the same value typography as price and mcap; holdings rollup across enabled wallets.

### Settings sheet readability
- Larger labels and number inputs (15px tabular, wider boxes, clearer borders).
- Buy / Sell and Advanced fields use label + input rows so decimals stay visible.

## 0.9.170 — 2026-08-23

### Paper wallet stats scope
- Stats / trade history only when wallets are **included** (toggle on); all off → zeros, no trades.
- Trade list newest-first; compact timestamps (`33m Ago`, `1H Ago`, `3D Ago`).
- No fallback to active wallet when every include toggle is off.

## 0.9.169 — 2026-08-23

### Paper wallets
- Fix include toggles (no longer nested inside button rows).
- Balance bar shows sum of **enabled** wallet cash; active wallet name in tag only (no “Paper Wallet” label).
- Invested / sold / fees / PnL rollup across all enabled wallets for the mint.
- Stronger active-wallet glow; excluded wallets dimmed.
- Trade History header; Fees Paid with % on hover; relative trade times with full date on hover.
- Trades bar chevron matches wallet bar styling.

## 0.9.168 — 2026-08-23 (Public open beta prep)

### Trade UI
- Wallet bar: Paper Wallet + Solana glyph + wallet tag; chevrons meet in the middle for wallet vs trades dropdowns.
- Trade rows: single-line layout with larger date/time, Solana glyph, Buy / Sell / Profit, Replay (no fee clutter).
- Buy chips: wallet name on hover only; centered Buy / Sell pills.
- Settings: toggle sliders, volume range, side-by-side Trade Quote chips.
- Trade Closed toast: compact centered card with PnL and time.

### Charts
- Average Buy / Average Sell lines park on fill-weighted MCAP (no flutter with live candles).
- PnL card snapshots: adaptive candle resolution (1m → 5m → 15m → 1H → 4H) by hold length.
- Trade Replay dashboard: same bar-budget logic as PnL cards; manual **4H** chip added.

### Docs
- Public install, security inspection, FAQ, Chrome Web Store runbook, logo concept brief.

## Earlier builds

See [README.md](README.md) status table and [docs/TESTING_GUIDE.md](docs/TESTING_GUIDE.md) for feature history by version band.
