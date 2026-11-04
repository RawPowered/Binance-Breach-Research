# Financial accounting: stolen, replaced and still outstanding

**Reviewed November 4, 2026, 22:15 UTC / 16:15 CST (America/Chicago).** Public-source assessment, not an independently audited ledger or a live balance feed. Earlier dated research is preserved.

## What can be stated

| User's question | Best supported assessment | Precision and meaning |
|---|---|---|
| How much was compromised? | Full potential exposure is **unknown**. The reported incident impact is approximately **$6.34 billion**. | Value stolen is not a measurement of every asset the compromised permissions could reach. [F1](https://www.binance.bh/en/blog/community/3229153443759566763) |
| How much was stolen? | Use **approximately $6.34B** as the company baseline. Published investigator estimates span **$6.30B–$6.43B**. | This is a source-estimate span, not a confidence interval or additional losses. [F1](https://www.binance.bh/en/blog/community/3229153443759566763), [F3](https://www.bitquery.io/investigations/binance-hack), [F4](https://www.elliptic.co/insights/binance-largest-hack-in-history/), [F6](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history) |
| How much has the company “paid back”? | Binance reports **98% replenished**, with **more than 100% of required funding set aside**. | Coverage/replacement, not a public cash-disbursement ledger. Actual purchase expenditure and customer payouts are not established here. [F2](https://www.binance.com/en/square/post/384674399709556) |
| How much stolen value has been stopped? | Approximately **$2.85B frozen/intercepted**, reported November 3. | Blocked assets are not necessarily delivered back to Binance. [F1](https://www.binance.bh/en/blog/community/3229153443759566763) |
| How much original stolen value has been returned? | **No reconciled total established in this review.** | Unknown does not mean zero. Require recipient-controlled settlement evidence before calling a freeze a return. |
| How much is still with the attacker? | Bitquery estimates **about $3.1B**, mainly BTC/ETH, at **09:56 UTC November 4**. | Attributed holdings estimate; much is idle. It is not an exact total actively circulating or cashed out. [F3](https://www.bitquery.io/investigations/binance-hack) |

## Replacement funding: the dollar calculation is conditional

Using the company baseline purely as an illustration:

| Calculation | Result | Interpretation |
|---|---:|---|
| $6.34B × 98% | $6.2132B, approximately **$6.21B** | Indicative replacement equivalent |
| $6.34B × 2% | $0.1268B, approximately **$126.8M** | Indicative remaining token-sourcing equivalent |

The percentages come from [Recovery Update #7](https://www.binance.com/en/square/post/384674399709556), not an audited dollar expense schedule. These calculations assume the coverage percentage uses the same USD denominator and valuation date as $6.34B; the reviewed disclosure does not establish that equivalence. Do not present either result as an exact payment or liability.

The [October 31 Update #3](https://www.binance.com/en-AU/support/announcement/detail/1fdf1f61559c401da0435895ffcccb62) identifies SAFU, the Futures insurance fund and corporate treasury as replacement resources, and reports more than $6.34B reserved. It does not itemize an exact dollar contribution from each. Assets already held and assets newly purchased need not have the same acquisition cost.

Funding reserved, token replacement completed, withdrawals paid to customers, and original stolen tokens returned are four different measures. A promise to cover all losses does not establish completed purchases for every token.

## What “still circulating” means

Three questions need different numbers:

1. **Still attributed to attacker-controlled holdings:** use F3's dated estimate above. That is the best current holdings observation located in this review.
2. **Currently moving through laundering routes:** no exact aggregate established. Repeated swaps and transfers can count the same value many times.
3. **Successfully cashed out to the operator:** no exact aggregate established. A bridge, exchange deposit or market-maker swap alone does not establish final cash-out or the operator's net proceeds.

F3's headline uses a 09:56 UTC snapshot, but its methodology includes newly counted wallets through 11:28 UTC, excludes a $1.3M DAI wallet and some onward-moving SOL/BTC, and warns labels may be incomplete. Its nine-chain scope and morning holdings prices limit completeness. This project has not replayed those balances. [Bitquery methodology](https://www.bitquery.io/investigations/binance-hack)

As a historical cross-check, Elliptic's November 1 version estimates approximately **$3.25B** in issuer-unfreezable assets. It is neither a November 4 balance nor an additional amount to add to F3. [Elliptic](https://www.elliptic.co/insights/binance-largest-hack-in-history/)

## Why subtraction does not produce an exact live balance

| Arithmetic from reported figures | Result | What it cannot establish |
|---|---:|---|
| Company impact $6.34B − reported frozen/intercepted $2.85B | **$3.49B** | Current holdings, active laundering volume or cash-out |
| Elliptic theft $6.43B − frozen/seized $2.85B | **$3.58B** | A current reconciled balance or an independently measured remainder |

These are residuals from approximate published inputs. They do not reconcile token by token, at one price timestamp, across common address labels. Elliptic explicitly values theft at transfer-time prices and freezes at current prices. [Elliptic valuation note](https://www.elliptic.co/insights/binance-largest-hack-in-history/)

The difference between a residual and a later holdings estimate must **not** be labeled recovered, missing or cashed out without evidence. Market prices, swaps, fees, collateral/debt, third-party proceeds and incomplete tracing all require separate reconciliation. Funds can remain traceable after being swapped; frozen funds can remain in attacker-address balances while being unusable.

Similarly, do not subtract company replacement purchases from the stolen-funds balance. Replenishment changes Binance's backing position; it does not remove stolen coins from attacker control. Do not add the replacement amount to gross theft and call the sum a new theft total.

## Source register and date conflicts

| ID | Source/version | Accounting role and access |
|---|---|---|
| F1 | [Binance preliminary findings, November 3](https://www.binance.bh/en/blog/community/3229153443759566763) | Company impact and freeze estimates. Direct report opened. Approximate, reconciliation and market volatility caveats apply. |
| F2 | [Binance Announcement, Recovery Update #7, November 4](https://www.binance.com/en/square/post/384674399709556) | Latest replenishment claim. Indexed official text inspected; direct page failed. Official [support index](https://www.binance.com/en/support/announcement/list/0000000000000000000000049) corroborates publication; [regional official copy](https://www.binance.com/en/square/post/384675891033200) supplies indexed text. |
| F3 | [Bitquery, November 4 version](https://www.bitquery.io/investigations/binance-hack) | Original holdings investigation; direct page and methodology opened. Header cutoff and later sub-observations differ as noted above. |
| F4 | [Elliptic, updated November 1 at 08:00 UTC](https://www.elliptic.co/insights/binance-largest-hack-in-history/) | $6.43B theft across 11 chains, $2.85B frozen/seized, historical holdings and valuation basis. Direct page opened. |
| F5 | [Binance Recovery Update #3, October 31](https://www.binance.com/en-AU/support/announcement/detail/1fdf1f61559c401da0435895ffcccb62) | Funding sources and earlier coverage; direct page opened. |
| F6 | [TRM initial investigation, October 29, figures through October 30 00:30 UTC](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history) | $6.36B across ten chains. Historical estimate, not November 4 holdings. Earlier inspected source retained for comparison. |

F1 retrospectively places 98% replenishment at October 31, while F5 reports 90% that day and the [November 2 update](../updates/2026-11-02/README.md) records 95%. The source chronology is inconsistent. This assessment anchors the current 98% claim to F2's November 4 publication and does not silently rewrite earlier snapshots.

This review did not verify the new proof cryptographically or inspect an audited company expense ledger. A proof-of-reserves snapshot by itself does not itemize replacement spending, prove restitution of stolen assets or establish every company liability.

## Requirements for an exact reconciliation

An exact assessment needs a transaction-level withdrawal list with chain, transaction ID, token contract and units; one common price timestamp; reconciled address labels across providers; freeze/unfreeze and rescue events; confirmed return receipts; current assets and linked liabilities without bridge double counting; and company records separating purchases, existing inventory, reserve transfers and customer disbursements.

Until those are available, retain source-specific estimates and cutoffs. The useful conclusion is substantial company replacement **alongside** substantial attacker-retained value; those facts are compatible.

[Main overview](../README.md) · [Sources](../SOURCES.md) · [Original financial observations](financial-estimates.csv)
