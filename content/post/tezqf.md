---
linkTitle: "https://forum.tezosagora.org/t/tezqf-a-quadratic-funding-and-clr-matching-based-grants-platform-on-tezos/2275/14"
title: "Quadratic Funding & CLR Matching based Grants Platform on Tezos"
summary: "The Tezos ecosystem has been growing rapidly and it is about time it has a grants platform to support the upcoming projects. We propose a quadratic funding and CLR matching based grants platform for an optimized and fair distribution of sponsor funds."
---

**Background and Motivations:**
There has been a rapid growth in the number of projects which are showing up on the Tezos ecosystem. Until now, most of the grants and support has been provided to the projects by Tezos Foundation, and other equivalent organizations. We believe that with Defi, Gaming, and various other spaces heating up on Tezos, it is about time we have a more robust grants platform which makes it easier for the funds to reach the right projects.

**TezQF** is a match funding platform, based on the foundation of **Liberal Radicalism**. Its core idea is inspired by the concept of **Quadratic Funding** as put forth by Vitalik Buterin, Zoë Hitzig, and Glen Weyl in their paper - [Liberal Radicalism: A Flexible Design For Philanthropic Matching Funds](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3243656).

Match-funding is an extension of crowdfunding. In addition to the contribution received from the community in a matching fund scheme, sponsors provide a ‘matching-gift’, usually in a 1:1 ratio. If Alice receives $1200 of community contribution for her project, she would be gifted an equal sum of $1200 by the sponsors.

Although this provides a better insight to the philanthropists and sponsors to direct their funds to the best of the entities, standard match-funding has a practical flaw that gets even more so exposed in a decentralized setting. To understand this better let’s consider an example-

- _10 contributors_ donated a total of _\$1200_ to Bob for his project whereas,
- John received the same amount i.e _\$1200_, but from just _2 contributors_, where one of the contributors was possibly his rich friend who contributed a hefty sum.

This indicates that Bob’s project has a higher community reach than John’s. Yet, both of them end up receiving the same match from the sponsors. Taking such situations into consideration gets trickier on a decentralized platform, as an entity might end up contributing to itself using a pseudo-anonymous account, thereby increasing the overall match significantly.

How can we design a better platform? Enter Quadratic Funding and the concept of **Capital-constrained Liberal Radicalism** (CLR) matching.

<br/>

**Mathematical Idea:**
Simply put, in quadratic funding the match amount is calculated as the square of the sum of the square-root of the contributions. As an equation, this would be-

> ![CodeCogsEqn (1)|177x59](upload://eXAQ66FZS8aMT8z8g2UkiK3mhpb.gif)
>
> Where ![CodeCogsEqn (2)|20x13, 100%](upload://n2iWFnBfGR85WAzRcCoK8B2md16.gif) is the individual contribution of a community member.

Considering our previous example, let’s say Bob received $120 from each of the 10 contributors whereas John received $1000 and \$200 from 2 contributors, then-

> ![CodeCogsEqn (5)|301x59](upload://jQE6evW1MGok2gmIi8itZfT3TY9.gif)
>
> ![CodeCogsEqn (6)|349x37](upload://wJiIjPKThaCDyFsqhINYko13S4b.gif)

We can see here, Bob’s match is significantly higher than John’s even though the contribution amount is the same. This is how CLR matching factors in the reach of the project.

On our platform, since we are having a funding pool consisting of limited funds at the start of every round, matching exactly to the result of the quadratic formula won’t be practical. Therefore, we use the result of the formula to calculate the ratio of subsidy weightage and then match accordingly.

For example, in the above situation, if the funding pool has _\$10,000_:

**Background and Motivations:**
There has been a rapid growth in the number of projects which are showing up on the Tezos ecosystem. Until now, most of the grants and support has been provided to the projects by Tezos Foundation, and other equivalent organizations. We believe that with Defi, Gaming, and various other spaces heating up on Tezos, it is about time we have a more robust grants platform which makes it easier for the funds to reach the right projects.

**TezQF** is a match funding platform, based on the foundation of **Liberal Radicalism**. Its core idea is inspired by the concept of **Quadratic Funding** as put forth by Vitalik Buterin, Zoë Hitzig, and Glen Weyl in their paper - [Liberal Radicalism: A Flexible Design For Philanthropic Matching Funds](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3243656).

Match-funding is an extension of crowdfunding. In addition to the contribution received from the community in a matching fund scheme, sponsors provide a ‘matching-gift’, usually in a 1:1 ratio. If Alice receives $1200 of community contribution for her project, she would be gifted an equal sum of $1200 by the sponsors.

Although this provides a better insight to the philanthropists and sponsors to direct their funds to the best of the entities, standard match-funding has a practical flaw that gets even more so exposed in a decentralized setting. To understand this better let’s consider an example-

- _10 contributors_ donated a total of _\$1200_ to Bob for his project whereas,
- John received the same amount i.e _\$1200_, but from just _2 contributors_, where one of the contributors was possibly his rich friend who contributed a hefty sum.

This indicates that Bob’s project has a higher community reach than John’s. Yet, both of them end up receiving the same match from the sponsors. Taking such situations into consideration gets trickier on a decentralized platform, as an entity might end up contributing to itself using a pseudo-anonymous account, thereby increasing the overall match significantly.

How can we design a better platform? Enter Quadratic Funding and the concept of **Capital-constrained Liberal Radicalism** (CLR) matching.

<br/>

**Mathematical Idea:**
Simply put, in quadratic funding the match amount is calculated as the square of the sum of the square-root of the contributions. As an equation, this would be-

> ![CodeCogsEqn (1)|177x59](upload://eXAQ66FZS8aMT8z8g2UkiK3mhpb.gif)
>
> Where ![CodeCogsEqn (2)|20x13, 100%](upload://n2iWFnBfGR85WAzRcCoK8B2md16.gif) is the individual contribution of a community member.

Considering our previous example, let’s say Bob received $120 from each of the 10 contributors whereas John received $1000 and \$200 from 2 contributors, then-

> ![CodeCogsEqn (5)|301x59](upload://jQE6evW1MGok2gmIi8itZfT3TY9.gif)
>
> ![CodeCogsEqn (6)|349x37](upload://wJiIjPKThaCDyFsqhINYko13S4b.gif)

We can see here, Bob’s match is significantly higher than John’s even though the contribution amount is the same. This is how CLR matching factors in the reach of the project.

On our platform, since we are having a funding pool consisting of limited funds at the start of every round, matching exactly to the result of the quadratic formula won’t be practical. Therefore, we use the result of the formula to calculate the ratio of subsidy weightage and then match accordingly.

For example, in the above situation, if the funding pool has _\$10,000_:

> ![|337x19](https://lh4.googleusercontent.com/AIKjmZyh7JAFYEZ3JsQd5KGamk6UBG9gjUh-ovttNf3Px1nG4t4b4k_DTlPMBoKHTsHRsNxVfU8Rb_zDwvKLQSQWVyjE-6vZCSdprxmHc1EPWqkCxM-8zsUywgoIfPzuDpTUR0_G) ![|338x19](https://lh3.googleusercontent.com/d8mpfXk_u3QQENp0U8S1zlrs2m5uhHFG5vkOOIWgkVEAzn1KAGWNUOEdRxmqmLcaqLuRP8-6ekJfkflH3FmH1b8STBHZS_0KSm3pNyrUpYMQPnbaTUdlWvCB0W6aaPLHi3Zkpiio)

> ![|337x19](upload://rjXwucTD0gb7RNO3YOT5Ic3GvEi.gif) ![|338x19](upload://3FSbAOeVH3THjyOhuEvltHr3Svc.gif)

So, Bob would receive _85%_ of \$10,000 whereas John would receive the remaining (Considering these are the only 2 entries).

To get a more in-depth insight into this, check out this [article](https://vitalik.ca/general/2019/12/07/quadratic.html).

<br />

**Architecture and Implementation:**
TezQF can be somewhat related to _Gitcoin Grants_ on Ethereum. Gitcoin Grants has a mixture of on-chain and off-chain components to it to manage security. However, with TezQF we are trying to put a majority of the features on-chain.

To achieve this we have created a _Decentralized Autonomous Organization (DAO)_ governing various aspects of the funding rounds through a token voting mechanism. Under the hood, this mechanism would follow [Quadratic Voting](https://en.wikipedia.org/wiki/Quadratic_voting) which would factor in the number of voters, besides the number of tokens used for a vote.

Our overall architecture consists of 3 smart contracts- A FA1.2 token contract for TQF governance token. A TQF DAO contract for handling all governance-related actions like round proposals, round initializations, and entry disputing (explained in detail in a later section). Finally, a Round Manager contract to handle all aspects of the funding rounds, like collecting contributions, receiving project entries, and matching the sponsor funds.

_Initially, governance tokens will be generated for the original team of developers and shall be extended to other members as they join the team._

_Basic architectural overview of the contract functionalities:_

![Arch|640x402, 75%](upload://k5i8cYLMdCQHhcIYtkrLdhpMzKX.png)

<br/>

_Activity Diagram of functionalities:_

![Activity|600x500, 75%](upload://fAJiLjRWGq5n3opuOwsNdzVRZjz.jpeg)

<br/>

**Important Actions:**

_Setting up a funding round proposal:_
Any TQF token holder having a balance above a certain threshold (2000 as of now) can set up a funding round proposal which shall be voted upon by other token holders by temporarily depositing their tokens. The voting decision will be made through quadratic voting.

_Entering a funding round:_
Any individual/team seeking funding for their project idea can enter an active funding round anytime. They have to provide some necessary details like a link to their codebase, an elaborate description, and the category their project belongs to.

_Raising a dispute:_
Any token holder can raise a dispute against a project listed in a funding round if he/she believes that the project is violating the integrity of the platform. To do so, the person must stake a certain amount of tokens (200 as of now), which shall be returned to him/her if and only if the dispute stands after a session of voting.

_Voting for a round proposal or dispute:_
All token holders can vote once, for/against any on-going proposal to conduct funding round, or a dispute being raised against an entry. To vote, the holder needs to deposit a certain number of tokens as he/she wishes (this number stands for the weight of the vote). These tokens shall be returned once the voting period expires.

_Contribute:_
All community members can contribute XTZ to the projects of their liking. There is no minimum limit on the amount of contribution. Because of the CLR matching, that we have implemented behind the scenes, even a contribution of < 5 XTZ from a few contributors could lead to a significant match.

_Sponsor a round:_
Anyone can become a sponsor by contributing XTZ to the match-funding pool during the donation period before the start of every round. As of now, we do not have a minimum limit for the sponsorship amount.

<br/>

**Why on-chain governance?**
On-chain governance would be a must since we are planning to keep the entire platform as decentralized as possible. Besides deciding on when to conduct the match-funding rounds, another important aspect of the governance model is to ensure that the listed projects maintain the integrity of the platform, and there’s a fair distribution of the CLR match.

Identity is a major issue when dealing with a decentralized setting. For a majority of the projects, the identity would be pseudo-anonymous which would lead to the issue of trust. Gitcoin Grants on Ethereum requires the entries to login using an aged Github account to participate. This ensures the identity, but there are still some potential issues.

Quadratic Funding is prone to Sybil attacks. Wherein, one person can create multiple pseudo-anonymous accounts and contribute a small amount to his project using each of the accounts. This would lead to an unfair distribution of funds. As of now, there’s no full-proof way to tackle Sybil attacks, but such an attack pattern is quite identifiable, and when combined with a voting model, any project appearing to self-contribute through multiple accounts can be voted against and disqualified.

<br/>

**Project Status:**
We are currently in the development stage with a demo running live on Delphinet. We are also planning a change- a mandatory security stake for all project entries. A part of this stake will go to the disputer in case the project gets disqualified.

We would soon be going for a public presentation to receive community feedback and consider any suggested changes. The link to the presentation will be posted in this thread soon. Meanwhile, all community members are welcomed to watch our platform walkthrough and give their valuable suggestions for improvements and addon.

<br />

Walkthrough video: [TezQF demo](https://www.youtube.com/watch?v=z6lqRbYnEXE&feature=youtu.be&ab_channel=GunaShekar)
Codebase: [TezQF Github](https://github.com/yashmuchhala/TezQF).
Live on Delphi: https://tezqf.vercel.app/ **(Requires Thanos Wallet)**

<br />
