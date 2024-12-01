---
title: 8. Invariants
layout: home
---

Invariants are fundamental safeguards within the Yieldstream protocol, ensuring the health and integrity of the system at all times.
These critical checks monitor key properties that reflect the state of the protocol and its interactions with external markets.
By leveraging invariants, Yieldstream is able to detect anomalies, mitigate risks, and protect user funds through automated responses.

## What are invariants?

In the context of Yieldstream, invariants are predefined rules or properties that must always hold true for the protocol to operate correctly. They act as real-time monitors for critical metrics, ensuring that:

1. The protocol functions as intended.
2. User assets are safeguarded from malicious or unforeseen events in external markets.
3. Risk is minimized by triggering corrective measures when necessary.

## The lending market invariant

A prime example of an invariant within the Yieldstream protocol is the lending market invariant.

1. **Purpose**

- This invariant ensures that the total value of funds in an external market can only increase due to interest payments made to depositors.
- This invariant guarantees that the protocol’s health is preserved by preventing any external manipulation or malfeasance from impacting user funds.

2. **How it works**

- The protocol continuously monitors the total value recorded in an external market compared to the deposits made by the vault.
- If the external market value ever drops below the deposited amount, the invariant is considered broken, signaling a potential malicious act or critical failure in the external market.

3. **Response to broken invariant**

- The protocol immediately switches the affected market to recovery mode.
- In recovery mode:
  - No further deposits are allowed into the market.
  - The remaining funds are queued for withdrawal.
  - As soon as any user interacts with the protocol, the funds are automatically withdrawn and secured back within the vault.
- This mechanism ensures a rapid and automated response to protect user assets.

## Recovery Mode in Action

For example:

- A vault deposits $1,000 in a stablecoin lending market.
- Over time, the value in the market should either remain at $1,000 or increase due to interest accrual.
- If the market suddenly reports $950, the lending invariant is triggered.
- The protocol immediately halts all interactions with the market and switches it to recovery mode.
- During the next user transaction, the $950 is withdrawn and returned to the vault, preventing further losses.

## Benefits of invariants

- **Enhanced Security**: Automated monitoring and response mechanisms reduce the reliance on manual oversight.
- **User Protection**: Safeguards user funds by mitigating risks from malicious acts or unexpected market conditions.
- **Protocol Integrity**: Ensures that Yieldstream operates as intended, even under adverse circumstances.
- **Trust and Transparency**: Builds user confidence by providing a robust framework for risk management.

Yieldstream's invariant framework will continue to evolve, incorporating new checks and improving its response mechanisms as the protocol grows.
By staying vigilant and adaptive, Yieldstream ensures that it remains a secure and reliable choice for yield aggregation in the DeFi ecosystem.
