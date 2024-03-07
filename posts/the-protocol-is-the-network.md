# The Protocol is the Network

Here are some thoughts on how the IBC-verse, as a connected network of blockchains, might work in a future world where less public state is written to ledgers, and instead shorter-lived assets are transacted elsewhere, in a protocol or interop layer.

## IBC is the future, and it is a protocol not a network

In Cosmos, validators often talk about the IBC-verse, or Interchain. Generally, these are taken to be the set of IBC-enabled chains, a distinction that many of the teams involved expect to become more important over time than which chains are "Cosmos" chains in the truest sense - that is, built using the Cosmos SDK. 

Indeed, it might be that over time the two definitions merge, or it could be that new technology supercedes Cosmos and IBC is the technology that survives into the next generation of blockchains.

It's common to hear the phrase, "we're early" - and if this indeed is true then we should expect chains becoming zombie chains, or halting altogether, to be the long-term expectation. Without utility, chains will tend towards empty blocks and a dwindling user base. Though some might retain speculative value, the size of the IBC-verse suggests that there will be enough chains left with utility to present a better opportunity for investors.[0]

## What is a Cosmos chain anyway?

As we've discussed elsewhere, on podcasts and in blog posts, we expect the current definition of Cosmos chain to evolve from "built with Tendermint and the Cosmos SDK" to "uses IBC". In this context, it's worth thinking about what exactly that stack is composed of. Tendermint contains the ledger, consensus and networking stack, and the state machine is handled by the SDK. These two interact via ABCI (and its successors), and are intended to be loosely coupled.

In practice, they're pretty more tightly coupled, but as an architectural model to take forwards, it's bang on the money. If you push the state machine further up the stack, and ideally require as little knowledge about its workings as possible, you can derive interesting properties. You may exchange some knowledge of what your ledger might contain, relaxing some assumptions, while gaining the benefits of greater reusability. We'll return to this idea later.

## Privacy and public state

At present, state is kept on blockchains, mainly public ones, which presents a number of issues. Firstly a simple case of privacy - do you want your financial life to be online and public? As chain indexing technology improves, third-party institutions are mining this data for insights and to de-anonymise the nodes in the network, i.e. YOU. What this means in practice is that any economic utility you gain also has a side effect - a third party gains additional utility on top. Indeed, it may be that their actions are actively harmful to you, for example, impacting your credit score, or reducing your access to certain financial products, and thus your utility will go down as theirs increases.

Secondly, there is a case of cyberattack. A great deal of literature has been written on game theoretic models of theft within economies, and in many of these two variables become key to whether or not an attacker will decide an attack, or theft, is worth their while. Firstly, there is being able to identify the holder of a good. Kicking down random doors is not only unlikely to be profitable, but it also incurs risk to them (e.g. from the potential victim, authorities, law enforcement, etc). Secondly, there is being able to identify the size of a holding, which will inform how much benefit they could gain from a _successful_ theft.

Being able to identify a victim and their holdings vastly simplifies the process of identifying worthwhile targets, and increases the likelihood of theft.

Finally, this model doesn't even take into account trolling and griefing, or mass/mob action. It is purely a rational agent model.

These are just some of the reasons that public state on blockchains is likely to be harmful.

## What should the blockchain record?

In many cases, the blockchain as integrity source does not require public visibility - it merely requires that a proof of a transaction can be provided on request, usually between counterparties. Revealing only specific information to specific parties is a more sensible basic model for transactional use-cases. Consider that other truism that "wallets are social" - that is because wallets and accounts on the blockchain constitute identity, bringing with them all the complications and risks that entails.

When we consider the transaction itself, we might instead model the blockchain as merely taking a proof of an update to an asset. This proof could be a hash with no unencrypted data. The asset would live somewhere else, only accessible and visible to its current owner.

So where would that be?

If only the asset needs to be updated, it can be done in the protocol layer, i.e. the API client that is called to update the asset with its new owner. This state could be held locally (a software architecture question, really) in some kind of cache, or potentially even persisted to a blockchain or ledger. Note that as long as the API and its more ephemeral storage stayed up, then the asset would be available, even in this simple model (and it is easy to extrapolate extra ways of improving robustness).

Note also that the same API client could write to different ledgers or interface between them, depending on the plumbing and protocols available. Thus a payments system of this type, or asset management system, has more in common with the IBC protocol in some ways than the blockchains of the Cosmos ecosystem.

In this model, the state machine exists as effectively a separate network. It may be that nodes (or entities) running the state machine software also are validators, but that's not a requirement. As mentioned, they might run a state machine node and not persist its data anywhere - although that would then beg the question of why clients would connect to them as a trusted intermediary for resolving transactions.

These are all the principles behind CBDC systems currently being proposed by academics, such as the Comet (no relation to Comet BFT) system[1]. In Cosmos, we're uniquely positioned to understand how such a system could connect permissioned and permissionless blockchains and facilitate payments in future.

[0] Of course, in the long run, only projects with utility will be value. In any event, it is probably the case that for any transactional economic system investor returns and the correct functioning of the cryptoeconomy are incompatible
[1] [Read more about Comet and USOs](https://link.springer.com/chapter/10.1007/978-3-031-32415-4_38)
