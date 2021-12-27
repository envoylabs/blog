---
layout: default
---

# Decentralized Name Service on Juno

For the last month or so, we've been leading the development of a name service that can be deployed via a CosmWasm smart contract, which we call (de)NS for short. It will be launched in a phased way this January on Juno's mainnet.

Whereas other systems like ENS and Terra seem to have spent a lot of time on the mechanics of selling and auctioning, we kind of think that stuff is a waste of time. (de)NS instead focuses on using a known interchain primitive to form a portable bearer ID - the NFT.

Names (think, usernames or domains) are charged for once. There is a cap on the number that can be owned, to avoid hoarding.

Obviously, there are ways that a malicious entity can get around that. For version one, we'd like to launch and see how users in the wild use the service and respond to it.

Users can sell or transfer their name NFT as they see fit, meaning that in time it should even be transferable via IBC.

That said, just as DID is not yet ubiquitous, it's not quite clear how this mechanism will function, especially in terms of guaranteeing the uniqueness needed for general-case addressability. It's currently not something that has been comprehensively solved in the space, in our opinion.

Probably, a third party oracle or decentralized name chain is needed for that. Incidentally, we might have a longer-term solution, but more on that later if we have the time to tackle it.

By writing an extended NFT contract with some additional indexing, you can make the nameservice mapping as simple as looking up the owner (address) of a domain or username.

To go the other way, you simply look up what domains or usernames an address has.

We allow users to set a primary alias. This links their wallet address 1-1 to an NFT name record, until they burn, or transfer the NFT or re-set the value.

What this means is that other smart contracts can do a lookup against (de)NS via a WASM message to see if any user interacting with their contract has a username configured as their preferred alias.

It seems very minor, but it's a small ergonomic improvement from where we are today, and should benefit users of other Juno dApps.

That's not all though. We have a lot of exciting ideas on our roadmap, like:

- dereferencing contracts
- a graph index of entities
- sliding privacy controls for certain meta
- web2 APIs
- web of trust functionality

However, we're a very small team, so things will take a bit of thought and time before they can be built. On that score, thanks to the other contributors on the project - `ekez`, `danwlsn` and `elsehow`, you're all legends.

If you'd like to check in on development, or have ideas, then say hey on the Juno Discord.

We're hoping to have it up and ready to test on the uni testnet by the end of the month, so stay tuned.
