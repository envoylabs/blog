---
layout: default
---

# Unity Prop Smart Contract

There are two actors that can take actions using this smart contract: **the withdrawer** and **the governance module**.

So let's dig into those a bit.

## The Withdrawer

Here's a diagram of actions available to this entity:

![Withdrawal actions](https://raw.githubusercontent.com/envoylabs/blog/gh-pages/assets/withdrawal_actions.png)

The withdrawer is simply an address that has permissions to initiate a withdrawal to a withdrawal address.

- The withdrawal address is configured when the contract is instantiated
- It must be the same address as the address initiating the withdrawal
- When a withdrawal is initiated, there is a delay until the funds can actually be withdrawn
- This will be set to 28 days

In order for this contract to be useful for mediating between CCN and the community then, it will have to be set up:

- So that a CCN address is the withdrawal address
- So that the delay is set to 28 days

Finally, CCN's funds will have to be moved to the contract balance. This can be done:

- Voluntarily (CCN sends funds)
- Via an upgrade (i.e. Unity/Prop 18)

The reality is that even with CCN's consent, their funds would need to be unstaked and sent to the contract with an upgrade handler. Allowing CCN to unstake their funds and send manually would be too risky.

## The Governance Module

Here's a diagram of actions available to this entity:

![Governance Module actions](https://raw.githubusercontent.com/envoylabs/blog/gh-pages/assets/gov_actions.png)

The governance module is the part of the Cosmos SDK that handles on-chain governance. It can control the contract via the `sudo` entrypoint.

There are three actions available to governance, if a proposal passes with the correct message type (i.e. JSON encoded arguments).

1. Burn all funds held by the contract
2. Send native funds to an address (in this case, Juno)
3. Send all funds held by the contract to an address

The contract then checks the message type sent to it, and acts accordingly.

Cases 1 and 3 should need no explanation; they effectively drain the contract.

However, it is point 2 that allows for more flexible negotiation.

Although heavy on admin, there is no reason why X amount of Juno could not be released in chunks, if a compromise between CCN and the community was reached.

## A note on admin

The current plan is that the contract will be instantiated **with the governance module as its admin.**

This means that the code could be migrated (i.e. upgraded) with a further governance prop, if the community passed a motion to do so.

It may, however, be preferable to instantiate it without an admin. This means that the code cannot be upgraded.

This removes potential leverage to change the contract via out-of-band means (i.e. additional distraction or stalling props).
