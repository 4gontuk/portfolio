<!-- agontuk · smart contract auditor portfolio · numbers pulled from public profiles, nov 2026 -->

<div align="center">
  <img src="assets/header.svg" width="880" alt="Agontuk, smart contract auditor. 60+ audits, 115+ valid findings, $31K+ paid" />
</div>

<div align="center">
  <a href="https://code4rena.com/@Agontuk"><img src="https://img.shields.io/badge/Code4rena-%40Agontuk-a371f7?style=for-the-badge&labelColor=0d1117" alt="Code4rena profile"/></a>
  <a href="https://audits.sherlock.xyz/watson/neeloy"><img src="https://img.shields.io/badge/Sherlock-neeloy-f85149?style=for-the-badge&labelColor=0d1117" alt="Sherlock profile"/></a>
  <a href="https://cantina.xyz/u/Agontuk1"><img src="https://img.shields.io/badge/Cantina-Agontuk1-d2a8ff?style=for-the-badge&labelColor=0d1117" alt="Cantina profile"/></a>
  <a href="https://immunefi.com/audit-competition/audit-comp-quantus/leaderboard/"><img src="https://img.shields.io/badge/Immunefi-Top%209%20Quantus-58a6ff?style=for-the-badge&labelColor=0d1117" alt="Immunefi result"/></a>
  <a href="https://cantina.xyz/competitions/4679e0fa-85f7-4ea5-8827-ee6c70bdee6b/leaderboard"><img src="https://img.shields.io/badge/Morpho%20Midnight-2nd%20%245k-d2a8ff?style=for-the-badge&labelColor=0d1117" alt="Morpho Midnight result"/></a>
</div>

---

## `$ whoami`

I go by Agontuk. I break smart contracts for a living.

Since mid 2024 I have joined 60+ audit contests. Code4rena, Sherlock, Cantina, Immunefi, HackenProof. Also CodeHawks, Dual Guard and SpecSiege. I found 115+ real bugs. 40+ are high severity. One is critical. Two podiums are gold. Best single prize: $5,000 for 2nd place on Morpho Midnight.

Most of my work is EVM DeFi. Lending markets, DEXes, perps, vaults, staking. Bridges and NFT systems too. I also work outside the EVM. Rust, Substrate, Starknet, XRPL core. If it holds money, I want to see where it breaks.

These days I mostly take private audits. Ping me if you need one.

> Want me to break your code before someone else does? [contact.agontuk@gmail.com](mailto:contact.agontuk@gmail.com)

---

## `$ ./stats`

```bash
$ ./agontuk --stats
├─ audit contests ............. 60+
├─ valid findings ............. 115+  (1 critical · 40+ high · 50+ medium)
├─ paid out ................... $31K+
├─ podiums .................... 3  (2 gold, 1 silver)
├─ top-10 finishes ............ 14
├─ protocols helped ........... 55+
└─ private jobs ............... 6  (reports sealed)
```

<p>
  <img src="https://img.shields.io/badge/audits-60%2B-238636?style=flat-square" alt="audits"/>
  <img src="https://img.shields.io/badge/findings-115%2B-da3633?style=flat-square" alt="findings"/>
  <img src="https://img.shields.io/badge/paid-%2431K%2B-bf8700?style=flat-square" alt="paid"/>
  <img src="https://img.shields.io/badge/top--10%20finishes-14x-8957e5?style=flat-square" alt="top-10 finishes"/>
  <img src="https://img.shields.io/badge/critical-1-b40000?style=flat-square" alt="critical findings"/>
</p>

*Numbers come from public profiles. Synced Nov 2026. Private stuff stays private.*

---

## `$ cat platforms.log`

| Platform | Handle | Record | Highlights |
|---|---|---|---|
| [**Code4rena**](https://code4rena.com/@Agontuk) | `Agontuk` | **22 High · 38 Medium** | 🥇 Covenant · 🥈 Sequence Rails · #96 this year · helped 24 protocols |
| [**Sherlock**](https://audits.sherlock.xyz/watson/neeloy) | `neeloy` / `4gontuk` | **2x 1st · 13x top-10 · 35x top-25** | 52 payouts · #398 all time |
| [**Cantina**](https://cantina.xyz/u/Agontuk1) | `Agontuk1` / `4gontuk` | 12 contests · **6 High · 4 Medium** | 🥈 2nd on Morpho Midnight, **$5,000**, my biggest prize · Fellowship '24 · primev #6, circuit-puzzles #8, hyperlend #8 |
| **Sherlock Audit Engine** | `neeloy` | 4 audits · **22+ valid** · $2.8K paid | Kamino MetaVault · Uniswap · Aero · Polygon Heimdall V2 (reports sealed) |
| [**Immunefi**](https://immunefi.com/audit-competition/audit-comp-quantus/leaderboard/) | `n3310y` | 4 valid Highs | #9 of 65 on Quantus. Rust L1, post quantum crypto, 64.8k lines of code |
| **HackenProof** | `-` | **1 Critical** | public bounty |

Also contest on CodeHawks, Dual Guard and SpecSiege. Full history on the three main profiles. Nothing hidden.

---

## `$ grep "critical\|high" findings/`

My sickest finds. Click a protocol name for proof.

Code4rena rows go straight to the exact finding in the official report, my name on it. Sherlock findings live on [my Sherlock profile](https://audits.sherlock.xyz/watson/neeloy) under the same titles.

| # | Severity | Protocol | Platform | Bug type | What happens |
|---|---|---|---|---|---|
| 01 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **[XRP Ledger](https://audits.sherlock.xyz/watson/neeloy)** | Sherlock | Access control | Batch multisignatures can be rebound to another account with the same signer list. An attacker spends XRP without owning it. XRPL later rebuilt the whole Batch amendment as V1.1 over this bug class |
| 02 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **[Fluid DEX v2](https://audits.sherlock.xyz/watson/neeloy)** | Sherlock | Liquidity | Attacker drains pooled liquidity from honest suppliers |
| 03 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **[Ammplify](https://audits.sherlock.xyz/watson/neeloy)** | Sherlock | Callback validation | Arbitrary token drain from Diamond through an unverified Uniswap V3 mint callback |
| 04 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **[Panoptic](https://code4rena.com/reports/2025-12-panoptic-next-core#h-01-builderwallet-init-is-unprotectedre-initializable-enabling-takeover-and-theft-of-builder-fees)** | Code4rena | Initialization | Unprotected, re-initializable `BuilderWallet.init()`. Takeover and theft of builder fees |
| 05 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **[Olas](https://code4rena.com/audits/2026-01-olas/submissions/S-902)** | Code4rena | Reentrancy | Cross-service reentrancy in `StakingBase._withdraw`. Protocol goes insolvent |
| 06 | <img src="https://img.shields.io/badge/HIGH%20%C3%972-e74c3c?style=flat-square" alt="high"/> | **[Velocimeter](https://solodit.cyfrin.io/issues/h-2-votingescrow-max_delegates-value-can-lead-to-dos-on-certain-evm-compatible-chains-sherlock-velocimeter-git)** | Sherlock | Vote escrow | Delegation DoS at `MAX_DELEGATES` ([on Solodit](https://solodit.cyfrin.io/issues/h-2-votingescrow-max_delegates-value-can-lead-to-dos-on-certain-evm-compatible-chains-sherlock-velocimeter-git)) · rewards locked forever via `killGaugeTotally` · stale supply checkpoint pays users wrong rewards |
| 07 | <img src="https://img.shields.io/badge/HIGH%20%C3%972-e74c3c?style=flat-square" alt="high"/> | **[Chakra](https://code4rena.com/reports/2024-08-chakra#h-07-anyone-can-manipulate-user-nonce-nonce_manager-in-settlement-contract)** | Code4rena | Cross chain | User nonces can be manipulated by anyone, [H-07](https://code4rena.com/reports/2024-08-chakra#h-07-anyone-can-manipulate-user-nonce-nonce_manager-in-settlement-contract) · processed Starknet messages replayable, [H-02](https://code4rena.com/reports/2024-08-chakra#h-02-in-starknet-already-processed-messages-can-be-re-submitted-and-by-anyone) |
| 08 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **[LoopFi](https://code4rena.com/reports/2024-07-loopfi)** | Code4rena | Accounting | `AuraVault::claim` skips fee deduction from reward amounts. DoS or rewards silently lost |

---

## `$ history | grep podium`

- 🥇 **1st, Covenant** (Code4rena). The official report names my writeup as [the judge's top score](https://code4rena.com/audits/2025-10-covenant/submissions/S-505)
- 🥈 **2nd, Morpho Midnight** (Cantina). [$400k pot, 3,890 findings submitted](https://cantina.xyz/competitions/4679e0fa-85f7-4ea5-8827-ee6c70bdee6b/leaderboard). $5,000. My biggest single prize
- 🥈 **2nd, Sequence: Transaction Rails** (Code4rena, [report](https://code4rena.com/reports/2025-11-sequence-transaction-rails))
- 11 more top-10s: [#4 Sequence](https://code4rena.com/reports/2025-10-sequence) · [#6 Pump Science](https://code4rena.com/reports/2025-01-pump-science) · #6 Velar, primev · [#7 Reserve Core](https://code4rena.com/reports/2024-07-reserve-core) · #8 circuit-puzzles, hyperlend · [#9 Axelar Network](https://code4rena.com/reports/2024-08-axelar-network) · #9 Rujira, Quantus · #10 Fluid DEX v2, Index Fun
- Sherlock and Cantina placements are on my profiles. Same handles, same results

---

## `$ ./scope --beyond-solidity`

- **Quantus** (Immunefi, #9 of 65). Rust, Substrate, lattice signatures, zk circuits. 64.8k lines of code
- **XRP Ledger** (Sherlock, #14). XRPL core amendments. Batch multisigs, MPToken vaults, sponsorship. Not EVM
- **Chakra** (Code4rena). Starknet, Cairo. Cross-chain messaging and settlement

Non-EVM is not a side quest. I take these contests on purpose.

---

## `$ ./work --private`

6 private jobs so far. None of the reports can be shared. The receipts can.

- **2 classic private audits.** NDA. That is all I can say about those.
- **4 on Sherlock Audit Engine.** Kamino MetaVault (finalizing now), Uniswap, Aero, Polygon Heimdall V2. 22+ valid findings there. $2.8K paid so far. One engagement alone paid $2,521.
- No public links yet. Reports drop when clients publish them. The engagement names are the receipts.

How I work:

- I read all the code. Then I try to steal from it.
- Every bug ships with a working proof of concept.
- You get a plain report. What to fix and why. No filler.
- When you ship fixes, I recheck them.

Solidity / EVM · lending · DEX and perp systems · vaults, staking, restaking · bridges · NFT systems · Starknet (Cairo) · Rust and Substrate L1s.

Want one? [contact.agontuk@gmail.com](mailto:contact.agontuk@gmail.com)

---

## `$ contact --list`

| | |
|---|---|
| <img src="assets/avatar.png" width="120" alt="Agontuk avatar"/> | <a href="mailto:contact.agontuk@gmail.com"><img src="https://img.shields.io/badge/email-contact.agontuk-c9d1d9?style=flat-square&logo=gmail&logoColor=white&labelColor=21262d" alt="email"/></a><br/><a href="https://x.com/4gontuk"><img src="https://img.shields.io/badge/%404gontuk-X-e6edf3?style=flat-square&logo=x&logoColor=white&labelColor=21262d" alt="X"/></a><br/><a href="https://t.me/Ag0ntuk"><img src="https://img.shields.io/badge/%40Ag0ntuk-Telegram-26a5e4?style=flat-square&logo=telegram&logoColor=white&labelColor=21262d" alt="Telegram"/></a><br/>discord → `@4gontuk` |

---

<div align="center">
  <img src="https://img.shields.io/badge/status-open%20for%20private%20audits-3fb950?style=for-the-badge&labelColor=0d1117" alt="open for private audits"/><br/><br/>
  <sub>numbers pulled from public profiles · nov 2026</sub>
</div>
