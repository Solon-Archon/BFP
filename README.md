# Bitcoin Fork Proposal Process

## 1. Contents

&nbsp;

1. Contents
2. Statement of Need
3. Objectives
4. Proposal - BFP Process
5. Example
6. Evaluation
7. Future Objectives
8. Risks
9. Support

&nbsp;
&nbsp;

-------------------

&nbsp;
&nbsp;

## 2. Statement of Need

&nbsp;

Finding consensus is hard, especially when using a decentralised development structure. Having multiple development teams, and therefore multiple streams of proposals, means that there is bound to be conflict and competition. This is a good thing though. Not only does decentralised development spread power and influence out so that there is **no core**, it also leads to a marketplace of competing ideas. More ideas means a higher probability of finding optimal solutions.

The downfall of this approach is the fact that it becomes difficult to decide what proposals gets implemented. Egos can flare up, and a split in the commmunity can occur if a debate gets too heated. Cryptocurrencies rely on network effect, therefore in almost all situations it is better for a network to remain in consensus. The only situation when a network split is justified, is when there is a fundamental idealogical disagreement within the community, like there was in Bitcoin for the past 3 years. In this situation it is better for a split to occur, and each group can go their separate ways, like in the situation of Bitcoin Cash and Bitcoin. This should be a rare occurance though, and therefore there is a need to implement an improved consensus finding process.

Consensus is not required for all software changes. It is only required for changes that will cause a split in the network. Development teams are free to make any software changes to their own code base that do not cause a split the network. Sometimes software upgrades will be required that can potentially cause a split in the network. It is important there is a process that the various development teams agree to follow, that allows upgrades to happen without causing a network split. Equally, it is important that each development team is able to offer up solutions to solving a problem, that may not necessarily be compatible with the solutions provided by the other teams.

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 3. Objectives

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

## 4. Proposal - BFP Process - Bitcoin (Cash) Fork Proposal

&nbsp;

### 4.1. Development Process

&nbsp;

The development process stays as it is currently, where anyone can discuss, develop and test software solutions, and then propose them to the network. The only difference being that they will assign their proposals a unique BFP ID using the guidelines below.

&nbsp;

### 4.2. Signalling

&nbsp;

Signalling is done by miners in the coinbase by using the following format: BFPXX/YY. 

XX represents a BFP 'batch' number. A batch number is a ID that represents a batch of proposals that all seek to fix the same problem. For example, all proposals that seek to fix the EDA problem.

YY represents a proposal number. The proposal number is an ID that represents a specific proposal in a batch of proposals. When YY = 0 then the miner is signalling that they do not support any proposal. 

&nbsp;

### 4.3. Voting Terms

&nbsp;

A proposal must receive absolute majority support (>50%) by miner signalling over a period of time, for the proposal to become locked in.

One caveat to this is that the aggregate support of all proposals must be over 75% vs support for 'no change', i.e. YY=0 in the signal.

The signalling period and lock-in period are to be pre-agreed by the entities making the proposals before the voting starts.

&nbsp;

### 4.4. Implementation

&nbsp;

After the signalling period occurs, all miners switch to signalling the winner of the vote, and the lock-in period starts. The lock-in period allows time for the participants of the network to update their software (if necessary). After the lock-in period 100% of the miners fork the network at a specific block number/timestamp.

In this way, miners and developers have a gentlemen's agreement with each other, and the network that; if a proposal receives the required support over the signalling period, then all miners will switch to support that proposal. This allows the network to remain in consensus while also allowing different solutions to compete.

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 5. Example

&nbsp;

There are three proposals. The proposals are given the IDs BFP1/1, BFP1/2, and BFP1/3. BFP1/0 is reserved for miners to signal for 'No Change' in a batch. The '1' in BFP1/Y is the batch number.
The community can then discuss the merits of each proposal, and miners can then signal for them. The miners signal/vote with the following representation over the signalling period:

- BFP1/0 = 10% share
- BFP1/1 = 55% share
- BFP1/2 = 15% share
- BFP1/3 = 20% share

The proposal BFP1/1 wins with a 55% share of the vote. This is because it has a majority share, and BFP1/0 is less than 25%. After the voting period ends, all miners then shift their signalling to BFP1/1 for the lock in period. The Bitcoin Cash economy then updates their software to be compatible with the BFP1/1 proposal. Miners then fork at a specific block height/ medium timestamp.

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 6. Evaluation

&nbsp;

I believe this proposal solves all the objectives specified but there is of course always room for improvement. 

&nbsp;
&nbsp;

---------------

&nbsp;
&nbsp;

## 7. Future Objectives

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

## 8. Risks

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

## 9. Support

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
- AcceptBitcoin.Cash
- u/KoKansei,
- u/jonald_fyookball
- Erik Beijnoff
- u/jessquit
- u/zquest
- Singularity

&nbsp;

I'd love to hear your thoughts below.

[Yours.org article](https://www.yours.org/content/a-proposal-for-a-consensus-finding-process-on-bitcoin-cash---the-bfp-p-ec068ee2043a)
