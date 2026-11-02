# Binance breach: why asset choice mattered

Dated research snapshot: October 31, 2026 CDT. This graphic explains post-theft containment and recovery, rather than establishing how the original intrusion succeeded. Sources were revisited during production; it is not a live status report.

## Numbered sources

1. [Elliptic, Binance theft analysis, updated October 31](https://www.elliptic.co/insights/binance-largest-hack-in-history/). Supports the token/native-asset distinction, reported ETH/TRX conversions, lending and later cross-chain movements. Its frozen/seized estimate is approximately $2.85B, at its stated valuation cutoff, excluding the Aave position.
2. [TRM Labs, Binance investigation](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history). Supports reported borrowing against USDT, costly swaps, token freezes and screening of linked deposits. It also identifies signing infrastructure as the suspected compromise while noting that the root cause has not been published. Its earlier frozen estimate and valuation cutoff differ from Elliptic's; the graphic does not add these totals.
3. [FBI, North Korea Responsible for $6 Billion+ Binance Attack, October 31](https://www.fbi.gov/investigate/cyber/alerts/2026/north-korea-responsible-for-6-billion-binance-attack). Reports conversion principally into ETH and urges services to block linked transactions. This is official attribution and a disruption request, not proof that all conversion or cash-out attempts succeeded.
4. [Circle, USDC Terms](https://www.circle.com/legal/usdc-terms), especially Blocked Addresses & Forfeited Funds and Blocklisting. Documents Circle's ability to block USDC transfers to and from addresses on-chain. This is the issuer's stated control; it does not mean Circle can freeze arbitrary ETH in the same wallet. USDT-specific observations are supported by the investigators above, not by Circle's terms.

## Interpretation and asset details

The movement row is explicitly an analysis: following additional services and chains requires connecting more transaction records and coordinating more parties. This is an inference from reported movements and the FBI's disruption request, not a measured estimate of delay.

The distinction concerns issuer control, not the stablecoin's dollar peg. Changing an address alone leaves a token subject to its contract's issuer controls. A swap transfers one asset and delivers another; it does not erase the original token's history or prevent its issuer from acting on tokens elsewhere.

Borrowing is a collateral-backed loan, with debt and liquidation risk; it is not newly created profit or an additional independent theft total. The reported ETH loan left pledged USDT in the lending protocol. A protocol market pause is different from taking possession of the borrowed assets.

BTC was stolen directly and then divided among addresses. It is included as a native-coin comparison, not as a claim that the attacker converted all stolen funds into BTC. ETH's relevance here is supported by the observed swaps, lending access and the FBI's account. The graphic does not rank currencies or claim knowledge of the operators' complete motives.

Absence of a token-issuer freeze switch does not imply anonymity or immunity from recovery. Custodial restrictions, key seizures and, on some networks, emergency governance actions are separate mechanisms. A freeze or seizure also does not establish return to Binance or customers. The graphic does not establish completed cash-out.

## Alt text for X

RawPowered glass-style graphic titled Binance Breach: Why the Asset Choice Mattered. It contrasts USDT/USDC issuer blocklisting with native ETH/TRX/BTC, then explains swaps, collateral-backed borrowing and tracing across wallets, services and chains. Moving funds does not erase their history. A final panel explains that rapid swaps could lose value and that freezes and deposit screening still constrained the attacker. The graphic distinguishes post-theft recovery from the unresolved original breach. Snapshot October 31, 2026 CDT; numbered sources: Elliptic, TRM Labs, FBI and Circle.


## Visual provenance

The accompanying graphic is an AI-assisted editorial illustration reviewed against the cited material. It is separate from the source-page screenshots in the evidence archive.

[Return to the visual guide](../GALLERY.md).
