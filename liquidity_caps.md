---
title: 7. Liquidity Caps
layout: home
---

The Yieldstream liquidity caps offer a secondary layer of control to the Yieldstream vault owner by allowing the owner to set constraints in the vault rebalancing process based on their own risk management framework.

The liquidity caps are entirely optional and can be set on an adapter by adapter basis by the vault owner.
On top of that they are entirely modifiable and can be changed at will by the vault owner on the fly.

For example a Yieldstream vault owner might operate a Yieldstream vault that provides usdc liquidity against the btc/usdc, eth/usdc and mkr/usdc markets of Morpho's Base deployment.
The vault owner might decide to limit their exposure to the mkr/usdc market to 20% of the vault's tvl.
This is possible through the use of liquidity caps.

These liquidity caps can be imposed by the vault owner during the vault deployment process or at any point in time later down the line.
The vault owner can always modify or remove these constraints as they wish.
Strategists will have to take these constraints into account when submitting rebalancing requests.

Vault deployers can set these constraints on any adapter of their choice whenever they choose to do so.
The liquidity caps are not necessary and the vault owner might choose to completely avoid their use or impose them only on specific markets.
