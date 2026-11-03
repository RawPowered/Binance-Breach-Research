# Sources

The dossier source IDs below preserve the October 31, 2026 research snapshot. Company statements, official attribution, investigator reconstructions and independent reporting have different roles. The [CSV register](research/source-register.csv) retains detailed claim locators and original access notes.

## November 2 evidence review

Update IDs identify source versions, not six independent confirmations. U01–U04 add four references; U05 and U06 revisit existing B05 and B07. The [dated addendum](updates/2026-11-02/README.md) and [update register](updates/2026-11-02/source-register.csv) record claims, section cutoffs and access limits. The original register below remains the October 31 record.

| Update ID | Reference / version | Role and limit |
|---|---|---|
| U01 | [Recovery Update #4: Withdrawals Resume in Phases](https://www.binance.com/en-GB/support/announcement/security-incident-recovery-update-4-withdrawals-resume-in-phases-2026-11-01-73911fb819b240f88b88256bdd318eda) — 2026-11-01; page heading 04:08, timezone not stated in heading | owner statement; Official page text read; its opening is prospective, not proof every withdrawal completed |
| U02 | [Recovery Update #5: October 31st PoR Snapshot Now Fully Verifiable](https://www.binance.com/en-GB/support/announcement/security-incident-recovery-update-5-october-31st-por-snapshot-now-fully-verifiable-by-users-as-zk-proof-generated-2026-11-02-185bd9a4717f44088b3be70287b8237f) — 2026-11-02; page heading 12:45, timezone not stated in heading | owner statement; Official text read via link from Update #4; direct access intermittent; verifier and reserve data not independently checked |
| U03 | [The Binance hack is laundering on autopilot](https://www.elliptic.co/insights/the-binance-hack-is-laundering-on-autopilot/) — 2026-10-31; key-point cutoff 08:11 UTC; later update 22:41 UTC | original investigator analysis; New to this bibliography, not a post-snapshot publication; section cutoffs differ; provider findings not replayed |
| U04 | [Binance incomplete RCA: signed delegation, unexplained access](https://www.maborak.com/blog/binance-incident-root-cause-evidence) — 2026-10-30; updated 2026-11-01 14:00 UTC | third party technical reproduction; Author-reported reproduction; not repeated here; historical state depends on one provider; no internal forensic access |
| U05 | [The largest theft in history: North Korea behind the Binance hack](https://www.elliptic.co/insights/binance-largest-hack-in-history/) — Last updated 2026-11-01 08:00 UTC; section cutoffs vary | original investigator analysis; Mutable page; distinguish header update, observation windows and retrieval date; no independent chain replay |
| U06 | [Binance hot-wallet investigation](https://bitquery.io/investigations/binance-hack) — 2026-11-02; holdings cutoff 13:26 UTC | original investigator analysis; Provider scope and labels differ from Elliptic; stronger laptop/key wording is not adopted as established fact |

Update #5 was read by following Update #4's official link after intermittent failures on direct retrieval. This source-access observation is not evidence of a correction or retraction. The proof announcement has not been independently cryptographically verified by this project.

## Attribution audit references

The [attribution audit](attribution/README.md) uses a local A-series key. Reused sources are mapped below; two references are added. Its registers distinguish source claims from checks performed by this project.

| Audit ID | Source | Existing key / access |
|---|---|---|
| A01 | [FBI attribution](https://www.fbi.gov/investigate/cyber/alerts/2026/north-korea-responsible-for-6-billion-binance-attack) | B03 |
| A02 | [Chainalysis investigation](https://www.chainalysis.com/blog/binance-exploit-latest-findings-and-response/) | B06 |
| A03 | [BitOK investigation](https://bitok.org/blog/binance-hack-bitok-investigation) | new attribution reference |
| A04 | [Elliptic Binance analysis](https://www.elliptic.co/insights/binance-largest-hack-in-history/) | B05 / U05 |
| A05 | [TRM investigation](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history) | B04 |
| A06 | [Elliptic Bitget assessment](https://www.elliptic.co/insights/bitget-attack-pushes-suspected-north-korea-crypto-heists-over-1-billion-in-2026/) | new attribution reference; indexed primary text |

A03 supplies a specific shared-recipient claim for future replay. A06 was read through indexed primary-publisher text; direct retrieval returned 404 during this review. Neither source changes a publisher claim into independently reproduced evidence. See the [verification plan](attribution/verification-plan.md).

## Dossier register

### B01 — Binance Announcement

[Security Incident Update Announcement #2](https://www.binance.com/en/square/post/382966352206379)

**Date/version:** 2026-10-30; signed 2026-10-31  
**Role:** Owner statement  
**Limits:** Full text read; heading and signature dates differ; not a final postmortem

### B02 — Binance Announcement

[Asset Replenishment Update: Approximately 90%](https://www.binance.com/en/square/post/383244329941551)

**Date/version:** 2026-10-31  
**Role:** Owner statement  
**Limits:** Full text read; future commitments not verified outcomes

### B03 — FBI

[North Korea Responsible for $6 Billion+ Binance Attack](https://www.fbi.gov/investigate/cyber/alerts/2026/north-korea-responsible-for-6-billion-binance-attack)

**Date/version:** 2026-10-31  
**Role:** Government attribution  
**Limits:** Full alert read; underlying intelligence not publicly reproduced

### B04 — TRM Labs

[North Korea Steals USD 6.36 Billion From Binance](https://www.trmlabs.com/resources/blog/north-korea-steals-usd-6-36-billion-from-binance-in-the-largest-hack-in-history)

**Date/version:** 2026-10-29; figures as of 2026-10-30 00:30 UTC  
**Role:** Original investigator analysis  
**Limits:** Full relevant sections read; early snapshot; estimates are not additive

### B05 — Elliptic / Tom Robinson

[The largest theft in history: North Korea behind the $6.4 billion Binance hack](https://www.elliptic.co/insights/binance-largest-hack-in-history/)

**Date/version:** 2026-10-30; updated 2026-10-31 23:55 UTC  
**Role:** Original investigator analysis  
**Limits:** Relevant full text read; value tables have different observation/price bases

### B06 — Chainalysis Team

[The $6.4 Billion Binance Hack: Tracing the North Korea Link](https://www.chainalysis.com/blog/binance-exploit-latest-findings-and-response/)

**Date/version:** 2026-10-30  
**Role:** Original investigator analysis  
**Limits:** Full text read; freeze cutoff contains literal [time] placeholder

### B07 — Bitquery / Gaurav Agarwal

[Binance hot-wallet investigation](https://www.bitquery.io/investigations/binance-hack)

**Date/version:** 2026-10-30; updated figures 2026-10-31 16:51 UTC  
**Role:** Original investigator analysis  
**Limits:** Relevant full text read; provider labels and valuation assumptions not independently recalculated

### B08 — Bitquery / Gaurav Agarwal

[The Binance hacker lost $119M to bad prices](https://www.bitquery.io/investigations/binance-hack-who-profited)

**Date/version:** 2026-10-30  
**Role:** Original investigator analysis  
**Limits:** Relevant full text read; benchmark-dependent estimates; not victim recovery

### B09 — Hacken / Dmytro Zap

[Binance $6.3B hack analysis: stolen key, hijacked signer or EIP-7702 delegation?](https://hacken.io/insights/binance-hack/)

**Date/version:** Date not displayed in inspected extract  
**Role:** Security analysis with transaction references  
**Limits:** Relevant full text read; cited explorer fetch blocked; no independent node replay

### B10 — Ethereum EIP authors

[EIP-7702: Set Code for EOAs](https://eips.ethereum.org/EIPS/eip-7702)

**Date/version:** Created 2024-05-07; current Final specification  
**Role:** Protocol specification  
**Limits:** Specification read; explains mechanism rather than incident attribution

### B11 — Binance Japan

[Response to the Security Incident at Binance Global](https://www.binance.com/en/square/post/382812261202623)

**Date/version:** 2026-10-30  
**Role:** Owner regional statement  
**Limits:** Indexed full statement inspected; current resumption not independently verified

### B12 — Reuters via Euronext

[Binance says it has covered 90% of losses from $6.3 billion hack](https://live.euronext.com/en/financial-news/binance-says-it-has-covered-90-losses-63-billion-hack)

**Date/version:** 2026-10-31; page display 23:11 zone unspecified  
**Role:** Independent reporting  
**Limits:** Relevant article read; reporting is not a reserves audit

### B13 — CoinDesk / Olivier Acuna

[Experts divided over Binance hack asset freezes, warn recovery is another matter](https://www.coindesk.com/business/2026/10/30/experts-divided-over-binance-hack-asset-freezes-warn-recovery-is-another-matter)

**Date/version:** 2026-10-30 15:55 EDT  
**Role:** Independent reporting and expert interviews  
**Limits:** Relevant full text read; jurisdiction-dependent legal commentary

### B14 — Associated Press

[Binance flags potential security issue](https://apnews.com/article/39cda8ceb8095e036334a18549d3d20d)

**Date/version:** 2026-10-29 23:28:49 UTC  
**Role:** Independent early reporting  
**Limits:** Search-returned article text inspected; developing preliminary account

### B15 — Binance Announcement

[Security Incident Update (initial)](https://www.binance.com/en/square/post/382967851743776)

**Date/version:** 2026-10-30  
**Role:** Owner statement; limited access  
**Limits:** Indexed statement inspected; direct page returned only shell; use B01 for current account

### B16 — Chainalysis Team

[Chainalysis Security Incident Information](https://www.chainalysis.com/blog/security-incident-october-30/)

**Date/version:** 2026-10-30  
**Role:** Owner statement  
**Limits:** Full statement inspected in same research session; does not prove shared actors

## Supplementary visual references

- [Circle USDC terms](https://www.circle.com/legal/usdc-terms): blocklisting powers cited in the asset-choice graphic.
- [Binance official newsroom](https://www.binance.com/en-GB/press) and its linked [Binance Style Guide](https://design.binance.vision/882e92a34/p/001e0b-binance-style-guide): official emblem reference used for the cover, not evidence of the breach.

## Publication-day access note

On November 2, the FBI alert remained readable in a targeted check. The two archived Binance Square statement links returned page shells in the same check; an alternate support link redirected to an announcement index. Original links and original access dates are preserved. A changed or unavailable page does not by itself establish a correction or retraction. The dated source screenshots and source-specific limits remain part of the record. This was a targeted availability check, not a complete update of incident status.

A subsequent November 2 review retrieved the newer support notices and revised investigator pages recorded above. The earlier access note remains a record of that narrower check.

[Overview](README.md) · [November 2 update](updates/2026-11-02/README.md) · [Dossier](research/DOSSIER.md)


## November 3, 2026 — focused macOS/Homebrew assessment

The [technical assessment](updates/2026-11-03/MACOS-HOMEBREW-ASSESSMENT.md) and [evidence register](updates/2026-11-03/macos-evidence-register.csv) provide separate claim statuses and bounded defensive guidance. Additional authoritative references: [Homebrew homepage](https://brew.sh/), [official installer repository](https://github.com/Homebrew/install), and [Homebrew security policy](https://github.com/Homebrew/brew/security). The [Binance X announcement](https://x.com/binance/status/2117626126214504729) is listed as a publication pointer, not an independent source. No verified connection between the SANS MacSync campaign and Binance's June endpoint is claimed.

## November 3, 2026 — Homebrew and internal intrusion update

The [dated addendum](updates/2026-11-03/README.md#source-register) records 13 sources with publication dates, access limits and evidence roles. Its source IDs S1–S13 are local to that addendum and do not replace earlier B/U identifiers.

- [Binance preliminary report, November 3](https://www.binance.com/es/blog/community/3229153443759566763): internal chronology and disclosed endpoint file operations; substantial indexed text inspected, direct page access failed.
- [SANS fake Homebrew/MacSync analysis, May 1](https://isc.sans.edu/diary/Malicious%20Ad%20for%20Homebrew%20Leads%20to%20MacSync%20Stealer/32942): original analysis of a separate campaign. Its domains and hashes are not established Binance indicators.
- [TRM laundering update, November 3](https://www.trmlabs.com/resources/blog/binance-hack-update-north-korea-launders-proceeds-through-self-minted-tokens-and-chained-bridges): follow-up tracing; stale FAQ attribution wording is flagged in the addendum.
- [SafeDep attack-path analysis, November 3](https://safedep.io/blog/binance-hack-developer-supply-chain-attack-path): incident narrative derives from Binance; campaign comparison is analyst interpretation.

The FBI and original blockchain investigations remain distinct evidence for official attribution and fund movements. No independent endpoint examination or transaction replay is claimed.
