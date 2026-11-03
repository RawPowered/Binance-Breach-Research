# Binance cybersecurity research update

Prepared November 3, 2026. Public evidence concerning the fake macOS Homebrew installation and subsequent wallet theft. All precise times below are UTC.

For a focused, evidence-led technical evaluation, see the [macOS/Homebrew malware assessment](MACOS-HOMEBREW-ASSESSMENT.md) and [14-row evidence register](macos-evidence-register.csv). These explain why June's fake installer and September's `pyenv` replacement must not be merged, provide official Homebrew source references, and identify safe, read-only triage options.

This dated addendum extends the [October 31 dossier](../../research/DOSSIER.md) and [November 2 evidence update](../2026-11-02/README.md). Earlier snapshots retain their original contents. Coverage is of public sources located during this review; confidential forensic evidence is outside its scope.

## Evidence assessment

The research needs two distinct evidence tracks: the internal intrusion account and the externally observable theft. An official company account establishes what Binance says happened, while attribution notices and blockchain analysis address different questions. Repetition of the company account in news stories does not independently validate laptop forensics.

**Binance's preliminary account, published November 3:**

| Date | Reported event |
|---|---|
| June 2026 | Engineer A, Wallet DevOps, downloaded a tampered Homebrew installer while seeking an AI coding tool. Binance replaced the device and rotated credentials; team information was exposed. |
| September 2026 | Engineer B received a fake interview assignment; repository setup executed malware on the work computer. |
| October 20 | An internal AI tool enabled access from B to A and C; attackers found A's container deployment token. |
| October 29, 17:15–19:56 | Attackers used C's computer and A's credentials to deploy a container and launch the attack. |
| October 29, 23:56 | Final unauthorized transfer: 2,961.9 ETH. |
| October 30, 00:10 | Binance14's EIP-7702 delegation was cleared. |

The disclosed endpoint sequence stages `/opt/homebrew/Cellar/pyenv/2.8.0/libexec/pyenv_`, replaces `pyenv` (3,344 → 3,414 bytes), changes `/opt/homebrew/bin/pyenv`, and starts `zsh`. This belongs to B's September compromise. Binance reports $6.34 billion affected and $2.85 billion frozen/intercepted, with independent review pending. [Binance preliminary report](https://www.binance.com/es/blog/community/3229153443759566763).

## Corroborating chronology

| Date/time | External evidence and its limits |
|---|---|
| April 30; published May 1 | Brad Duncan documents a separate fake Homebrew advertisement distributing MacSync Stealer. Useful precedent; no established victim-specific link to Binance. [SANS diary](https://isc.sans.edu/diary/Malicious%20Ad%20for%20Homebrew%20Leads%20to%20MacSync%20Stealer/32942). |
| October 28–29 | TRM traces small Tornado Cash funding withdrawals and attack rehearsals before the theft. [TRM initial investigation](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history). |
| October 29, 20:05–20:09 | TRM observes 233.46 million XRP leaving five wallets; later transfers span multiple chains. [TRM](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history). |
| October 29, 20:20 | TRM identifies one Ethereum transaction carrying 50 signed authorizations; 3 minutes 24 seconds later, a sweep moves 167,464 ETH and 63 tokens. [TRM](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history). |
| October 29, 21:01 / 21:04 | TRM records Tether and Circle freezes. It also records another theft wave around 23:05. [TRM](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history). |
| October 30 | Chainalysis publishes its TraderTraitor assessment, citing commingling with proceeds of a previously attributed Bitget theft. [Chainalysis investigation](https://www.chainalysis.com/blog/binance-exploit-latest-findings-and-response/). |
| October 30 | Elliptic publishes a downloadable address blocklist. This supplies screening evidence, rather than endpoint evidence. [Elliptic blocklist announcement](https://www.elliptic.co/insights/free-binance-exploit-blocklist-available-from-elliptic-for-the-crypto-community-to-screen-against-the-attributed-addresses-now/). |
| October 31 | FBI publicly attributes the theft to North Korea's TraderTraitor activity and publishes associated Ethereum addresses. It does not describe a Homebrew infection chain. [FBI notice](https://www.fbi.gov/investigate/cyber/alerts/2026/north-korea-responsible-for-6-billion-binance-attack). |
| October 31–November 2; published November 3 | TRM tracks laundering through self-minted tokens, lending receipt tokens, and chained cross-chain swaps. These observations concern proceeds, not the original malware. [TRM follow-up](https://www.trmlabs.com/resources/blog/binance-hack-update-north-korea-launders-proceeds-through-self-minted-tokens-and-chained-bridges). |

## Evidence inventory and confidence

| Evidence | What it supports | What it does not establish |
|---|---|---|
| Binance's incident narrative and file-operation sequence | First-party account of internal events | Independent reproduction of the compromise or complete forensic provenance |
| FBI attribution and address list | Official attribution and leads for transaction screening | Public disclosure of the evidence underlying attribution; identity of the installer |
| TRM cross-chain signature analysis | Investigator assessment that wallet signing infrastructure was abused | Which workstation action produced each signature |
| Chainalysis commingling observation | An on-chain connection informing actor attribution | Proof that the earlier and later intrusions used identical malware |
| Elliptic transaction analysis and blocklist | Transfer accounting and attributed-address screening | A static, exhaustive list of every future laundering destination |
| SANS fake Homebrew sample analysis | Independently documented impersonation technique and sample indicators | Identification of Binance's June sample as MacSync |

For an example of the FBI's published address evidence, its notice lists `0x8532FA14ACAf483729C449b8458aedDb900543D4`. Preserve the notice's wording about associated addresses; an address label alone does not identify a human operator. [FBI notice](https://www.fbi.gov/investigate/cyber/alerts/2026/north-korea-responsible-for-6-billion-binance-attack).

## Fake Homebrew indicators: contextual evidence only

SANS reports a counterfeit page at `hxxps[:]//sites.google[.]com/view/brewpage`, a C2 domain `glowmedaesthetics[.]com`, and temporary collection archive `/tmp/osalogging.zip`. Its published SHA-256 indicators are:

| Role | SHA-256 |
|---|---|
| Copy/paste script | `a4fcfecc5ac8fa57614b23928a0e9b7aa4f4a3b2b3a8c1772487b46277125571` |
| Initial download | `0d58616c750fc8530a7e90eee18398ddedd08cc0f4908c863ab650673b9819dd` |
| Decoded shell script | `86d0c50cab4f394c58976c44d6d7b67a7dfbbb813fbcf622236e183d94fd944f` |

Source: [Brad Duncan, SANS ISC, May 1](https://isc.sans.edu/diary/Malicious%20Ad%20for%20Homebrew%20Leads%20to%20MacSync%20Stealer/32942). These are indicators for that documented campaign, **not confirmed Binance indicators**. No malware was downloaded or executed during this research.

## Interpretation and unresolved questions

These are research conclusions and questions, not additional forensic findings:

- A search-distributed impersonation installer does not by itself establish compromise of Homebrew's official repositories, release process, or infrastructure. Retain that distinction when using the phrase “supply chain attack.”
- Do not merge the June installer event with September's developer-tool replacement. Request a separate sample, hash, execution chain, and date for each event.
- Establish the June download URL, search result or advertisement, payload hash, malware family, C2 infrastructure, and exact installation date before assigning specific fake-Homebrew campaign indicators to Binance.
- Request evidence showing how the internal AI tool crossed device boundaries: tool identity, access model, relevant logs, execution permissions, and affected versions. Prompt injection, a product vulnerability, and credential abuse are different hypotheses.
- Require a CVE, vendor advisory, or demonstrated vulnerability before describing undetected malware as a confirmed software zero-day exploit. Failure to detect a payload alone does not prove exploitation of an unknown vulnerability.
- A deployment token's scope, lifetime, storage, and authorization path to signing require investigation. Ask whether signature requests enforced policy independently of container identity.
- Validate independent-review findings when published. Treat remediation effectiveness as a separate question from whether a remediation action was announced.

SafeDep's article explicitly says its incident facts come from Binance; its comparison with Contagious Interview is an analyst assessment, rather than separate confirmation of that campaign identity. [SafeDep analysis, November 3](https://safedep.io/blog/binance-hack-developer-supply-chain-attack-path).

## Discrepancies to retain in the research

| Issue | How to record it |
|---|---|
| Loss estimates | TRM reports $6.36B and Elliptic $6.43B. Preserve each source's valuation and scope rather than silently choosing one. [TRM](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history), [Elliptic](https://www.elliptic.co/insights/binance-largest-hack-in-history/). |
| Chain count | TRM's initial accounting covers ten chains; Elliptic covers eleven. A reconciled transfer ledger is needed to resolve scope. [TRM](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history), [Elliptic](https://www.elliptic.co/insights/binance-largest-hack-in-history/). |
| Start time | Chainalysis gives approximately 4:20 p.m. Eastern, equivalent to 20:20 UTC on October 29; TRM gives 20:05 UTC for XRP. Possible explanation: different chain/event scope; this remains an inference. [Chainalysis](https://www.chainalysis.com/blog/binance-exploit-latest-findings-and-response/), [TRM](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history). |
| 50 authorizations | Preserve TRM's distinction between one outer transaction and 50 authorizations. The protocol supports an authorization list within a transaction. [TRM](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history), [EIP-7702 specification](https://eips.ethereum.org/EIPS/eip-7702). |
| Frozen versus recovered | Elliptic reports verified freezes/seizures; a freeze does not by itself establish restitution to Binance or customers. Its reported total is $2.85B. [Elliptic](https://www.elliptic.co/insights/binance-largest-hack-in-history/). |
| Stale source text | TRM's November 3 follow-up retains FAQ language saying no government has attributed the theft. This conflicts with the dated October 31 FBI notice; use the FBI notice for official attribution. [TRM follow-up](https://www.trmlabs.com/resources/blog/binance-hack-update-north-korea-launders-proceeds-through-self-minted-tokens-and-chained-bridges), [FBI](https://www.fbi.gov/investigate/cyber/alerts/2026/north-korea-responsible-for-6-billion-binance-attack). |

## Source register

All sources were checked November 3, 2026. Dates describe publication unless otherwise specified. Live articles and address lists may change.

| ID | Source/date | Role and access notes |
|---|---|---|
| S1 | [Binance initial findings](https://www.binance.com/es/blog/community/3229153443759566763), Nov 3 | Core first-party internal chronology. Substantial indexed text was available; direct page opening failed. The locale path returned English report text in search. |
| S2 | [FBI attribution](https://www.fbi.gov/investigate/cyber/alerts/2026/north-korea-responsible-for-6-billion-binance-attack), Oct 31 | Government attribution and address evidence; page opened. |
| S3 | [TRM initial investigation](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history), Oct 29 | Original cross-chain analysis; page opened. |
| S4 | [Chainalysis theft investigation](https://www.chainalysis.com/blog/binance-exploit-latest-findings-and-response/), Oct 30 | Original tracing and attribution rationale; substantial indexed text available. |
| S5 | [Elliptic main analysis](https://www.elliptic.co/insights/binance-largest-hack-in-history/), Oct 30, updated Nov 1 | Original accounting and transfer analysis; page opened. |
| S6 | [Elliptic blocklist announcement](https://www.elliptic.co/insights/free-binance-exploit-blocklist-available-from-elliptic-for-the-crypto-community-to-screen-against-the-attributed-addresses-now/), Oct 30 | Public address dataset entry point; indexed announcement checked, underlying CSV not downloaded. |
| S7 | [TRM laundering follow-up](https://www.trmlabs.com/resources/blog/binance-hack-update-north-korea-launders-proceeds-through-self-minted-tokens-and-chained-bridges), Nov 3 | Original follow-up tracing; indexed text checked; contains stale FAQ language. |
| S8 | [SANS MacSync/Homebrew diary](https://isc.sans.edu/diary/Malicious%20Ad%20for%20Homebrew%20Leads%20to%20MacSync%20Stealer/32942), May 1 | Original malware analysis of a separate observed campaign; page opened. |
| S9 | [EIP-7702](https://eips.ethereum.org/EIPS/eip-7702), specification | Primary protocol reference; page opened. |
| S10 | [SafeDep developer attack-path analysis](https://safedep.io/blog/binance-hack-developer-supply-chain-attack-path), Nov 3 | Secondary incident account with original interpretation; indexed text checked, direct opening failed. |
| S11 | [The Block report](https://www.theblock.co/news/business/2026-11-03-binance-hack-incident-report-north-korea-fake-job-interview-ai-tool-432406), Nov 3 | News coverage, useful for publication chronology; indexed text checked. No independent endpoint evidence identified. |
| S12 | [The Hacker News coverage](https://thehackernews.com/2026/11/binance-reveals-how-fake-job-interviews.html), Nov 3 | Discovery/corroborating coverage; indexed excerpt only, direct opening failed. Headline uses $6.43B. |
| S13 | [WIRED coverage](https://www.wired.com/story/binance-says-hackers-used-well-known-tricks-to-carry-out-a-dollar634-billion-heist/), Nov 3 | Additional reporting located; excerpt only, not relied on for technical reconstruction. |

No complete endpoint log set, installer sample tied to Engineer A, interview repository tied to Engineer B, or independently published internal forensic report was located in the sources reviewed. This document is a sourced public-evidence synthesis, not a forensic examination of Binance systems.

[Overview](../../README.md) · [Sources](../../SOURCES.md) · [Research changes](../../CHANGELOG.md)
