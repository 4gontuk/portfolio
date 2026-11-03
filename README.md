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

Since mid 2024 I have joined 60+ audit contests. Code4rena, Sherlock, Cantina, Immunefi, HackenProof. Also CodeHawks, Dual Guard and SpecSiege. I found 115+ real bugs. 40+ are high severity. One is critical. Two podiums are gold. Best single prize so far: $5,000 for 2nd place on Morpho Midnight.

Most of my work is EVM DeFi. Lending markets, DEXes, perps, vaults, staking. Bridges and NFT systems too. Sometimes I leave the EVM. Starknet, Rust L1s, Substrate. If it holds money, I want to see where it breaks.

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

Also contest on CodeHawks, Dual Guard and SpecSiege.

---

## `$ grep "critical\|high" findings/`

Real bugs. All public. Want proof? Open the platform profiles.

| # | Severity | Protocol | Platform | Bug type | What happens |
|---|---|---|---|---|---|
| 01 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **XRP Ledger** | Sherlock | Access control | Batch multisignatures can be rebound to another account with the same signer list, so an attacker spends XRP without owning it |
| 02 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **Fluid DEX v2** | Sherlock | Liquidity | Attacker drains pooled liquidity from honest suppliers |
| 03 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **Ammplify** | Sherlock | Callback validation | Arbitrary token drain from Diamond through an unverified Uniswap V3 mint callback |
| 04 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **Panoptic** | Code4rena | Initialization | Unprotected, re-initializable `BuilderWallet.init()`. Takeover and theft of builder fees |
| 05 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **Olas** | Code4rena | Reentrancy | Cross-service reentrancy in `StakingBase._withdraw`. Protocol goes insolvent |
| 06 | <img src="https://img.shields.io/badge/HIGH-e74c3c?style=flat-square" alt="high"/> | **Winnables Raffles** | Sherlock | ETH accounting | Wrong ETH locking in `refundPlayers`. Funds lock up forever |
| 07 | <img src="https://img.shields.io/badge/HIGH%20%C3%972-e74c3c?style=flat-square" alt="high"/> | **Velocimeter** | Sherlock | Vote escrow | Delegation DoS at `MAX_DELEGATES` · rewards locked forever via `killGaugeTotally` · stale supply checkpoint pays users wrong rewards |
| 08 | <img src="https://img.shields.io/badge/HIGH%20%C3%972-e74c3c?style=flat-square" alt="high"/> | **Chakra** | Code4rena | Cross chain | Anyone can mess with user nonces in the settlement contract. Old Starknet messages can be replayed by anyone |

---

## `$ history | grep podium`

- 🥇 **1st, Covenant** (Code4rena)
- 🥈 **2nd, Morpho Midnight** (Cantina · $400k pot · 3,890 findings submitted · [leaderboard](https://cantina.xyz/competitions/4679e0fa-85f7-4ea5-8827-ee6c70bdee6b/leaderboard)). Solid codebase, no HMs existed. My low and info reports ranked 2nd of everyone. $5,000
- 🥈 **2nd, Sequence: Transaction Rails** (Code4rena)
- 4th Sequence · 6th Pump Science · 9th Rujira. All Code4rena. That Rujira run: 4 High and 4 Medium in one contest
- **14 top-10 finishes.** Sequence #4 · Velar #6, primev #6, Pump Science #6 · Reserve Core #7 · circuit-puzzles #8, hyperlend #8 · Axelar #9, Rujira #9 · Fluid DEX #10, Index Fun #10
- 35x top-25 on Sherlock alone

---

<details>
<summary><b>$ cat full_battle_record.log</b> <i>(every public contest, click to open)</i></summary>

| Date | Contest | Platform | Place | Findings | Paid |
|---|---|---|---|---|---|
| Jun '26 | **Morpho Midnight** | Cantina | 🥈 **2nd** | info only | **$5,000.00** |
| Jun '26 | DRE App (dreUSD) | Sherlock | #65 | - | $27.48 |
| Apr '26 | **XRP Ledger** | Sherlock | **#14** | 1 H / 5 M | **$3,979.95** |
| Apr '26 | Clear Macro by Superfluid | Sherlock | #57 | - | $15.79 |
| Mar '26 | Chainlink Payment Abstraction V2 | Code4rena | #11 | 1 M | - |
| Feb '26 | **Injective Peggy Bridge** | Code4rena | #16 | 1 H / 2 M | $44.12 |
| Feb '26 | **Olas** | Code4rena | #54 | 1 H | $1.21 |
| Feb '26 | **Fluid DEX v2** | Sherlock | **#10** | 1 H / 1 M | $194.51 |
| Feb '26 | OpenCover Insured Vaults | Sherlock | #54 | - | $22.47 |
| Feb '26 | Hotstuff | Sherlock | #39 | - | $29.70 |
| Feb '26 | Flying Tulip | Sherlock | #84 | - | $117.32 |
| Dec '25 | **Panoptic: Next Core** | Code4rena | #15 | 1 H / 4 M | $527.31 |
| Dec '25 | **Rujira** | Code4rena | **#9** | 4 H / 4 M | $703.12 |
| Dec '25 | Monolith Stablecoin Factory | Sherlock | #11 | 4 M | $208.42 |
| Nov '25 | Swafe | Code4rena | #23 | 2 M | $15.58 |
| Nov '25 | **Sequence: Transaction Rails** | Code4rena | 🥈 **2nd** | - | $189.47 |
| Nov '25 | Megapot | Code4rena | #25 | 2 M | $0.13 |
| Oct '25 | **Covenant** | Code4rena | 🥇 **1st** | - | $757.89 |
| Oct '25 | Index Fun Order Book | Sherlock | **#10** | 1 M | $70.67 |
| Oct '25 | **Sequence** | Code4rena | **#4** | 2 M | **$2,109.39** |
| Sep '25 | **Ammplify** | Sherlock | #16 | 3 H / 4 M | $377.46 |
| Aug '25 | Fluid | Code4rena | #16 | - | $764.94 |
| Aug '25 | kuru-contracts | Cantina | #54 | 1 H | $313.61 |
| May '25 | primev-validator-registry | Cantina | **#6** | 1 H | $0.18 |
| May '25 | stability-contracts | Cantina | #26 | 1 H | $77.49 |
| May '25 | circuit-puzzles | Cantina | **#8** | 1 H / 1 M | **$1,139.23** |
| Apr '25 | mezo-monorepo | Cantina | #17 | 1 H | $977.49 |
| Feb '25 | defi-app-contracts | Cantina | #26 | 1 H | $11.53 |
| Jan '25 | daao-contracts | Cantina | #13 | 4 H / 1 M | $296.83 |
| Jan '25 | dahlia-protocol | Cantina | #14 | 1 M | $1,137.14 |
| Jan '25 | Liquid Ron | Code4rena | #11 | 1 M | - |
| Jan '25 | Pump Science | Code4rena | **#6** | 1 M | $417.31 |
| Dec '24 | SecondSwap | Code4rena | #45 | 1 H / 2 M | $6.98 |
| Dec '24 | Oku (New Order Types) | Sherlock | #65 | 1 M | $0.01 |
| Dec '24 | **Lambo.win** | Code4rena | #16 | 2 H / 1 M | $196.51 |
| Nov '24 | Concrete | Code4rena | #55 | - | $141.88 |
| Nov '24 | hyperlend | Cantina | **#8** | 1 M | **$2,708.38** |
| Sep '24 | symbioticfi-core | Cantina | #22 | 1 M | $211.51 |
| Aug '24 | Velar Artha PerpDEX | Sherlock | **#6** | 1 M | $873.14 |
| Aug '24 | **Chakra** | Code4rena | #54 | 2 H | $2.03 |
| Aug '24 | **Cork Protocol** | Sherlock | #15 | 1 H / 1 M | $31.50 |
| Aug '24 | Rumpel Point Tokenization | Sherlock | #14 | - | $88.38 |
| Aug '24 | Superposition | Code4rena | #32 | 1 M | $1.26 |
| Aug '24 | **Phi** | Code4rena | #47 | 1 H | $9.15 |
| Aug '24 | **zetachain-protocol** | Cantina | #16 | 2 H | **$2,162.62** |
| Aug '24 | **Winnables Raffles** | Sherlock | #37 | 1 H | $1.80 |
| Aug '24 | Sentiment V2 | Sherlock | #42 | 2 M | $12.96 |
| Aug '24 | **Axelar Network** | Code4rena | **#9** | - | - |
| Jul '24 | **Basin** | Code4rena | #11 | 1 H | $8.44 |
| Jul '24 | **Reserve Core** | Code4rena | **#7** | - | - |
| Jul '24 | **TraitForge** | Code4rena | #16 | 1 H / 2 M | $284.23 |
| Jul '24 | **LoopFi** | Code4rena | #13 | 1 H / 3 M | **$1,493.94** |
| Jul '24 | **Velocimeter** | Sherlock | #20 | 3 H / 2 M | $439.87 |

*Plus 4 private jobs on Sherlock Audit Engine (Uniswap, Aero, Polygon Heimdall V2, Kamino MetaVault) and 2 NDA audits. Contest numbers are from the Sherlock aggregate. Morpho row comes from Cantina.*

</details>

---

## `$ ./work --private`

6 private jobs so far. None of the reports can be shared. The receipts can.

- **2 classic private audits.** NDA. That is all I can say about those.
- **4 on Sherlock Audit Engine.** Kamino MetaVault (finalizing now), Uniswap, Aero, Polygon Heimdall V2. 22+ valid findings there. $2.8K paid so far. One engagement alone paid $2,521.

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
