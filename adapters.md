---
title: 5. Adapters
layout: home
---

## Yieldstream Adapters

Yieldstream adapters are the essential connectors that enable vault tokens to seamlessly interact with external projects and markets.
Acting as the bridge between the vault and the DeFi ecosystem, adapters facilitate key functionalities that ensure smooth and efficient integration with external protocols.

### Core Functionality

Yieldstream adapters are built on a generic adapter interface, which defines a standardized set of functionalities, including:

- `maxWithdraw`: Determines the maximum amount of assets that can be withdrawn at any given time.
- `maxDeposit`: Defines the upper limit for deposits into the adapter.
- `totalAssets`: Tracks the total value of assets managed by the adapter within the external market.
- `deposit`: Allocates tokens from the vault to the target external market.
- `withdraw`: Retrieves assets from the external market back into the vault.

These core functionalities provide a consistent and predictable way for vaults to interact with various markets, ensuring interoperability and ease of use.

### Market Integration

One of the standout features of Yieldstream adapters is their flexibility to integrate with any market that supports atomic transactions. This means:

- Any DeFi protocol with transaction mechanisms that complete in a single operation can be integrated.
- Users can deploy vaults connected to a wide range of markets, from lending protocols to liquidity pools, based on their strategy.

### Strategy Execution with Adapters

Adapters play a critical role in the execution of vault strategies:

- Tokens deposited into the vault are distributed across external markets via adapters, based on the active strategy.
- The modular nature of adapters allows users to update or replace them, enabling dynamic strategy adjustments as new markets or opportunities arise.

### Developing and Registering Adapters

Yieldstream encourages innovation and community participation in expanding its ecosystem:

**Creating Custom Adapters**:

- Developers can implement the generic adapter interface to create custom adapters for new markets.
- The standardized design ensures compatibility with the Yieldstream protocol.

**Registering Adapters**:

- Once developed, adapters can be submitted for inclusion in the Yieldstream registry, making them available for use by all vault deployers.

### Benefits of Yieldstream Adapters

- **Flexibility**: Adapters allow vault deployers to target diverse markets, maximizing yield opportunities.
- **Standardization**: The generic interface ensures consistency across all adapters, simplifying the user experience.
- **Innovation-Friendly**: Yieldstream’s open architecture encourages developers to create and contribute adapters, expanding the ecosystem.
- **Dynamic Allocation**: Adapters enable real-time, strategy-driven allocation of assets across markets.

### Example Use Case

A Yieldstream vault targeting stablecoin markets might utilize adapters for:

- A lending protocol offering USDC/DAI pools.
- A decentralized exchange providing high APY on USDC/USDT pairs.
- The vault owner uses these adapters to dynamically allocate funds to the most profitable pools while maintaining risk limits.

Yieldstream adapters are more than just connectors—they are the engine driving interoperability and innovation in the protocol. With their modular design and broad compatibility, adapters empower users to curate strategies that adapt to the dynamic DeFi landscape. Whether you're leveraging existing adapters or creating new ones, Yieldstream adapters are the key to unlocking the protocol's full potential.
