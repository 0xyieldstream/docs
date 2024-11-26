---
title: 6. Rebalancing
layout: home
---

The Yieldstream rebalancing process is the central innovation behind the Yieldstream protocol as it functions entirely on-chain through the use of a decentralised and open process that anyone can participate in, removing the requirement for the use of any off-chain infrastructure.

Anyone can send a rebalancing request to any Yieldstream vault of their choice as long as the request satisfies the following requirements:

1. All the markets involved in the request must belong in the list of the owner's whitelisted markets based on their vault configuration

2. The apy improvement satisfies the minimum improvement requirement set by the vault owner during the vault deployment process

3. The allocations proposed by the strategist's rebalancing request respect the allocation caps set by the vault's owner

A rebalancing request will go through as long as the above requirements are being met

The entire rebalancing process takes place entirely on-chain.
The Yieldstream vault receives the rebalancing request and proceeds to calculate the actual apy's of the proposal by taking into account the apy fluctuations that will be caused by it's own rebalancing activity based on the interest rate curves of the underlying markets.

The strategists that submit successful rebalancing requests get rewarded for doing so by receiving part of the yield that the underlying vault generates for as long as their proposals are active. The rewards are calculated based on the underlying vault's revshare rate which is set by the vault owner and can be modified over time.
