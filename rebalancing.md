---
title: 6. Rebalancing
layout: home
---

## Yieldstream Rebalancing

The Yieldstream rebalancing process is the cornerstone of the protocol, enabling dynamic and decentralized optimization of yield strategies. By operating entirely on-chain, Yieldstream eliminates the need for off-chain infrastructure, ensuring transparency, security, and open participation.

### Overview of Rebalancing

The rebalancing process allows strategists to submit proposals that adjust a vault's allocation of assets across supported markets. These proposals are evaluated and executed entirely on-chain, ensuring a seamless and trustless process.

### Rebalancing Requirements

For a rebalancing request to be considered valid, it must meet the following criteria:

**Whitelisted Markets**:

- All proposed markets must belong to the list of markets approved by the vault owner during the vault’s configuration.

**Minimum APY Improvement**:

- The proposal must deliver an APY improvement that satisfies the minimum threshold set by the vault owner at deployment.

**Liquidity Caps**:

- The proposed allocations must respect the liquidity caps defined by the vault owner for each market, preventing overexposure.

As long as these requirements are met, the rebalancing request will be approved and executed.

### How Rebalancing Works

**Submission**:

- Strategists send a rebalancing request to a Yieldstream vault, specifying the desired reallocation of assets.

**On-Chain Evaluation**:

- The vault calculates the actual APY improvements, considering potential fluctuations caused by the rebalancing itself.
- These calculations use the interest rate curves of the underlying markets to estimate post-rebalancing yields.

**Execution**:

- If the request meets all requirements, the vault reallocates its assets according to the proposal.

**Strategist Rewards**:

- Strategists whose proposals are executed successfully earn a share of the vault’s yield.
- The reward rate is determined by the revshare rate, which is configured by the vault owner and can be updated over time.

### Key Features of Rebalancing

**Fully On-Chain**:

- The entire process, from proposal submission to execution, takes place on-chain, ensuring transparency and eliminating reliance on off-chain infrastructure.

**Permissionless Participation**:

- Anyone can submit a rebalancing request, fostering an open and competitive environment for yield optimization.

**Dynamic Yield Optimization**:

- The protocol continuously adapts to market conditions, maximizing returns while adhering to vault-specific constraints.

**Flexible Incentives**:

- Strategists are rewarded based on the duration and performance of their active proposals, ensuring alignment with the vault’s goals.

### Configurable Parameters

Vault owners have several tools to customize the rebalancing process:

**Whitelisted Markets**:

- Define the list of markets eligible for rebalancing to align with the vault's strategy.

**Minimum APY Threshold**:

- Set the minimum APY improvement required for proposals to be considered.

**Revshare Rate**:

- Determine the share of yield allocated to strategists, balancing incentives and vault profitability.

**Liquidity Caps**:

- Set allocation limits for each market to manage risk and maintain diversified strategies.

### Example Workflow

1. A strategist identifies an opportunity to improve a vault’s yield by reallocating funds between ETH/USDC and DAI/USDC markets.
2. The strategist submits a rebalancing request proposing a new allocation while ensuring it respects the vault’s whitelisted markets, minimum APY improvement, and liquidity caps.
3. The vault evaluates the proposal on-chain, considering potential APY changes due to rebalancing.
4. If approved, the vault reallocates assets, and the strategist earns a share of the vault’s yield as long as their proposal remains active.

The rebalancing process is a testament to Yieldstream’s commitment to innovation, decentralization, and user empowerment. By enabling anyone to participate in optimizing vault strategies and automating the entire process on-chain, Yieldstream sets a new standard for efficiency and transparency in DeFi yield aggregation.
