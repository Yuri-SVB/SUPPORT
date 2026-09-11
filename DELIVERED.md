# 📦 Delivered

A dated record of what has actually shipped, newest first.

This file exists so that "the work is happening" is a checkable claim rather
than an assertion. Git carries the timestamps, so entries cannot be quietly
backdated or removed — [check the log](https://github.com/Yuri-SVB/support/commits/main/DELIVERED.md)
rather than taking this page's word for it.

No promises are made about cadence. Entries are added when something ships,
and nothing is listed here that has not.

---

**🔗 2026-08-13 — Three incidents merged into the physical-attacks registry**
Revelles (FR), Trincity (TT), and Paris (FR) added to
[`jlopp/physical-bitcoin-attacks`](https://github.com/jlopp/physical-bitcoin-attacks/pull/212)
with archival links, reviewed and merged upstream. The data belongs to the
registry, not to this project.

**🎲 2026-08-05 — BTC-D20 published**
[Printable D20 seed-generation kit](https://github.com/Yuri-SVB/BTC-D20) in
English, Spanish, Italian, and Brazilian Portuguese. The lookup table is built
directly from the commit-pinned `bitcoin/bips` wordlist, and both worked
examples are machine-verified against the BIP-39 checksum algorithm.

**🎥 2026-08-02 — Great Wall demo 50: protocol 0.4.0**
[Walkthrough](https://www.youtube.com/watch?v=9lJvw-8PZOA) of the protocol at
version 0.4.0.

**🧂 2026-07-05 — Namtso, the Sacred Salt**
[Reference library and CLI](https://github.com/Yuri-SVB/namtso-the-sacred-salt)
for a memorization-free, precomputation-resistant salt derived from the Bitcoin
timechain: a person reproduces it from a single remembered date, harvests from a 
local node, an offline headers bundle, or cross-checked public explorers, with 
optional date cloaking so a remote source learns an interval rather than the day. 
Shipped with frozen test vectors.

**🎥 2026-06-28 — Great Wall demo 45: Dart interface**
[Video](https://youtu.be/zoJF1Ex7hkI) of the reworked interface — the
polished-UX milestone.

**🎥 2026-05-31 — Great Wall demo 40: 24-word round trip**
[Video](https://www.youtube.com/watch?v=oeHELcybK5E) demonstrating the
bijection at maximum-length input, in both directions.

**📚 2026-05-31 — `great-wall-docs` consolidated**
Design documents, threat model, architecture, papers, and go-to-market
material gathered into
[one public repository](https://github.com/Yuri-SVB/great-wall-docs).

**📣 2026-05-31 — Public peer review opened**
A Great Wallet discussion opened on the **bitcoindev** mailing list, putting
the protocol in front of open review.

**🎬 2026-05-31 — Formosa / BIP-450 explained**
[Guest appearance](https://www.youtube.com/watch?v=-Obi5y_rM7c) walking
through Formosa and BIP-450 (in Portuguese).

**🎥 2026-05-19 — Great Wallet demo 39: BIP-39 round trip**
[Video](https://www.youtube.com/watch?v=qO66Hg07WNM) demonstrating the 12-word
bijection in both directions.

**📜 2026-04-17 — BIP-450 (Formosa) merged into `bitcoin/bips`**
Formosa promoted from proposal to
[an official BIP](https://github.com/bitcoin/bips/blob/master/bip-0450.mediawiki):
seed entropy mapped onto grammatical sentences, forwards- and
backwards-compatible with BIP-39.
