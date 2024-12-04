---
title: 7. Liquidity Caps
layout: home
---

## Yieldstream Liquidity Caps

Liquidity caps provide Yieldstream vault owners with an additional layer of control over the rebalancing process, enabling tailored risk management strategies. By setting constraints on how much of the vault’s total value can be allocated to specific markets, liquidity caps ensure that vault owners maintain oversight and reduce exposure to any single market or adapter.

### Key Features of Liquidity Caps

**Customizable Risk Management**:

- Vault owners can define allocation limits for individual markets, tailoring their exposure based on risk tolerance and strategy preferences.

**Flexible and Modifiable**:

- Liquidity caps can be configured during vault deployment or at any time post-deployment.
- Vault owners have the freedom to adjust, add, or remove these caps dynamically, responding to changing market conditions.

**Optional Constraints**:

- The use of liquidity caps is entirely optional. Vault owners may choose to impose them on specific markets, apply them broadly, or avoid their use altogether.

### How Liquidity Caps Work

Liquidity caps are set on an adapter-by-adapter basis and define the maximum percentage of the vault’s total value (TVL) that can be allocated to a particular market. These constraints are enforced during the rebalancing process, ensuring that strategists submitting proposals adhere to the defined limits.

### Example Use Case

A vault owner operating a USDC vault with exposure to the BTC/USDC, ETH/USDC, and MKR/USDC markets on Morpho's Base deployment might:

- Decide to limit exposure to the MKR/USDC market to 20% of the vault’s TVL to mitigate risk from volatility in that market.
- Set no caps on BTC/USDC and ETH/USDC, allowing unrestricted allocations to these markets.

In this scenario:

- Strategists submitting rebalancing requests must ensure their proposals do not allocate more than 20% of the vault’s TVL to the MKR/USDC adapter.
- If the market conditions change, the vault owner can adjust the cap, remove it entirely, or impose new constraints on other markets.

### Strategist Compliance with Liquidity Caps

- Strategists must account for liquidity caps when formulating rebalancing requests.
- Proposals that exceed the defined caps are automatically invalidated, ensuring vault owners’ constraints are always respected.

### Benefits of Liquidity Caps

**Enhanced Control**:

- Vault owners gain granular control over market allocations, reducing the risk of overexposure.

**Dynamic Adjustments**:

- Caps can be modified in real-time, allowing vault owners to react to market developments or changes in their strategy.

**Tailored Risk Profiles**:

- Vault owners can define unique risk profiles for their strategies, balancing yield potential with security.

### Setting Liquidity Caps

**During Deployment**:

- Vault owners can configure liquidity caps as part of the initial deployment process via the Yieldstream vault factory.

**Post-Deployment**:

- Caps can be added, adjusted, or removed at any time using the protocol’s management tools, giving vault owners full flexibility.

Liquidity caps offer Yieldstream vault owners a powerful tool to implement precise risk management while maintaining the flexibility to adapt their strategies as needed. Whether used broadly or selectively, liquidity caps ensure that vault owners retain full control over their asset allocations, creating a safer and more robust environment for yield generation.
