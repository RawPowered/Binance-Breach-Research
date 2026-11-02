# Binance breach — how the attack unfolded

Research snapshot: October 31, 2026 CDT. Web sources checked November 1 at approximately 02:36 UTC (October 31, 21:36 CDT). This graphic continues the RawPowered Cyber Security Research X series.

## Numbered citations

1. [Binance, Security Incident Update #2](https://www.binance.com/en/square/post/382966352206379). The company says investigators identified additional compromise points beyond the initially suspected laptop and had not established the full attack sequence. It reported no evidence of wallet private-key compromise at that stage. The graphic therefore marks initial access as unresolved.
2. [TRM Labs, North Korea Steals USD 6.36 Billion From Binance](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history). Primary investigator analysis covering ten chains, most outflows in roughly twenty minutes, Ethereum delegation, ordinary transfers elsewhere, repeat sweeps and use of swaps and lending. Compromise of hot-wallet signing infrastructure is TRM's assessment, not a confirmed internal root cause.
3. [Hacken, Binance hack analysis](https://hacken.io/insights/binance-hack/). Documents Ethereum delegation to sweeper code, subsequent sweeps and eventual delegation reset, with links to transactions. This graphic relies on published reconstruction and does not claim an independent transaction replay. Several Hacken conclusions also cite TRM and Elliptic, so they are not independent corroboration of every point.
4. [Elliptic, Binance theft analysis](https://www.elliptic.co/insights/binance-largest-hack-in-history/). October 31 update covers eleven affected chains, swaps from stablecoins into native assets, borrowing ETH against USDT collateral and cross-chain movements. Together with TRM's ten-chain scope, this supports the rounded label “10+ chains.” The twenty-minute wording is TRM's estimate for most outflows; later activity continued.

Supporting protocol reference: [EIP-7702: Set Code for EOAs](https://eips.ethereum.org/EIPS/eip-7702). Delegation permits an account to execute designated code and persists until changed. The existence of this mechanism does not establish an underlying Ethereum protocol vulnerability in this incident.

## Reading the diagram

This is a conceptual reconstruction, not an exact timestamp chart. Transfers, conversions and containment overlapped. Amber indicates unresolved entry and an investigator assessment; green stages summarize published transaction analysis. “Two withdrawal paths” groups different observed methods: Ethereum also had ordinary transfers from another hot wallet, so delegation was not the only Ethereum path. “What stood out” identifies distinctive features of this case, not first-ever or historically unique techniques. The graphic makes no claim that keys were definitely extracted or that AI caused the incident.

## Alt text for X

RawPowered graphic: Binance Breach — How the Attack Unfolded. Reported reconstruction, October 29–30, 2026 UTC; snapshot October 31 CDT. Four stages: unresolved entry with multiple compromise points; TRM's assessment of compromised hot-wallet signing infrastructure; two withdrawal paths, with Ethereum delegation to attacker-controlled sweeper code and ordinary signed transfers on other chains; then swaps, borrowing and cross-chain movements. Distinctive features: coordinated activity across ten or more chains with most funds moved in roughly twenty minutes, repeat sweeps of later Ethereum deposits, and stablecoins exchanged or pledged to obtain native crypto during a race against freezes. Takeaway: valid signatures can authorize malicious actions. Sources: Binance, TRM, Hacken and Elliptic.


## Visual provenance

The accompanying graphic is an AI-assisted editorial illustration reviewed against the cited material. It is separate from the source-page screenshots in the evidence archive.

[Return to the visual guide](../GALLERY.md).
