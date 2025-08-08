# Lido-research

## 1. Executive Summary（摘要）
（建议最后写，浓缩全文）

简要介绍 Lido 是什么、做了什么、为什么重要

强调它在 ETH 流动性质押市场的垄断地位

给出你对它的估值、增长、风险、投资价值的核心判断（多空逻辑）

### 2.1 Core Protocol Mechanism
Lido Finance is the largest liquid staking provider on Ethereum, enabling anyone to stake any amount of ETH and receive stETH in return. Users bypass the technical and financial barriers of solo staking—such as operating a validator and locking 32 ETH—by depositing into Lido’s smart contract. The protocol then delegates these deposits to a set of vetted professional validators selected by the Lido DAO.

In return, users receive stETH, a rebasing token minted 1:1 with the deposited ETH. This token automatically increases in balance daily as staking rewards accumulate, allowing holders to passively earn ETH staking yield while preserving liquidity.

For DeFi users and protocols that require fixed-balance assets, Lido offers wstETH, a wrapped, non-rebasing version of stETH. wstETH reflects rewards through an increasing exchange rate against ETH. This design gives Lido the flexibility to serve both casual ETH holders and sophisticated DeFi participants.

<img width="1920" height="950" alt="image" src="https://github.com/user-attachments/assets/52c87ca0-5ba8-418e-8a0d-369c246269e9" />


### 2.2 stETH, Composability, and DeFi Adoption
One of Lido’s defining strengths lies in the broad composability of stETH and wstETH within the Ethereum DeFi ecosystem. These tokens are accepted across over 35 protocols as of mid-2025, ranging from lending markets to DEXs, structured products, and Layer-2 networks.

stETH is widely used as collateral on Aave and MakerDAO, and supports efficient swaps through Curve’s stETH/ETH pool—one of the deepest in DeFi. Meanwhile, wstETH has become the preferred format for liquidity provisioning on Uniswap and bridging to Layer-2s.

The effect is a powerful feedback loop: as more protocols integrate stETH and wstETH, their utility grows, drawing in more users and reinforcing Lido’s dominance. Even Layer-2s like Linea now auto-stake ETH into stETH for yield, underlining its role as DeFi’s “default staking token.”

### 2.3 Fee Model and LDO Token Utility
Lido charges a 10% protocol fee on staking rewards, with 90% going to users. This fee is split between the DAO treasury and node operators (currently 50/50). For example, if Ethereum’s native staking APR is 4%, Lido users receive about 3.6% after fees. The treasury portion funds audits, liquidity incentives, and future development—such as the Curve pool seeding or Lido V3 R&D.

Reward distribution differs by token: stETH auto-compounds by increasing balances daily, while wstETH holds a fixed balance with a rising price. Users can convert between them freely.

Lido’s governance token, LDO, grants holders decision-making power over the protocol. Via Snapshot, holders can vote on changes such as validator onboarding, treasury allocation, and parameter tuning. However, LDO currently carries no direct claim on revenue—all rewards flow to the DAO. While revenue-sharing proposals have been discussed, no model is live yet as of August 2025.

<img width="959" height="533" alt="image" src="https://github.com/user-attachments/assets/b1cb39be-3fef-4081-bb0d-9ab088956ea5" />


## 3. Market Position & Competitive Landscape
### 3.1 Market Share & Leadership
Lido remains the largest single staking entity, securing ~8.9M ETH (~24.5% as of Aug 2025). But while Ethereum’s overall staking base has continued to expand (now >36M ETH), Lido’s deposits have not grown at the same pace, so its market share has drifted down from a >30% peak. The difference has been absorbed by rising alternatives—most visibly eETH/cbETH on the token side and CEX custody—alongside community efforts to diversify validators. Lido still leads on liquidity depth and DeFi integrations, yet the moat is being diluted at the margin as share keeps sliding even with absolute stake roughly flat-to-up.

<img width="1506" height="618" alt="image" src="https://github.com/user-attachments/assets/ebfdc600-64ad-4ed1-a717-cd529f9c9531" />

### 3.2 Competitor Landscape
There are two overlapping views. By entity, Lido remains the largest single staker; among centralized exchanges, Binance is the biggest block of competition by share, followed by Coinbase and Kraken. By liquid staking tokens (LSTs), however, the most substitutable challengers to stETH are Ether.fi’s eETH and Coinbase’s cbETH, with Rocket Pool’s rETH anchoring the decentralization end of the spectrum.

**Coinbase (cbETH).** Centralized service with a liquid token. Distribution and fiat on-ramps are its superpower, and cbETH keeps gaining DeFi acceptance. Trade-off: custodial exposure and slower integration velocity vs. stETH. *~2.4M ETH, ~6–7%.*

**Binance (CEX staking).** Largest single CEX competitor **by entity share** (≈8%+). Frictionless for in-exchange users, but limited on-chain composability and transparency vs. LST protocols—more “off-chain yield channel” than DeFi-native substitute.

**Kraken (CEX staking).** Institution-friendly, compliance-first staking with similar pros/cons to Binance/Coinbase custody; negligible DeFi surface area. **Indirect** pressure via convenience and brand trust.

**Ether.fi (eETH).** 2024–2025 breakout. Non-custodial UX, restaking alignment, and incentives drove rapid share gains. Strong DeFi integrations, while validator decentralization and stacked restaking risk remain under scrutiny. *~2.5M ETH, ~7%.*

**Rocket Pool (rETH).** Permissionless node operators and a community-first ethos deliver the clearest decentralization story. Liquidity depth and absolute scale are more modest, but growth is steady. *~0.7M ETH, ~2%.*

**Frax (frxETH/sfrxETH).** Two-token design separates base liquidity (frxETH) from yield (sfrxETH). Small headline share (~0.3%) yet outsized mindshare among DeFi strategists.

**StakeWise v3 (osETH).** Vault-/module-based architecture with DVT compatibility; prioritizes customizability and risk isolation. Integrations are improving; scale is still ramping.

**Mantle (mETH/cmETH).** Treasury-backed, “double-yield” narrative inside an L2 ecosystem. Early adoption skews toward advanced users inside Mantle; cross-ecosystem liquidity is the next hurdle.

#### Comparative matrix — stETH vs key alternatives *(sorted by scale, Aug 2025 snapshot)*

> Figures are approximate and for comparison only. CEX rows are **by entity** (converted from share), LST rows are **by token**.

| Protocol | Token | **Scale (Aug-2025, ~)** | Model | Validator Decentralization | DeFi Liquidity/Integrations | Restaking-Native | Primary Edge | Key Risks |
|---|---|---|---|---|---|---|---|---|
| **Lido** | **stETH / wstETH** | **~9.0M ETH (~24–25%)** | LST w/ multi-operator + Staking Router (DVT roadmap) | High (diverse operators; expanding via DVT) | **Highest** (deepest liquidity; widest integrations) | Optional via third-party | Network effects + liquidity depth | Share concentration; governance/coordination risk |
| **Binance** | — (custodial) | **~3.0M ETH (~8.4% by entity)** | CEX staking | Low | Low–Mid (on-chain weak) | No | UX simplicity; massive user base | Custodial/venue risk; limited composability |
| **Ether.fi** | **eETH / weETH** | **~2.5M ETH (~7%)** | LST with non-custodial UX; restaking-aligned | Mid–High (improving) | High (fast integrations) | **Yes** (core to thesis) | Yield stack + user sovereignty narrative | Stacked risk from restaking; validator dispersion questions |
| **Coinbase** | **cbETH** | **~2.4M ETH (~6–7%)** | CEX-backed LST | Mid (custodial) | Mid–High (brand + growing DeFi support) | Limited/indirect | Distribution; compliance credibility | Custodial exposure; slower feature velocity |
| **Kraken** | — (custodial) | **~2.35M ETH (~6.5% by entity)** | CEX staking | Low | Low | No | Compliance/institutional reach | Same as above |
| **Rocket Pool** | **rETH** | **~0.7M ETH (~2%)** | Permissionless node set | **Highest** among majors | Mid (solid but thinner than stETH) | Limited | Decentralization purity | Liquidity/scale constraints |
| **StakeWise v3** | **osETH** | **Sub-1% (growing)** | Modular vaults + DVT-ready | Mid–High | Mid | Optional | Customizability; risk isolation | Smaller network effects; integration ramp |
| **Mantle** | **mETH / cmETH** | **Sub-1% (early)** | L2-aligned LST, treasury-backed “double yield” | Mid | Mid (ecosystem-skewed) | Optional | Ecosystem leverage | Cross-ecosystem liquidity; complexity |
| **Frax** | **frxETH / sfrxETH** | **~0.1M ETH (~0.3%)** | Two-token (liquidity vs. yield) | Mid | Mid–High (strategy-friendly) | Optional | Design flexibility; DeFi strategy fit | Complexity; limited scale today |


### 3.3 Decentralization, Regulation, and Moat
Lido’s dominance has drawn criticism over centralization. The DAO controls validator selection (currently ~30 operators), and large LDO holders exert considerable influence over governance. To address this, Lido has introduced dual governance (allowing stETH holders to veto proposals) and is testing DVT systems for more distributed validator control.

From a regulatory standpoint, the outlook has improved. In August 2025, the SEC clarified that liquid staking tokens like stETH and rETH are not securities, recognizing them as technical staking receipts rather than investment contracts. This has removed a significant overhang from U.S. market participants.

Despite this, governance tokens like LDO are still under observation. While Lido does not distribute revenue to LDO holders, future fee-sharing mechanisms could raise regulatory questions. For now, Lido’s DAO remains legally unincorporated, governed by tokenholders and executed via multisig.

Finally, Lido’s moat is strong yet eroding. The protocol’s early mover advantage has created unmatched liquidity and integrations; stETH/wstETH is still the base asset in lending markets and the deepest ETH pair on Curve and Balancer. The DAO also controls a substantial treasury to incentivize new integrations. However, competitors are gaining ground: Ether.fi, Rocket Pool and cbETH are all expanding, and Lido’s share has steadily declined from >30% to ~24.5%. Decentralization modules have yet to materially boost Lido’s own stake inflows. Replicating Lido’s ecosystem entrenchment will take time, but the network effects are no longer uncontested—improving decentralization and defending liquidity depth are now as important as growth itself.

## 4. Tokenomics & Distribution
### 4.1 Supply Mechanism – Fixed Cap, Blurry Value Accrual
LDO has a fixed total supply of 1 billion tokens, with approximately 890 million already in circulation. There is no ongoing issuance, no programmed burn, and no formal buyback mechanism. In other words, while supply is capped, there is also no direct demand-side mechanism—such as revenue sharing, staking rewards, or fee discounts—to anchor long-term value.

This leaves LDO’s price largely dependent on governance utility and market speculation about future protocol growth, rather than any intrinsic yield.
Proposals to change this have emerged repeatedly:

- Feb 2024 — “Activate Lido Protocol Governance with Revenue Share Staking” proposed directing 20–50% of protocol revenue to LDO stakers, with weekly buyback-and-distribution and a six-month vesting period.

- Jun 2025 — “Enable LDO Staking with Protocol Revenue Sharing” suggested giving stakers 20–30% of revenue, paid in ETH, stETH, or via LDO buybacks.

Both gained attention but have not been implemented, due to concerns over treasury depletion and protocol sustainability.

<img width="1407" height="795" alt="image" src="https://github.com/user-attachments/assets/98843306-c0b7-40ab-a8ca-df866686ee19" />

### 4.2 Initial Allocation vs Current Structure – Early Concentration, Limited Governance Reach
Initial allocation (2020 launch):
- DAO Treasury — 36%
- Early Investors — 22%
- Team — 20%
- Node Operators — 6.5%
- Liquidity Mining Incentives — 15%

The current distribution is roughly:
- Team & Validators — 40%
- Investors — 34.6%
- DAO Treasury — 25.3% (~253.5 M LDO)

The 15% liquidity mining allocation was a one-time distribution during Lido’s early growth phase, rewarding LPs and early DeFi adopters. It was not PoW mining—LDO has never been mined. Most of these tokens have already been distributed and are no longer locked.

Despite the broad token unlock, governance power remains concentrated in a handful of large wallets. Active voter participation is low, with most proposals decided by a small group of delegates. This introduces the classic DeFi paradox: decentralized in theory, oligarchic in practice.




### 4.3 DAO Treasury – Well-Funded, Under-Leveraged
The DAO Treasury currently holds over 100 M LDO and significant ETH/stETH reserves, valued at an estimated $400–480 M depending on market conditions. Historically, treasury usage has been cautious and episodic:
- 2021 — Proposal to sell 100 M LDO to strategic partners like Paradigm in exchange for ETH, with gradual unlocks, to onboard long-term ecosystem allies.
- 2023 — Multiple motions to diversify holdings into stablecoins to secure multi-year operational runway.
- 2023 — Discussion to create a Treasury Management Committee to formalize spending policy.
- 2024–2025 — Revenue-sharing proposals (see 4.1) debated but not enacted.

To date, the treasury’s primary uses have been ecosystem grants, liquidity incentives, and operational costs, but without a recurring, structured capital deployment framework. The size of the treasury is a valuation anchor for LDO, but its economic impact on token holders remains unrealized.

(Insert Dune chart: DAO Treasury LDO balance over time)

5. Financial Performance & Revenue Model（财务表现与收入模型）
5.1 收入来源
Lido 对 staking 奖励抽取 10% 费用

其中 50% 分给节点运营者，50% 进入 DAO Treasury

5.2 年化收入
2024 Q1：staking 总收入 ~$287M，Lido 收益 ~$28M

年化推算：约 $110–120M，高度依赖 ETH staking 活跃度和 ETH 价格

5.3 收入增长趋势
ETH staking 量逐年上升

stETH 在 DeFi 的广泛使用增加收益潜力（AAVE、Eigenlayer）

但也面临 Restaking 模式分流部分收益的风险

6. Valuation & Risk Analysis（估值分析与风险识别）
6.1 PE / EV / Revenue 指标
LDO 当前 FDV（Fully Diluted Valuation）超 $2B

PE-like ratio 高达 800–900 倍，明显高于传统 DeFi 项目（MKR、AAVE）

PEG ratio 接近 0.4–0.5，表明增长能部分解释高估值

6.2 DCF 粗估
假设 ETH staking 增长 30%，ETH 价格年增长 30%

折现率 40%，终值增长率 2%

得出理论估值为 ~$13.96/LDO（示意）

6.3 核心风险
治理高度集中，少数地址控制多数投票权

法律监管不确定（尤其是美方）

技术路线挑战（Restaking 与 LRT）

stETH 深度集中在几个协议，可能引发系统性风险

7. Conclusion & Investment View（结论与投资观点）
Lido 协议具备稳定收入、高增长特征

LDO 作为治理代币尚未参与分红，估值高度依赖“未来预期”

若 DAO 结构优化 + 分红机制上线，或有 re-rating 可能

适合长期看好 ETH 生态和 LSD 模式的中高风险投资者
