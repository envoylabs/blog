---
layout: default
---

# (de)NS Roadmap

![deNS](https://raw.githubusercontent.com/envoylabs/blog/gh-pages/assets/messages.png)

Now that we're on mainnet, it's time to define a rough roadmap for what's to come. 

We're about to release some minor fixes, that allow for experimental things like messaging via message memos (caveat: we have no idea if this will scale).

Regardless, we have a rough idea that the roadmap will be (in order):

1. Work out if we can help Keplr support CW721 NFTs (and thus the nameservice names)
2. Any work required for DAODAO to integrate (i.e. DAOs & contracts managing base tokens)†
3. Transferring names you own to another wallet
4. Minting of subdomains (paths) - these are free to the owner of the base token
5. A marketplace for names and paths you own
6. Expanded profile pages with txs etc. for names
  * For validators, this will show staking info & allow you to stake
  * For contracts, it will show contract meta
7. A name can reference a blob of data on IPFS (this could be yr website, app, or something else - see 8, below)
8. Some boilerplate contracts to allow for things like e.g. selling music that is held as files at a subpath
9. Better hooks and UI for messaging
10. Private messaging (with the caveat that this should be thought of as more like email than instant messaging)

† with the critical difference from [elsehow's blog post](https://nickmerrill.substack.com/p/naming-could-be-rad) being that nobody other than the current owner of a name can burn, transfer or send a name - there is no central authority, and at present that _also includes the base token_. They can point it at things without transferring ownership, if they want to maintain control over a base token, or sub path.

Obviously all of this is subject to change, but that's where we are right now.

As always, you can get in touch via the `#name-service` channel on the [Juno Discord](https://discord.gg/wHdzjS5vXx), or tweet us [@decentralizedns](https://twitter.com/decentralizedns).

We've said before that this was very much a side project, and we're blown away and a little humbled by the response it's gotten.

We had originally a quite different roadmap in mind, as we assumed we would have a very small initial user base - but it's bigger than expected, and you've told us that Keplr is the priority - so we've switched things around, as the list above shows.

All that remains to be said is thanks to everybody that's checked it out and thinks it's cool. It's very early days for projects like this in the Cosmos, and hopefully it will develop into something really cool, with your support!
