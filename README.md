# Binance Breach Research

![Binance breach: cybersecurity, cryptocurrency and consequences. RawPowered independent research.](assets/social/cover.png)

**Independent research by RawPowered on the October 29, 2026 Binance hot-wallet theft and its attribution to North Korea's TraderTraitor activity.**

**Original snapshot: October 31, 2026. Latest evidence review: November 4, 2026 (America/Chicago).** The [financial accounting assessment](research/FINANCIAL-ACCOUNTING.md) separates theft, freezes, company replenishment and attacker holdings. The [November 3 update](updates/2026-11-03/README.md) documents the reported intrusion. Earlier snapshots and graphics are preserved.

**Latest reported developments:** Binance's preliminary report describes a June tampered Homebrew installer, September fake interview assignment, October internal AI-tool pivot and access to wallet signing operations. The internal sequence remains a company-reported account pending independent review. [Timeline, sources and evidence limits](updates/2026-11-03/README.md).

Binance reported roughly $6.3B in losses. The FBI's October 31 alert attributed the theft to North Korea's TraderTraitor activity. Binance has now published a preliminary internal intrusion account; this project has not independently verified its endpoint forensics. [Company statement](https://www.binance.com/en/square/post/382966352206379) · [FBI attribution](https://www.fbi.gov/investigate/cyber/alerts/2026/north-korea-responsible-for-6-billion-binance-attack)

## How much was stolen, replaced and remains outstanding?

**As of the November 4 review, public evidence does not establish exact reconciled totals.** These measures overlap and must not be added together.

| Measure | Best supported figure | What it means |
|---|---|---|
| Compromised exposure | Full reachable amount **unknown** | Stolen value does not measure the full permissions exposure. |
| Gross stolen / reported impact | **Approximately $6.34B** company baseline | Investigator estimates span $6.30B–$6.43B; scopes differ. [Company report](https://www.binance.bh/en/blog/community/3229153443759566763) |
| Frozen / intercepted | **Approximately $2.85B**, reported Nov 3 | Not automatically returned to Binance. [Company report](https://www.binance.bh/en/blog/community/3229153443759566763) |
| Replaced by company | **98% replenished**; more than 100% funding reserved | Company claim, not an audited payment ledger. [Recovery Update #7](https://www.binance.com/en/square/post/384674399709556) |
| Dollar equivalent of replacement | **About $6.21B**, conditional calculation | 98% × $6.34B; **not an exact amount paid**. [Assumptions](research/FINANCIAL-ACCOUNTING.md#replacement-funding-the-dollar-calculation-is-conditional) |
| Still in attacker-linked holdings | **About $3.1B** at 09:56 UTC Nov 4 | Bitquery estimate, mostly idle BTC/ETH; not all actively circulating. [Investigation](https://www.bitquery.io/investigations/binance-hack) |
| Original stolen funds actually returned / exact cash-out | **Not established** | Freezes, replacement and return receipts are different evidence. |

The **$3.49B** subtraction ($6.34B − $2.85B) is an unreconciled residual, not a live holdings estimate. Company replenishment does not reduce the attacker's stolen-funds balance. [Full assessment, source cutoffs and limitations](research/FINANCIAL-ACCOUNTING.md).

## Start with the evidence

| Read | What it contains |
|---|---|
| [Financial accounting assessment](research/FINANCIAL-ACCOUNTING.md) | Stolen, frozen, replaced and attacker-retained amounts, calculation limits and source cutoffs |
| [macOS/Homebrew malware assessment](updates/2026-11-03/MACOS-HOMEBREW-ASSESSMENT.md) | June vs. September infection analysis, defensive triage, official Homebrew references and [machine-readable evidence register](updates/2026-11-03/macos-evidence-register.csv) |
| [November 3 Homebrew and intrusion update](updates/2026-11-03/README.md) | Dated attack chronology, disclosed endpoint artifacts, 13 sources and verification gaps |
| [November 2 evidence update](updates/2026-11-02/README.md) | New citations, revised tracing, operational milestones and claim follow-up |
| [North Korea attribution audit](attribution/README.md) | Published evidence, source dependencies, alternative explanations and verification gaps |
| [Full research dossier](research/DOSSIER.md) | Attack mechanics, attribution, financial accounting, response and open questions |
| [Four-graphic guide](GALLERY.md) | The cover, reported compromise points, attack sequence and asset-choice explanation, with captions and citations |
| [Annotated source evidence](research/VISUAL-EVIDENCE.md) | Three source-page screenshots and three original data/concept graphics |
| [Sources](SOURCES.md) | Original and follow-up citations, attribution references, source roles and access limits |
| [Claim audit](research/claim-audit.csv) | Thirteen claims with status boundaries |

## North Korea attribution: evidence and uncertainty

**The FBI officially attributes the theft to North Korea's TraderTraitor activity.** [Read the official notice](https://www.fbi.gov/investigate/cyber/alerts/2026/north-korea-responsible-for-6-billion-binance-attack). Our [attribution audit](attribution/README.md) examines the supporting financial links, source independence and the evidence needed to connect wallets, operators and state affiliation.

| What is established in this study | Verification boundary |
|---|---|
| The official attribution is published | The complete underlying intelligence is not public in the FBI alert |
| Investigators report Binance–Bitget financial links | This project has not independently replayed those flows or established the operators' identities |

Read the [evidence and uncertainty assessment](attribution/README.md), explore the [source-dependency map](attribution/source-dependencies.csv), or review the [alternative-explanation checks](attribution/alternative-explanations.csv). The audit identifies both support and possible failure points; it does not claim conclusive independent proof or assign unsupported percentages.

## The visual exploration

Select a preview for the full-resolution graphic. The [visual guide](GALLERY.md) provides readable full-width versions and the source keys used on each image.

| Reported compromise points | How the attack unfolded | Why asset choice mattered |
|---|---|---|
| [![Evidence map distinguishing the initial laptop lead, undisclosed points, analyst assessment and wallet effects](assets/social/compromise-points.png)](assets/social/compromise-points.png) | [![Reported attack reconstruction with Ethereum delegation and ordinary transfers on other chains](assets/social/attack-mechanics.png)](assets/social/attack-mechanics.png) | [![Issuer-controlled tokens versus native coins, swaps, borrowing and tracing](assets/social/asset-choice.png)](assets/social/asset-choice.png) |
| [Sources and alt text](visuals/compromise-points.md) | [Sources and alt text](visuals/attack-mechanics.md) | [Sources and alt text](visuals/asset-choice.md) |

## What the case distinguishes

- **Company reports, investigator assessments and observed wallet actions.** The November 3 company report supplies an internal intrusion account; wallet outflows independently establish a different part of the evidence. The earlier graphics preserve their original evidence cutoff.
- **Theft, frozen assets, returned assets and replacement funding.** These are different accounting questions. Source estimates overlap and have different cutoffs.
- **Issuer-controlled tokens and native coins.** Converting or borrowing changed which asset the attacker held and which controls applied; transaction history remained available for investigation.
- **Automation and AI attribution.** Automation alone does not establish AI use. The November 3 report describes abuse of an internal AI tool; its precise mechanism remains undisclosed. This does not establish attacker use of AI to automate laundering.

The supporting analysis and citations are in the [dossier](research/DOSSIER.md). The graphics summarize the October 31 record and do not add new forensic findings; consult the dated updates for later disclosures.

## Structured research

| Dataset | Archived observations |
|---|---:|
| [Timeline](research/timeline.csv) | 18 dated events, observations and targets |
| [Financial estimates](research/financial-estimates.csv) | 15 separately scoped observations |
| [Claim audit](research/claim-audit.csv) | 13 claim assessments |
| [Source register](research/source-register.csv) | 16 resources |

Future commitments in the original timeline remain targets in that snapshot. Later observations and milestone reports are recorded separately in the [update datasets](updates/2026-11-02/README.md#read-the-update-data).

## Scope and provenance

This compilation uses public owner statements, official attribution, published blockchain investigations, protocol documentation and selected reporting. It does not include internal incident logs or claim an independent chain replay, reserve audit or forensic attribution.

Authentic source-page captures and original data charts are labeled in the [evidence archive](research/VISUAL-EVIDENCE.md). The four glass-series graphics are AI-assisted editorial illustrations, separately documented in the [visual guide](GALLERY.md). Their appearance is not evidence of incident facts.

Read the [publication record](PUBLICATION.md) for preservation and source-access notes, the [reuse and attribution notes](RIGHTS.md) for third-party material, or the [plain-text citations](CITATIONS.txt) for sharing.

<p align="right"><img src="assets/brand/research-stamp.png" alt="RawPowered Cyber Security Research" width="340"></p>
