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

<img width="3532" height="1919" alt="image" src="https://github.com/user-attachments/assets/7dadacf9-7a1e-4067-b1a4-ee693d2307b3" />


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
Lido controls approximately 8.9–9.0 million ETH staked, representing 24–25% of Ethereum’s staking market as of August 2025. Despite falling from a peak of over 30%, Lido remains far ahead of any individual competitor. Its dominance is driven by first-mover advantage, deep liquidity, and seamless DeFi integrations.

That said, the trend is shifting. Community-led efforts to decentralize staking, paired with the rise of viable alternatives, have caused Lido’s relative share to slip. Nonetheless, its absolute stake volume continues to grow alongside Ethereum’s total staking base, now surpassing 36 million ETH.

📊 [Insert: Ethereum staking market share pie chart – Lido vs others]


### 3.2 Competitor Landscape
Coinbase (cbETH) offers a centralized staking service with a focus on retail accessibility. While cbETH is transferable and earns yield, it lacks deep DeFi integration and poses custodial risks. It holds ~2.4M ETH (~6–7% market share).

Rocket Pool (rETH) emphasizes decentralization with hundreds of permissionless node operators. Its ~700k ETH stake (~2% share) is modest but growing. rETH is non-rebasing, DeFi-integrated, and community-driven—attracting users prioritizing decentralization over scale.

Ether.fi (eETH) rapidly gained ~7% share by promoting restaking and non-custodial control via NFT-based credentials. With 2.5M ETH staked, it represents the most successful challenger of 2024–2025. Its appeal lies in high yield, user sovereignty, and airdrop incentives, though questions remain about its validator decentralization.

Frax (frxETH/sfrxETH) employs a two-token system separating liquidity from yield. While small in market share (~0.3%), Frax has made notable design contributions and remains a favorite for DeFi-native strategies.

Mantle (mETH/cmETH) entered the market with a double-yield model backed by BitDAO’s treasury. Its adoption is still early stage, appealing mostly to advanced users within Mantle’s Layer-2 ecosystem.

Additionally, players like Binance, Kraken, and SSV Network round out the landscape. While centralized exchanges retain market share (~8%), infrastructure projects like SSV aim to decentralize validator architecture, which Lido is also exploring through its Staking Router and DVT modules.

📊 [Insert: Comparative table – stETH vs rETH vs cbETH vs eETH etc.]

3.3 Decentralization, Regulation, and Moat
Lido’s dominance has drawn criticism over centralization. The DAO controls validator selection (currently ~30 operators), and large LDO holders exert considerable influence over governance. To address this, Lido has introduced dual governance (allowing stETH holders to veto proposals) and is testing DVT systems for more distributed validator control.

From a regulatory standpoint, the outlook has improved. In August 2025, the SEC clarified that liquid staking tokens like stETH and rETH are not securities, recognizing them as technical staking receipts rather than investment contracts. This has removed a significant overhang from U.S. market participants.

Despite this, governance tokens like LDO are still under observation. While Lido does not distribute revenue to LDO holders, future fee-sharing mechanisms could raise regulatory questions. For now, Lido’s DAO remains legally unincorporated, governed by tokenholders and executed via multisig.

Finally, Lido’s moat remains strong. Its liquidity depth, early integrations, and DAO treasury continue to give it an edge. stETH is the default in many DeFi applications, and Curve’s stETH/ETH pool alone regularly handles massive volumes with minimal slippage. Competitors may offer better decentralization or yields, but replicating Lido’s ecosystem entrenchment will take time.

👉 [Insert regulatory timeline or summary of key enforcement events here]

4. Tokenomics & Distribution（代币经济模型与分配结构）
4.1 供应机制
固定总量：1,000,000,000 LDO

当前流通：约 890–900M（90%），无新锁仓计划

没有增发机制（通缩或回购机制未明确）

4.2 初始分配 vs 当前结构
初始分配：DAO Treasury（36%）、早期投资人（22%）、团队（20%）、节点（6.5%）、挖矿激励（15%）

当前结构（参考 Dune）：大部分已解锁，Treasury 持币仍占比较高；治理投票活跃地址少

4.3 DAO Treasury 管理现状
Treasury 地址仍持有约 100M+ LDO

用于未来激励、流动性支持、生态资助、运营成本

可构成估值锚点之一（“账上资产”）

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
