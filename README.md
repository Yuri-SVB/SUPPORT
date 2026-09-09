<p align="center">
  <img src="assets/yuri.png?raw=true" alt="Yuri da Silva Villas Boas" width="180">
</p>

<h1 align="center">Yuri da Silva Villas Boas</h1>

<p align="center">
  <strong>Applied Cryptographer</strong><br>
  <sub>Coercion-resistant Bitcoin self-custody · author of BIP-450 · Great Wall</sub>
</p>

<p align="center">
  <a href="https://twitter.com/yurivillasboas">X</a> ·
  <a href="https://njump.me/yurisvb@nostrplebs.com">Nostr</a> ·
  <a href="https://www.linkedin.com/in/yuri-da-silva-villas-boas-a1995143/">LinkedIn</a> ·
  <a href="https://github.com/Yuri-SVB">GitHub</a>
</p>

---

# ⚡ Support

Free software and free documents on coercion-resistant Bitcoin self-custody.
Nothing here is gated, delayed, or for sale. If some of it was worth something
to you, this is where to say so.

<img src="assets/lightning-offer-qr.png?raw=true" width="240" align="left" alt="Lightning BOLT12 offer QR code">

**⚡ Lightning** — BOLT12 offer · reusable · scan the code or copy the string

```
lno1pgqppmsrse80qf0aara4slvcjxrvu6j2rp5ftmjy4yntlsmsutpkvkt6878sx00dte5jw8axkhj4zg6skes6cema5ntf6xg3czz94yqzg8rv66vjqgpusqusntzmtyc30d4k9axx6j75zyquezf9hyrheh4lggnmm8sypzqqxwrklrq3vj2y9w4jxp0fzdxh8rc4rzf2m7ssrte56upl2qqm85ffxtwl5ay90e0z2uscpm3eyxdr9c07s2pqxw0x4pfmzcdxelfju0hh0apdmxxc3l9lld5h2wfuhwulsedjjg3eqqew5wgxv3zc6qzsl0eahjhsznvpxe88rzxw04yw5685jj4quqny9xqpmvehu3dmtq6t7pnzs2zjuaewcgyq
```
<details>
<summary>ℹ️ <sub>What is a BOLT12 offer?</sub></summary>

A **BOLT12 offer** (`lno1…`), not a Lightning address or a BOLT11 invoice.
Permanent and reusable — your wallet fetches a fresh invoice from it on every
payment, over a blinded path, so nothing is reused and paying it does not
reveal my node.

> **⚠️ Wallet support is narrower than for `lnbc…` invoices.**
> **Phoenix**, **Zeus**, and **Core Lightning** pay offers today. If your wallet
> rejects it, that is a missing feature, not a bad string.

</details>

<br clear="all"><br>

<img src="assets/silent-payment-qr.png?raw=true" width="240" align="left" alt="Silent payment address QR code">

**⛓️ On-chain** — silent payment · BIP-352

```
sp1qq2d6duq9c3f3tewjpd4gry4y5q849yq3qna48r725p785kgxgmugqq469df4alnlf07afhpukw2nvmn6j8rnh56539w73e8m84ddt7858qgkjlnw
```
<details>
<summary>ℹ️ <sub>Why a silent payment?</sub></summary>

A silent payment address (`sp1…`,
[BIP-352](https://github.com/bitcoin/bips/blob/master/bip-0352.mediawiki)) —
for larger amounts and for people who run no Lightning wallet at all. Every
payment lands on a fresh, unlinkable output, so nothing accumulates in public.

</details>

<br clear="all"><br>

What has actually shipped is logged in [`DELIVERED.md`](./DELIVERED.md), dated,
in git history that anyone can audit.

---

## 📦 The work

**📜 [BIP-450 — Formosa](https://github.com/bitcoin/bips/blob/master/bip-0450.mediawiki)**
A forwards- and backwards-compatible expansion of BIP-39 that maps seed entropy
onto grammatical sentences instead of word lists. In the Bitcoin standards
repository.

**🎲 [BTC-D20](https://github.com/Yuri-SVB/BTC-D20)**
A printable two-page kit for generating a BIP-39 seed phrase with a 20-sided
die, in English, Spanish, Italian, and Brazilian Portuguese. Entropy you watch
happen, with no electronic RNG anywhere in the process.

**🧱 [Great Wall](https://github.com/Yuri-SVB/Great-Wallet)**
A protocol for coercion-resistant self-custody through Tacit Knowledge-Based
Authentication — memory-held entropy navigated against a user-specific
perturbation of a fractal, gated by a calibrated derivation. The first
construction that is Kerckhoffian and coercion-resistant at the same time.

**🔬 [Research](https://github.com/Yuri-SVB/great-wall-docs)**
A formal threat model for physical ("$5 wrench") attacks on Bitcoin holders,
building on [Jameson Lopp's incident registry](https://github.com/jlopp/physical-bitcoin-attacks),
to which incident data goes upstream — where it is public property and belongs
to everyone, not to this project.

---

## 🤝 What support does, per project

These are at different stages, and the honest ask differs for each.

### 🎲 BTC-D20 — a finished thing

It works today, it needs nothing from me to keep working, and it will never
need a server, a subscription, or an update. If you printed it and used it,
that's the classic case: it was worth something, you decide how much.

### 🧱 Great Wall — development, not a product

The implementation is a **prototype**. Do not put savings behind it yet.
Support here funds the work that gets it to the point where I would tell you
otherwise. It is not a purchase, and it buys no priority, no early access, and
no support obligation.

### 🔬 The research — papers, standards, registry work

BIP-450 is finished and public. The threat-model work is under academic review.
The incident data belongs to the registry that hosts it. None of this is
fundable in the ordinary sense and none of it pays; if you think it should
exist, this is the mechanism.

---

## ✅ The pledge

- **Free forever.** MIT or Apache-2.0, and that does not change.
- **No gated features.** Not now, not in a later "pro" edition.
- **No donor priority.** Donating buys no support obligation, no feature
  requests, and no place in a queue. If you need something, open an issue like
  everyone else — that is where it will be answered.
- **No delayed releases.** Nothing is held back for supporters.

If you want something built, say so in an issue. That directs the work better
than money does.

---

## 🔍 Notes on the two rails

**Lightning** is for small and impulsive amounts. The keys are mine — nothing
here is custodial — but liquidity is managed by a provider rather than by a
node I would have to keep alive. A donation channel only ever receives, so its
inbound capacity depletes in one direction and payments eventually start
failing silently, on your screen, where I would never learn about it. That
trade buys reliability at the cost of a piece of infrastructure sovereignty a
tip jar does not need. Stating it plainly seems better than implying otherwise.

A BOLT12 offer rather than a static invoice or a Lightning address, because it
is reusable without being *reused*: each payment fetches its own invoice over a
blinded path, so donations are not linkable to one another and paying one does
not reveal my node.

**The on-chain rail** is a silent payment address — for larger amounts and for
people who keep everything in cold storage and run no Lightning wallet at all.

It is a silent payment rather than an ordinary address for a reason that is
the whole argument of this project: a static reused address publishes a running
balance next to a real name, which is precisely the targeting pattern the
research documents — attacks driven by aggregated public data rather than by
anything the holder disclosed. Every payment to an `sp1` address lands on a
fresh, unlinkable output instead. Nothing accumulates in public.

The same principle runs through both rails, and it is the only reason either is
shaped the way it is: the point is not that you should trust me. It is that you
should not have to.
