> Distribution update: future Alpha Trench packages are delivered through authenticated [AlphaTek.App](https://www.AlphaTek.App/alpha-trench) downloads. This repository no longer contains package archives or development source.

## Alpha Trench v0.9.239 — Axiom Price-Unit Safety Fix

### Critical Fix
- Correctly interprets Axiom compact USD notation such as `$0.0₃2` as `$0.0002`.
- Stops broad page-text scanning from treating wallet balances, fees, or order sizes as SOL-per-token.
- Requires an explicit native-price field or a USD/native pair that implies a plausible SOL/USD rate before bootstrapping.
- Cross-checks paper execution price against trusted SOL/USD and fails closed if the unit remains unverified.
- Repairs affected open-position token quantity when Avg Entry MC provides an independent fill-time anchor.

### Example
At approximately `$246K` market cap and `974M` supply, token price is about `$0.0002526`—not two cents. A 30 SOL paper buy should therefore receive millions of tokens, not roughly 1,500.

### Packages
- **Windows / Chrome / Edge:** `alpha-trench-0.9.239.zip`
- **Safari 18+ preview:** `alpha-trench-safari-0.9.239.zip`

---

## Alpha Trench v0.9.238 — Wallet-Scoped Charts and Trade UI Polish

### Windows / Chromium + Safari
- **Wallet-scoped chart marks:** enabled wallets with an open eye are the only books allowed to draw B/S bubbles and average lines.
- **Immediate chart actuation:** Eye, wallet enable, Multi Wallet, and Select All changes clear stale renderers before replaying the new scope.
- **Correct averages:** Average Buy (green) and Average Sell (red) use each visible wallet's current open round instead of lifetime fills.
- **Legacy lines removed:** TSL, stop-loss, and take-profit chart lines and the old popup TSL control are gone.
- **Trade History:** Closed Trades is the default compact view; All Trades shows individual fills. Closed rows use `#1`, `#2`, and so on.
- **Paper Wallets:** Trade Quote and Fill Adapter moved to Settings → Wallets; the wallet menu is compact and keeps rotation controls in its footer.
- **Fill Adapter:** Paper is the available adapter; DevNet and Mainnet are visible but disabled in the compact three-button selector.
- **PnL card:** larger token identity, SOL Invested mark, red Avg Exit, clearer percentage, and tighter stats.
- **Fee behavior:** hidden fee/slippage settings no longer affect paper fills. When enabled, the configured profile values apply.

### Fixes Since 0.9.226
- Fixed the extension-content syntax regression that briefly prevented the widget from mounting.
- Removed stale TradingView shape fallback flashes and ghost average lines.
- Eye toggles now add/remove marks without requiring a wallet switch or second click.
- Avg Entry and trade history market caps use fill market cap rather than slippage-inflated token price.

### Packages
- **Windows / Chrome / Edge:** `alpha-trench-0.9.238.zip`
- **Safari 18+ preview:** `alpha-trench-safari-0.9.238.zip`

### Install / Verify
1. Reload Alpha Trench in the browser extension manager.
2. Hard-refresh the active pair page.
3. Confirm disabling all wallets or eyes clears every B/S mark and average line.
4. Confirm Average Buy is green and Average Sell / Avg Exit are red.
