# Evidence update — November 2, 2026

**Research checked:** November 2, 2026, approximately 17:52 UTC / 11:52 CST (America/Chicago). This targeted addendum extends the [October 31 dossier](../../research/DOSSIER.md). It records publisher claims and research findings without changing that snapshot.

## What changed

| Topic | New evidence and its boundary |
|---|---|
| Replenishment | Binance reports 95% coverage, up from the snapshot's 90%; this is replacement funding, not assets returned by attackers. [U01](https://www.binance.com/en-GB/support/announcement/security-incident-recovery-update-4-withdrawals-resume-in-phases-2026-11-01-73911fb819b240f88b88256bdd318eda) |
| Withdrawals | Update #4 sets a phased restart window on November 1; Elliptic subsequently records reopening beginning with Bitcoin. This does not establish availability of every asset/network pair. [U01](https://www.binance.com/en-GB/support/announcement/security-incident-recovery-update-4-withdrawals-resume-in-phases-2026-11-01-73911fb819b240f88b88256bdd318eda) · [U05](https://www.elliptic.co/insights/binance-largest-hack-in-history/) |
| Reserve proof | Binance says the proof for its October 31 snapshot is complete for ten named tokens. This research did not run the verifier or independently audit reserves. [U02](https://www.binance.com/en-GB/support/announcement/security-incident-recovery-update-5-october-31st-por-snapshot-now-fully-verifiable-by-users-as-zk-proof-generated-2026-11-02-185bd9a4717f44088b3be70287b8237f) |
| Tracing | Bitquery reports approximately $3.0B retained and 539,862 ETH at its November 2 cutoff. These are provider-scoped observations, not a reconciled total. [U06](https://bitquery.io/investigations/binance-hack) |

## New citations

- **[U01 — Binance Update #4, November 1](https://www.binance.com/en-GB/support/announcement/security-incident-recovery-update-4-withdrawals-resume-in-phases-2026-11-01-73911fb819b240f88b88256bdd318eda):** advances operational and funding disclosures. A phase-one plan and a later reported start are separate observations.
- **[U02 — Binance Update #5, November 2](https://www.binance.com/en-GB/support/announcement/security-incident-recovery-update-5-october-31st-por-snapshot-now-fully-verifiable-by-users-as-zk-proof-generated-2026-11-02-185bd9a4717f44088b3be70287b8237f):** changes proof generation from a target to a company-reported completed milestone. The next withdrawal phase and expanded snapshot remain plans, not completed outcomes.
- **[U03 — Elliptic, laundering on autopilot](https://www.elliptic.co/insights/the-binance-hack-is-laundering-on-autopilot/):** adds measurements of around-the-clock activity and repeated transfer behavior. Published October 31; newly added to the bibliography rather than newly published today.
- **[U04 — Maborak technical reconstruction, updated November 1](https://www.maborak.com/blog/binance-incident-root-cause-evidence):** reports read-only queries and offline signature checks. These corroborate execution mechanics at the author's stated level of verification, not how access was obtained. We have not reproduced those checks.

## Revised versions of existing sources

**[U05 / original B05 — Elliptic](https://www.elliptic.co/insights/binance-largest-hack-in-history/):** its November 1 version extends the Tron observation window to 05:33 UTC and reports 1,113 transfers. It describes failed bridge attempts as more consistent with repeated script retries than learning. On-chain patterns still do not establish AI involvement.

**[U06 / original B07 — Bitquery](https://bitquery.io/investigations/binance-hack):** the updated cutoff is November 2 at 13:26 UTC. Its scope remains nine chains. Different scopes, asset prices and address labels prevent simple subtraction or aggregation with other providers. Its categorical laptop/key wording is not treated as a final internal forensic finding.

## Interpretation and limits

The claim that a signing service was compromised remains an assessment. Maborak explains that valid recovered signatures do not distinguish signer misuse from key extraction. The initial laptop-to-container account and the wallet execution trace still lack a publicly established connecting path. [U04](https://www.maborak.com/blog/binance-incident-root-cause-evidence)

No final Binance technical postmortem was located in this targeted review. Update #4 still promises a later report. Additional internal compromise points remain unnamed in the reviewed sources. [U01](https://www.binance.com/en-GB/support/announcement/security-incident-recovery-update-4-withdrawals-resume-in-phases-2026-11-01-73911fb819b240f88b88256bdd318eda) · [U04](https://www.maborak.com/blog/binance-incident-root-cause-evidence)

Proof availability is distinct from this project's independent verification and from a comprehensive balance-sheet audit. Likewise, issuer freezes, native-asset holdings and replacement purchases remain different categories. Future dates in the new [timeline](timeline.csv) are explicitly labeled targets.

## Read the update data

- [Six source-version records](source-register.csv): four added references, two newer versions of existing references.
- [Timeline and observation windows](timeline.csv).
- [Source-specific financial observations](financial-observations.csv).
- [Claim-status follow-up](claim-status.csv): links back to relevant original claim IDs.

Original dossier files, CSVs, screenshots and editorial graphics retain their October 31 snapshot and original bytes. An absence of later events in that snapshot should not be read as a current-status claim.

[Overview](../../README.md) · [Sources](../../SOURCES.md) · [Original dossier](../../research/DOSSIER.md)
