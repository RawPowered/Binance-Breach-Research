# Binance breach — reported multiple compromise points

Research snapshot: October 31, 2026 CDT. A cited evidence map, not a verified internal architecture or a count of separate intrusion routes.

## Numbered sources

1. [Binance, Security Incident Update #2](https://www.binance.com/en/square/post/382966352206379). The company expands its initial laptop hypothesis to additional compromise points without naming the systems. It reports no evidence of compromised private keys at that stage and says the full attack sequence is still under investigation.
2. [TRM Labs, Binance investigation](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history). Investigators interpret valid transfers across chains as evidence consistent with compromise of hot-wallet signing infrastructure. The published reconstruction describes Ethereum delegation and repeated sweeps as well as ordinary transfers from other wallets. This remains an investigator assessment of the signing failure; internal root cause is not established.
3. [Elliptic, Binance investigation, October 31 update](https://www.elliptic.co/insights/binance-largest-hack-in-history/). Preserves the initial DevOps laptop/service-container account, later expanded company statements and the observed Ethereum delegation. Its article makes clear that the additional breach points were not identified in the reviewed public account.

## How to read the graphic

The two top cards are evidence categories, not a declaration of exactly two entry points. Stacked question-mark nodes do not represent a measured number of compromised machines. The initial lead is provisional. Dashed connectors indicate undisclosed relationships; they do not establish lateral movement, a credential path or a proven endpoint-to-signer sequence.

On-chain effects demonstrate wallet actions, not which internal endpoints were compromised. Ethereum also had ordinary transfers from a different wallet; delegation was one observed method, not the only Ethereum action. The private-key strip records the company's qualified statement, not proof of no key exposure. The layout's vertical order is explanatory rather than a timestamped sequence.

## Alt text for X

Dark glass RawPowered graphic titled Binance Breach: Reported Multiple Compromise Points. The initial provisional laptop and service-container lead sits beside additional points that Binance reported but did not identify. Dashed amber lines connect them to an undisclosed internal path and TRM's suspected hot-wallet signing compromise. Separate green panels show reported Ethereum delegation with repeat withdrawals and ordinary signed transfers from other wallets and chains. A qualification notes Binance found no evidence of private-key compromise while investigating. The takeaway states that wallet outflows do not identify every entry point. Snapshot October 31, 2026 CDT. Sources: Binance, TRM and Elliptic. Research stamp at lower right.


## Visual provenance

The accompanying graphic is an AI-assisted editorial illustration reviewed against the cited material. It is separate from the source-page screenshots in the evidence archive.

[Return to the visual guide](../GALLERY.md).
