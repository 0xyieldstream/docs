---
title: 5. Adapters
layout: home
---

Yieldstream adapters form the basis for making tokens of a Vault available in an external project and offer basic functionalities for interacting with it.
A generic adapter interface has been created that implements basic functionalities (e.g., maxWithdraw, maxDeposit, totalAssets, deposit, withdraw).

In principle, any type of market that provides atomic transactions can be integrated using adapters.
Tokens in the vault are distributed to the respective markets based on the currently active strategy.
