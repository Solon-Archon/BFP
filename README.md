Bitcoin Fork Proposal Process

## 1. Contents

&nbsp;

1. Contents
2. Introduction
3. Statement of Need
4. Objectives
5. Proposal - BFP Process
6. Example
7. Evaluation
8. Future Objectives
9. Risks
10. Support

&nbsp;
&nbsp;

-------------------

&nbsp;
&nbsp;

## 2. Introduction

&nbsp;

This could have been partly remedied by improved communication, but I think fundamentally it is an issue with the decentralised development model Bitcoin Cash has adopted (i.e. multiple development teams).
I would like to offer a proposal to improve the consensus finding mechanisms of Bitcoin Cash.

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 3. Statement of Need

&nbsp;

Finding consensus is hard, especially when using a decentralised development structure. Having multiple development teams, and therefore multiple streams of proposals, means that there is bound to be conflict and competition. This is a good thing though. Not only does decentralised development spread power and influence out so that there is **no core**, it also leads to a marketplace of competing ideas. More ideas means a higher probability of finding optimal solutions.

The downfall of this approach is the fact that it becomes difficult to decide what proposals gets implemented. Egos can flare up, and a split in the commmunity can occur if a debate gets too heated. Cryptocurrencies rely on network effect therefore in almost all situations it is better for a network to remain in consensus. The only situation when a network split is justified is when there is a fundamental idealogical disagreement within the community like there was in Bitcoin for the past 3 years. In this situation it is better for a split to occur and each group can go their separate ways, like in the situation of Bitcoin Cash and Bitcoin. This should be a rare occurance though and therefore there is a need to implement an improved consensus finding process.

Consensus is not required for all software changes. It is only required for changes that will cause a split in the network. Development teams are free to make any software changes to their own code base that do not cause a split the network. Sometimes software upgrades will be required that can potentially cause a split in the network. It is important there is a process that the various development teams agree to follow, that allows upgrades to happen without causing a network split. Equally, it is important that each development team is able to offer up solutions to solving a problem, that may not necessarily be compatible with the solutions provided by the other teams.

In the bitcoin white paper the following sentence refers to a decision making process:

>The proof-of-work also solves the problem of determining representation in majority decision making. If the majority were based on one-IP-address-one-vote, it could be subverted by anyone able to allocate many IPs. Proof-of-work is essentially one-CPU-one-vote. The majority decision is represented by the longest chain, which has the greatest proof-of-work effort invested in it.

Satoshi may have been suggesting that decisions could be made by all miners simply following the majority after a vote. In this way the network is able to make upgrades and the network remains in consensus at all times (i.e. no network splits). My proposal is essentially just this in a more formalised process.

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 4. Objectives

&nbsp;

- Unanimous consensus is no longer necessary.
- Development teams are able to offer up different proposals and the miners can decide which proposal is best.
- Miners are able to decide to make no change at all.
- The network remains in 100% consensus at all times other than in situations of extreme idealogical disagreement.
- Process can be implemented immediately.
- Process is loose enough that it can be applied to any upgrade that requires consensus.
- Does not conflict with other improvement proposal processes, such as BUIP.
- Provide confidence for network participants that community leaders (i.e. developers, miners and businesses) will support a process that aims to use free market principles but still keep the network in 100% consensus at all times.

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 5. Proposal - BFP Process - Bitcoin (Cash) Fork Proposal

&nbsp;

# 5.1. Development Process

&nbsp;

1. Developers find an issue in the software or think of an improvement that can be made, but the solution requires a network fork (hard or soft).
2. Development teams discuss how the issue can be fixed or how the improvement can be implemented. Cross pollination of ideas occurs and possibly some conflict.
3. Development teams created coded solutions that are then tested for safety and performance.
4. The community is then able to discuss the proposals in public and miners are able to signal for a specific proposal.

&nbsp;

# 5.2. Signalling

&nbsp;

Signalling is done by miners in the coinbase by using the following format: BFPXX/YY. 

XX represents a BFP 'batch' number. A batch number is a ID that represents a batch of proposals that all seek to fix the same problem. For example, all proposals that seek to fix the EDA problem.

YY represents a proposal number. The proposal number is an ID that represents a specific proposal in a batch of proposals. When YY = 0 then the miner is signalling that they do not support any proposal. 

A signalling period is used for miners to signal their support for a proposal.

&nbsp;

# 5.3. Voting Terms

&nbsp;

Voting terms are dependent on the nature of the issue being solved.

&nbsp;

# Time Sensitive Forks

If a fix/improvement needs to be chosen in a short amount of time the following terms can be used; a proposal must receive relative majority support (proposal with more miner support than any other proposal).

A caveat is that in the situation where there are only two options (i.e. BFPX/0 and BFPX/1) then a larger majority of 60% is required.

&nbsp;

**Standard Forks**

If a fix/improvement is not under time pressure, the following terms can be use; a proposal must receive absolute majority support (>50%) by miner signalling over a period of time, for the proposal to become locked in.

One caveat to this is that the aggregate support of all proposals must be over 75% vs support for 'no change', i.e. YY=0 in the signal.

&nbsp;

**Extreme Forks**

If a fix/improvement is significant, and it is highly controversial whether a change should take place, the following terms can be used; a proposal must receive a super majority of support (>75%) by miner signalling over a period of time, for the proposal to become locked in.

&nbsp;

# 5.4. Implementation

&nbsp;

Finally after the signalling period occurs all miners switch to signalling the winner of the vote, and the lock in period occurs. The lock in period allows time for the participants of the network to update their software (if necessary). After the lock in period 100% of the miners fork the network at a specific block number/time.

In this way, miners and developers have a gentlemen's agreement with each other and the network that; if a proposal receives the required support over the signalling period, then all miners will switch to support that proposal. This allows the network to remain in consensus while also allowing different solutions to compete.

Most soft and hard forks are not going to be idealogical disagreements like the Bitcoin Cash genesis fork was. There may be some disagreement on the exact solution, but in almost all cases it will be preferable for one proposal to be chosen and the network to remain in consensus.

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 6. Example

&nbsp;

Lets take the situation with EDA fix proposals and apply the BFP process to it. This can be considered to be a 'Time sensitive fork'. Discussion has already happened and proposals have been developed. There are three proposals. We will give the proposals the IDs BFP1/1, BFP1/2, and BFP1/3. BFP1/0 is reserved for miners to signal for 'No Change'. The '1' in BFP1/Y is the batch number.
The community can then discuss the merits of each proposal, and miners can then signal for them. The miners signal/vote with the following representation over the signalling period:

- BFP1/0 = 10% share
- BFP1/1 = 40% share
- BFP1/2 =30% share
- BFP1/3 = 20% share

The proposal BFP1/1 wins with a 40% share of the vote. This is because it has a higher share than any other proposal. After the voting period ends, all miners then shift their signalling to BFP1/1 for the lock in period. The Bitcoin Cash economy then updates their software to be compatible with the BFP1/1 proposal. Miners then fork at a specific block height/ medium timestamp.

If the example above had been a 'Standard Fork' then no proposal would have been chosen because no proposal reached >50% of the vote. In this situation a proposal with a smaller share may have to agree to bow out of the race (i.e. BFP1/3 in this scenario) as a way of breaking the deadlock.

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 7. Evaluation

&nbsp;

I believe this proposal solves all the objectives specified but there is of course always room for improvement. 

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 8. Future Objectives

&nbsp;

- Make improvements to the details of the BFP process.
- Research the use of a coded BFP process for a more streamlined and automated process. For example, automate the switching of signalling after a BFP receives the required support over the signalling period.
- Research the use of synthetic forks.
- Improve communication channels between the developers, miners and network participants.
- Improve communication by developers (The BFP process incentivises good communication of BFP proposals because it must win a vote).

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 9. Risks

&nbsp;

- Developers and/or miners do not stick to the agreed upon BFP process (already true).
- Miners do not educate themselves enough to make a decision on what the best proposal is (already true).
- Users do not have a way of signalling their preference (already true).
- Miners signalling falsely.

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 10. Support

&nbsp;

This is a list of all people who support this initiative. Please reach out and say if you support this.

&nbsp;

- u/ftrader
- LocalBitcoinCash.org
- Ryan X Charles.
- Yours.org
- Robbot
- Rocketr.net
- Tippr
- u/KoKansei,
- u/jonald_fyookball
- Erik Beijnoff
- u/jessquit
- u/zquest
- Singularity

&nbsp;

I'd love to hear your thoughts below.

[Yours.org article](https://www.yours.org/content/a-proposal-for-a-consensus-finding-process-on-bitcoin-cash---the-bfp-p-ec068ee2043a)
