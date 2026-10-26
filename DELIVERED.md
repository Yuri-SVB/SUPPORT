# 📦 Delivered

A dated record of what has actually shipped, newest first.

This file exists so that "the work is happening" is a checkable claim rather
than an assertion. Git carries the timestamps, so entries cannot be quietly
backdated or removed — [check the log](https://github.com/Yuri-SVB/support/commits/main/DELIVERED.md)
rather than taking this page's word for it.

No promises are made about cadence. Entries are added when something ships,
and nothing is listed here that has not.

---

**🎨 2026-10-26 — Great Wallet: brightness controls**
Brightness now falls steadily with escape count, so a deeper shell is never
brighter than a shallower one. A slope control (`G`) joins the offset (`L`),
and `A` turns on auto exposure, which fits both to what is on screen, as the
film does. Deep render (`Alt+L`) now gives every escape count its own shade
instead of merging them four at a time. great-wallet `c095bc0`.

**🎥 2026-10-26 — Great Wall demo 70**
[Full-length film](https://www.youtube.com/watch?v=Ry9wzHq1wOA) from
`great-wall-render`, protocol 0.4.0. Each map is now toured from its outer
shell to the canonical leaf through a chain of landmark features, and every
frame is lit from its own escape counts so shells read as distinct shades.
Demo entropy only.

**🔐 2026-10-25 — Great Wall protocol 0.5.0**
The orbit's state widens to 512 bits (SHA-512), and each stage's master
secret is now separate from the value that advances the orbit, so a leaked
key no longer hands out the next stage's orbit point. Keys leave only through
a label-salted export. Core, its Python reference, frozen test vectors and the
wallet moved together; 0.4.0 setups must be rebuilt. great-wallet `aa431ab`.

**🎥 2026-10-20 — Great Wall demo 65: the rendered film, narrated**
[Full-length film](https://youtu.be/j8Fgh9jPZEo) from `great-wall-render`,
reworked since demo 60 to sit closer to the real app. After each 32-bit
point is committed, the camera moves to the wallet's own canonical view of
that leaf and lights its canonical island, exactly as core selects it. The
explanatory cards type out on a console screen while a synthetic voice reads
them; the stage advance shows its time gate as a progress bar over a
user-set number of non-parallelizable, deterministic steps, then fades one
stage's fractal out and the next one in; every event has its own sound cue.
The cards state the claims plainly: the fractal is a perceptual oracle; a
wrench attacker would have to hold you for the entire key-derivation time
chosen at setup; preliminary experiments put setup training at about five
hours and upkeep at five minutes a week. Demo entropy only.

**🔧 2026-10-16 — Formosa: Table Selector fixes and keyboard navigation**
A screening pass over the [Formosa](https://github.com/Yuri-SVB/formosa)
desktop application. Fixes: the shuffle of the grid keys, the only thing hiding
the chosen word from an onlooker, was drawn from a Mersenne Twister whose every
output is put on screen, which is enough to predict the next ones; it is now
drawn from the system entropy source. Switching tabs no longer sends the grid
back to the first word of a half-built phrase, so the next pick can no longer
fill the wrong slot. Two tabs opened blank until clicked. An error mid-search
could leave a cached theme searching the wrong words. Changing theme enabled
Generate Phrase with nothing picked. `setup.py`, still Trezor's, could not run,
and an installed copy would have carried no themes. `output.txt`, where Save
writes seed phrases in plain text, was not git-ignored. Improvements:
Backspace and a Back button give up the last key or word picked; the left and
right arrows walk the phrase so an earlier word can be reviewed or swapped, with
the compatibility warning recomputed from the words each time; Ctrl+PageUp and
Ctrl+PageDown cycle the tabs; and the screen says which word the grid is on
("Phrase 2, word 3 of 6") and names the syntactic slot being filled.

**🎥 2026-10-16 — Great Wall demo 60: the rendered film, protocol 0.4.0**
[Full-length film](https://www.youtube.com/watch?v=3sKMejVDF9s) from
`great-wall-render`, an offline renderer that animates the encoding itself:
islands appear, a split line lands, a bit picks a half and the camera dives,
one bit at a time, a word every eleven bits, across the 0.4.0 orbit layout of
sibling boards per stage. Explanatory cards state the argument outright rather
than leaving it to inference: the encoding is one-to-one; the place is
recognisable with the fractal in front of you and inexpressible without it, so
threat or torture cannot extract what cannot be said; and the next fractal
costs hours per stage, so nobody could have produced it faster. Demo entropy
only — the renderer displays the bits, which is exactly why it must never see
a real seed.

**📰 2026-10-05 — Ten posts published, five languages each**
A [reading series](https://github.com/Yuri-SVB/great-wall-posts) also live at
[yuri-svb.github.io](https://yuri-svb.github.io/posts/) on coercion-resistant
self-custody, fifty pages in English, Portuguese, Spanish, French and Italian:
why the window for keeping a low profile has closed, what Kerckhoffs says about
decoys and duress PINs, the arithmetic that makes a half-finished seizure price
the holder's death, the Balland case, the RATIRL torture, a French tax-office
database queried for people who had declared crypto gains, and what today's
wrench-attack numbers extrapolate to. Each one ends at a DOI rather than at a
PDF in a repository, and every figure carries its caveat in the same sentence:
the registry is a press-sourced sample coded by headline, the categories
overlap, and the fatality share is a floor.

Two had run before and are included for completeness: *The Window Has Closed*
on 17 September, and *Does Hiding Your Bitcoin Still Protect You?* in Brazilian
Portuguese at [bitcoinblock.com.br](https://bitcoinblock.com.br/2026/09/22/esconder-bitcoin-ainda-protege/)
on 22 September. The other eight are new. The arguments are the two open-access
papers, [*The Deadly Race*](https://zenodo.org/doi/10.5281/zenodo.22018891) and
[*The Denial Spiral*](https://zenodo.org/doi/10.5281/zenodo.22778480); the posts
are the plain-language route in.

**🌀 2026-09-16 — *The Denial Spiral* v1 deposited**
[Companion paper](https://zenodo.org/doi/10.5281/zenodo.22778480) split out of the
wrench-attack threat model: the obscurity class, the mechanism running from a
norm of concealment through attacker disbelief to further coercion, the
praxeological account of what kind of claim this is, the four mechanisms that
censor the evidence — one of which survives publication — and the registry
coding method behind the empirical grounding. Concept DOI; resolves to the
latest version.

**💀 2026-09-16 — *The Deadly Race* v4**
[Fourth version](https://zenodo.org/doi/10.5281/zenodo.22778256) of the coercion-resistance
threat model, with a [changelog](https://github.com/Yuri-SVB/great-wall-docs/blob/main/papers/wrench-attack-threat-model/CHANGES-v4.md)
absorbing v3, which shipped without one. The manuscript is now two papers, cut
along the epistemic boundary. Three claims v2 stated loosely are made rigorous:
the pivotal condition is non-completion rather than relative pace, the spend
authority is a set of states rather than a private key, and the hostage surface
needs a necessary *subset* of tokens rather than a single necessary one. A
vendor now documents the naive tier in its own words, and the design comparison
gains a column asking the criterion directly — which the four properties do not
generate. No design's classification changed.

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
