---
layout: default
---

# Okay, code is law. What next?

A self-indulgent look at where we are with on-chain governance, and maybe where we are going.

## TL;DR

This article explores a number of questions that we as an interchain have to answer.

- Is code law? If it is, then there is an implicit power structure. Are developers and validators a check-and-balance on the electorate?
- Who is responsible for the actions of a DAO?
- Traditional political parties are struggling to adapt to a multipolar world; is the interchain a regressive or progressive influence?
- Who owns the interchain anyway? How will governance for projects and DAOs evolve?

It's worth saying that these are _just our opinions_, and are obviously based on a particular interpretation of broad economic and historical trends.

This blog is split into 4 parts:

1. **Is code law? The implications of Juno Prop 16**, a discussion of how Prop 16 has highlighted some of the implicit governance parallels that may exist on Cosmos chains
2. **Multilateralism and decentralization**, a very un-academic musing on whether decentralized systems are part of a wider discourse of multilateral political struggle
3. **Vector capitalism and ownership on the interchain**, some thoughts on how networks where payments are built-in offer chances for agency and ownership, but also risk accelerating vector capitalism
4. **Conclusion**

___

## I: Is code law? The implications of Juno Prop 16

Most systems of government have a number of moving parts. But let's design a toy one.

It might have:

- Laws
- A judiciary to make judgements based on the law
- An electorate to pass laws

Okay, so far, so good.

So, in Cosmos governance, what do we have? Well, let's try to line it up.

- Laws: code
- Judiciary: ???
- Electorate: stakers

Okay, so where do validators and developers fit into this model? Because changes to code require their input.

As an aside, this is also part of the increasing mood in the Cosmos that governance proposals that require a software change should only be submitted with the code. This means that the intention is clear, the desired change to the 'Law' enumerated in full, and the work already done by engineers who are happy to implement it, which is important, because of the question of liability.

On liability, then. Engineers and validators are much more visible, and are thus taking on much higher risk to themselves in implmenting a proposal that is controversial or may draw regulatory ire. This is doubly complicated if they don't agree with the decision. What are they to do in that situation?

Purists would presumably argue that DAO governance supersedes their personal opinion, except that's... obviously un-enforceable in practice.[0]

Making sure that code is presented alongside any governance proposal is a good counter to this. It's also why many engineers associated with Juno voted no on Prop 18. The question was, who is going to implement this?

If it is unclear who will write the code, test the code, and get it merged, then the proposal is un-enforceable as written.

This, of course, was also a problem for Prop 16, where in practice, as written, it was incredibly difficult to see how it could get implemented, tested and approved, let alone actually run by the validator set.

Which brings us to the final missing piece of this imaginary system: validators.

We propose that the way they acted in the Prop 16 scenario was akin to that of an upper house, by checking what was seen as an overreach of interpretation on an unworkable proposal.

Many validators wrote long-form judgments on Prop 16 (much like you would expect from a judiciary) to back up their positions, but the net effect was that validators brought the conversation back to the table for a compromise that _was workable_.

That's sort of like a high court or supreme court in function, if you kind of squint.

Now, this compromise might not be considered ideal by anyone, but it is broadly palatable to all, **and that's often the sign of a compromise**.

In that sense, perhaps the dramatic back-and-forth on Prop 16 _is simply governance working as intended_, where validators and developers act as a check on the pure power of the electorate.

If this is the case, then any formal acknowledgment of the shape of Cosmos governance should likely take this into account, as this implicit check on governance shocked and angered many.

However, should the same situation arise tomorrow on another chain, it would be likely to pan out in a very similar fashion.

### Can governance scale?

Okay, this could be literally a book in its own right, but the implications of the exact technical mechanism by which voting occurs deserves a little attention.

This has its own header, purely so that some quick observations can be made:

- direct democracy is hard to scale
- a wallet is not one person, or entity
- yes/no/abstain is a quite coarse voting system
- no with veto will become a common blocking mechanism as knowledge of the mechanics matures

So clearly our governance systems on-chain are going to have to get more sophisticated.

At a bare minimum, that means upgradeable governance. This is currently possible via the SDK, but there's a broader conversation to be had whether better systems than dPoS exist, and are within our near or mid-term reach.

It's our bet as an organisation that IBC is the technology from Cosmos that will 'make it', but all other bets, long-term, are off, as they say.

### A diversion into liability

Where the rubber will hit the road on these governance systems will be liability, as we've seen with Prop 16. Sooner or later, something that is very controversial, possibly illegal, will happen across multiple jurisdictions where regulators are motivated to act.

Who they target, what their reasoning is, and how successful that enforcement action is, will be a watershed moment for the maturity of on-chain governance and DAOs in general.

___

## II: Multilateralism and decentralization

To indulge a stock pet theory, the primary political battleground is becoming fought on a unilateral versus multilateral playing field. Not, necessarily 'left' and 'right', although there is some overlap.

Many others have expressed this in one form or another during the last ten years, as the implications of the 2008 banking crisis have shaken out.

_Decentralized systems are inherently multilateral._ Though some context as to why this is important from our lived political experience may be relevant.

At least in the UK, for the last hundred years the primary political axis has been that of Socialist (via the Labour Party and movement) versus Conservative (via the Tories). The effectiveness of the Conservative narrative of needing no change (essentially the entrenchment of the interests of the ruling class)[1] is such that the Conservatives (Tories) were in power in the 20th Century United Kingdom for longer than the Communist Party in Russia.

In the last thirty years, the driving force for multilateral action has been international finance and the forces of globalisation - often a regressive, or malign influence as experienced by ordinary citizens.

This cannot be countered easily by traditional political parties that conceive of the world in a unipolar way, the so-called 'One Nation' Conservatives, or Labour movements that are inherently anchored to a place. How do you regulate international companies and forces that are not tied to a place?

If you're jumping ahead and going 'hang on, that sounds like crypto', then put a pin in that thought.

At a time when manufacturing has already largely fled, in any case, the meaningful experience of most working-age people is very far removed from a 'working class' as experienced since the dawn of industrial capitalism, and into a series of much more fragmented class experiences based on economic precarity.

Thus, should a political movement, be it socialists, or the Pirate party, want to effectively argue their case, they must re-evaluate both their constituents and the battlefield they are fighting on.

Both the Green movement and the Pirate movement have seen this first-hand. Both of these movements are also inherently multilateral, as they are set up to fight something (the destruction of the planet, and international copyright and censorship) that is also multilateral, or cross-border in nature.

Socialist movements, on the other hand, often try to fight the corrosive influence of international capital (for example, large-scale criminal tax evasion) on a country-by-country basis. That isn't going to work, as we've seen time and time again.[2]

Fighting these things in just your city, state, country, is not enough. It is no coincidence that both the Greens and Pirates have had much of their initial success working in this fashion, in for example the European Parliament.

One nation Conservatives are still effective at fighting these multilateral progressives purely because their stock argument of "no change is needed" will always appeal to some, not because it is a meaningful reflection of our current reality.

Conservative movements are quicker to adapt to these changing currents, in general. As they represent the wishes of the ruling class, the most effective conservative cliques are able to simply subsume the incoming competitor class.

This happened with landowners and capitalists, and there's no reason to think an accommodation won't be made to either the vector class, or any elite classes that follow.

Even in crypto, this can be seen in wealth management becoming alive to Bitcoin, and increasingly becoming interested in novel coins and gen2/3 blockchain projects.

So it seems the question is, **whether the crypto space is an accelerating, or purer form of these already existing regressive trends**, or **whether it is part of the balancing of the axis against regressive multilateralism that harms people, individual and collective agency and the planet**.

___

## III: Vector capitalism and ownership on the interchain

It's at this point that, if you're familiar with McKenzie Wark's _Capital is Dead_ you will probably be spotting elements of their central argument.

Much of the technological change that has resulted in our multilateral political present was an attempt by capitalists to bypass labour, using communication technology as a way of globalising their workforces and supply chains.

That has had far reaching impacts, culturally, politically, socially, technically, and many of them overlap pretty heavily with the discussion of multilateralism. Simply put - all of these changes have happened across borders, even if the individual cause and effect you might clearly see (Trump, Brexit, stagnant real wages etc etc) are often seen though the lens of an individual country.

Anyway - what's important here is that vector capitalism assumes that the information vector, rather than the means of production, is where excess value is created, through "any surplus information, acquired through unequal exchanges of information."[3]

The question is, on the interchain, who owns that?

The obvious answer is 'the whole chain' or 'no one', if the code is open-source, as is common among these projects.

However, the answer is more subtle - which is that programs in practice are divided into a runtime and state. The state, i.e. the data, remains where the "surplus information" is to be found, and that's the same on web2 and the interchain.

So, back to our interchain, and our governance, why should we care about this?

The question comes back to ownership. On web2, everything is free, and everything is owned by massive corporations as the result of an "unequal exchange of information." On the interchain, paying for things is commonplace, which is why advertising as a revenue model is redundant, laughable even.

However, it's important to as a user consider how vendor lock-in works. Whether an admin of a contract can burn your NFT, for example, or what ability you have to move it elsewhere.

Perhaps, even if you have little agency over the data in a practical sense, that's a reasonable trade-off for not having your data bought, sold and held by huge international corporations. However, it's naive to think that as dApps scale in size and value that these projects will not also trend a certain way.

This ability to pay for things easily on the interchain means we can radically re-think the way that vector capitalism has shaped the world via the internet, but it requires a conscious effort to do so.

Some of these initial questions for the end user start off very simple.

In short: how fully do you own the things that you've paid for? Doubly so, since they are just data.

Put simply - you've paid for it, to what extent do you actually own it? Are applications on-chain capturing a reasonable excess for their work, or are you still experiencing an asymmetrical output?

This applies at chain level too - and perhaps is the root of a lot of the anger at the whale. Such a huge holder fundamentally unbalances a chain. However, looking at the valset, as Nick Merrill did in _Minority Rule is Possible_ reveals that validator voting power distribution suggests (potentially fundamental) issues with dPoS.[4]

Or, to put it another way, **if, as we posited before, validators are akin to a judiciary, or upper house, then shouldn't their votes have equal weighting?**

Luckily, people are asking these questions, and tooling is improving for normal people to interrogate and understand blockchain-hosted code[5].

Finally, it's becoming increasingly common for projects to launch, and then stabilize into DAOs themselves. As these DAOs become able to host their own projects, and pay for any number of key services directly from their treasuries, they will force a step-change in how governments perceive these fundamentally cross-border, multilateral entities.

The real question will be how ownership thrashes out in practice in these DAOs - if they end up as unequal as the systems they have replaced, then all we have achieved with the interchain is simply to complete a multilateral (or, decentralized) expression of the inequality present in our existing systems.

___

## IV: Conclusion

We have a unique moment to build novel, multilateral governance systems that combat an increasingly regressive multilateral global order. Wouldn't it be cool if we took the opportunity?

___

[0] Though it is an interesting thought experiment to say: in a world where DAOs were self-governing with no external pressures, would it be reasonable to say that a core dev should always implement the wishes of the electorate? Maybe. Obviously though that is a pure thought experiment.

[1] In some cases, this ruling class goes all the way back to 1066, for an idea of just how resilient a ruling class can be.

[2] While this is controversial to some, we're obviously not against taxation. In the UK we have free healthcare as a result, and (personal story time) getting hit by a car and getting scraped off the road by paramedics and treated has cemented the author's already strong belief that taxes spent on human dignity are never wasted.

[3] Taken from [this article](https://www.e-flux.com/journal/65/336347/the-vectoralist-class/)

[4] Read the original article [here](https://nickmerrill.substack.com/p/warning-minority-rule-is-possible).

[5] Or 'smart contracts', if you prefer.
