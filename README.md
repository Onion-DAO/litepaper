# Onion DAO Litepaper

```
version: 0.0.1
contributors: actuallymentor
contact: @actuallymentor (Twitter), Mentor#8798 (Discord)
```

Onion DAO recognises that **public goods run by volunteers** result in suboptimal support for said public goods. Onion DAO aims to **add incentive layers to public goods** in order to stimulate entities to support them.

The first (and potentially only) application of this principle is to stimulate the running of [Tor](https://www.torproject.org/) exit nodes by rewarding [POAP](https://poap.xyz/)s as detailed in the [actuallymentor/onion-poap](https://github.com/actuallymentor/onion-poap) Github repository.

## 1. There are public goods run by volunteers

> In economics, a public good (also referred to as a social good or collective good)[1] is a good that is both non-excludable and non-rivalrous. [Wikipedia, 11-march-2022](https://en.wikipedia.org/wiki/Public_good_(economics))

Especially in the digital world, many (unfunded or underfunded) **volunteers maintain tooling that is essential** to the human race. Examples include:

1. Open source libraries
2. Tor network node operators
3. Wikipedia content writers and moderators

The **world tends to be wholly unaware** how much of our collective human infrastructure depends on a few dedicated volunteers. Examples include:

Steven Pruitt, who _"is an American Wikipedia editor with the highest number of edits made on the English Wikipedia, at 4.4 million. He has also created more than 33,000 Wikipedia articles."_ ([Wikipedia](https://en.wikipedia.org/wiki/Steven_Pruitt), 11 March 2022)

The OpenSSL maintainers, who write the specifications and code for the security of amongst other things the `https://` in your browser. In 2014 a major bug caused chaos across the world, at which point [Ars Technica noted](https://arstechnica.com/information-technology/2014/04/tech-giants-chastened-by-heartbleed-finally-agree-to-fund-openssl/) that: _"Tech giants, chastened by Heartbleed, finally agree to fund OpenSSL ... The important role OpenSSL plays in securing the Internet has never been matched by the financial resources devoted to maintaining it."_

> In essence we rely on the donated time and expertise of random people for **foundational aspects of our society**

The most relevant public good for Onion DAO at this point is the [Tor network](https://www.torproject.org/), an anonymity network and browser which _"sees use by many important segments of the population, including whistle blowers, journalists, Chinese dissidents skirting the Great Firewall and oppressive censorship, abuse victims, stalker targets, the US military, and law enforcement, just to name a few"_ ([read more about Tor users](https://2019.www.torproject.org/about/torusers)).

The Tor network relies on volunteers who are paid nothing to run the nodes that anonymise the traffic of its users.

## 2. Useful activities should be rewarded

If you want more of a thing, you should reward that thing; if you want people to do useful things, **give them incentives to do useful things**.

> Show me the incentives and I will show you the outcome. ~ Charlie Munger

In his book "Bullshit Jobs", anthropologist David Graeber describes a societal tendency to assume that **doing good should be payment enough**. This is reflected in statements like "you shouldn't become a teacher because you want to make money, but because you have a passion for teaching".

There appears to be a measurable trend where activities with **positive societal externalities receive on aggregate less** financial compensation than those with negative societal externalities. Estimates are that *"the negative externalities from management are 8.1% of total income"*, whereas teachers cause a *"spillover of 6.8% of economy income"* (doi `10.1086/693393`, p30-34).

> Plainly: job types that cause societal mayhem when they strike (nurses, garbage men, etc) are paid less than those who cause little to no societal issues when they strike (bankers, corporate lawyers).

Onion DAO believes that this tendency is harmful, and that upon reflection most people would agree that **rewarding good activities is a positive thing**.

## 3. Blockchain tokens as behaviour rewards

Both fungible and non-fungible tokens can be used to reward behaviour, different applications of tokens can be used to signal reputation or provide utility:

- POAPs are effective at signalling activity and presumably with that signal values held by an entity
- Profile picture NTFs (PFPs) are ways to express identity or affiliation
- Fungible tokens provide easy-to-compare relative stakes in a project

Onion DAO will explore the use of these token types to reward behaviours that contribute to under- and/or unfunded public goods.

### 3.1 Non-fungible tokens as reputation markers

POAPs are a way to verify activity according to the issuer of the POAP. Expressed differently: the issuer of a POAP is an oracle that bridges real-world activity to an on-chain token.

Onion DAO will provide POAPs to those who contribute to public goods, starting with the running of a Tor exit node.

The initial utility of these POAPs is purely reputational, in that contributors can showcase their contribution on their POAP profiles.

### 3.2 Fungible tokens as reputation markers

The advantage of NFTs as tokens is that they can easily be traced to a specific action on behalf of a specific individual. A downside however is that they are **harder to compare on a value-judgement level**.

A POAP profile for example is a great way to get a sense of a wallet-owner's activity in an ecosystem, but viewing a list of POAP holders is not a practical way to figure out **who is a core supporter** of a project.

Fungible tokens could be used as an **expression of the level of desirable behaviour** an entity engaged in. Instead of saying "`0xrobin`'s profile has a few Onion POAPs so they are a supporter of a public good", one could say "`0xrobin`'s wallet has 10% of all Onion `erc20` tokens, they are a vital supporter of the Onion DAO".

### 3.3 Financialising tokens to sustain desirable behaviour

**Reputation points alone may provide enough incentive** to take action to support a public good. But adding a way to (in-)directly provide financial support to those providing a public-good service may stimulate desirable behaviour much more**.

It is possible that a **third-party entity wishes to support** those who contribute to public goods, but is unable or unwilling to contribute in a direct way.

One way that desire to support could be harnessed is by **providing a fungible token** to public good supporters, that could be traded against a monetary reward.

One example implementation of this could look like:

1. `0xrobin` runs a Tor exit node for 3 months
2. `0xrobin` is awarded 3 POAPs that certify "you run a Tor exit node in jan/feb/march"
3. `oniondao.eth` airdrops 10 Onion `erc20` tokens for each Onion POAP distributed
4. `0xrobin` receives `3*10=30` Onion tokens
5. `0xrobin` swaps these tokens for Dai on Foodswap to pay for server costs
6. `0xbenefactor` swaps Dai for 200 `erc20` Onion tokens

In the above scenario `0xrobin` gets compensated (in whole or part dependent on Onion market price) for their beneficial activity, and `0xbenefactor` was able to frictionlessly support a public good and **signal their support in a quantifiable way**.

## 4. Proposed roadmap for Onion DAO

This is a sequence of events that could be taken to give shape to Onion DAO. It is not a promise or even a plan, it is not even a timeline.

- Phase 1: hand out POAPs to those running Tor exit nodes
	- Goal: build a community of public-good supporters that care about reputation
- Phase 2: structurally airdrop `erc20` tokens to Onion DAO POAP holders
	- Goal: provide a quantifiable and tradable way to reward support
- Phase 3: explore `erc20` demand driving activities like financialisation or the generation of Onion DAO PFPs in return for burning Onion DAO `erc20` tokens
	- Goal: provide financial support to those who take action to support public goods

## 5. How to get involved

Currently the Onion DAO is one step beyond "maybe we should start a DAO" and quite a while away from "airdrop next month". If you are interested in contributing to or following the progress of Onion DAO, you can:

1. [Run an Onion DAO Tor exit node](https://github.com/actuallymentor/onion-poap)
2. Follow [@actuallymentor](https://twitter.com/ActuallyMentor) on twitter for updates
3. Leave feedback on this document in this repository

