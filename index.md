---
title: 1. Intro
layout: home
---

Yieldstream is a novel concept in the yield aggregation space that answers a question many of you have been asking yourselves in the last few years.
What if I could be my own curator? What if I could actually play around with defi's money legos directly without having to rely on the decisions of third parties in my yield generation activities? What if I had access to an endless amount of options in Ethereum's infinite garden?

Yieldstream is the answer to that question.
Yieldstream will free you from defi's current constraints by allowing you to take your yield generation strategy into your own hands through it's flexible yield aggregation infrastructure, unlocking an endless amount of possibilities and allowing you to package them into a highly flexible ERC-4626 vault that you can modify over time as you please.

But Yieldstream is not just another yield aggregator.
Yieldstream goes a step further by completely reimagining the way yield is aggregated through the introduction of a decentralised rebalancing mechanism and through the concept of liquidity caps.
This approach allows you to engage in highly granular capital management without having to engage with the rebalancing process as the open market works on your behalf to optimise your returns through Yieldstream's onchain revshare mechanism.

Yieldstream's decentralised rebalancing process modernises the yield aggregation concept by bringing the entire process on-chain removing the reliance on off-chain components.
The Yieldstream rebalancing process achieves this by allowing the open submission of rebalancing requests to any operational Yieldstream vault in exchange for a slice of the yield that the underlying vault generates for the lifetime of a proposal with the revshare rate being chosen by the vault owner upon deployment.

The Yieldstream framework allows vault deployers to exercise full control on the market selection layer and is highly flexible as it allows deployers to add and remove markets over time but the decentralised nature of the rebalancing process creates the need for a more granular risk management framework so Yieldstream goes a step further by adding a second layer of control through the liquidity cap mechanism.

The liquidity cap feature allows vault deployers to set up limits on the rebalancing process by providing them with the ability to impose tvl% caps on an adapter by adapter basis.
For example a user that operates a vault which allocates liquidity to the btc/usdc, eth/usdc and mkr/usdc markets of Morpho's Base deployment might choose to impose a 20% tvl limit on the mkr/usdc market barring strategists from allocating more than 20% of the vault's tvl into the mkr/usdc pool.

Apart from the above features Yieldstream vaults offer another feature that enables them to stand out from the crowd. That feature is called the invariant and acts as an additional layer of security for Yieldstream users.
The invariant checks out the underlying markets and acts as a circuit breaker in the case of losses by blocking deposits in the affected adapter while the vault owner is then able to call the rescue function in order to pull out the affected deposits.

Yieldstream is a completely new approach in the yield aggregation space.
If you always wanted to become your own curator Yieldstream will allow you to do exactly that.
We are launching soon on top of Morpho's Base deployment and you are free to join us in this journey as the Yieldstream platform is entirely permissionless. No admin keys. No gatekeepers. No bullshit.
