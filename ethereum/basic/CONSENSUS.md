By consensus, we mean that a general agreement has been reached. Consider a group of five people going to the cinema. If three out of five agree on a film, a consensus is achieved — majority rules.

Proof-of-work
Ethereum, like Bitcoin, currently uses a proof-of-work (PoW) consensus protocol

Proof-of-work is done by [miners](https://ethereum.org/en/developers/docs/consensus-mechanisms/pow/mining/), who compete to create new blocks full of processed transactions. The winner shares the new block with the rest of the network and earns some freshly minted ETH.

Proof-of-stake
Ethereum has plans to upgrade to a proof-of-stake (PoS) consensus protocol


A  **chain selection rule**  is used to decide which chain is the "correct" chain. Ethereum and Bitcoin currently use the "longest chain" rule, which means that whichever blockchain is the longest will be the one the rest of the nodes accept as valid and work with. For proof-of-work chains, the longest chain is determined by the chain's total cumulative proof-of-work difficulty.

The combination of proof-

## COMPARED TO PROOF OF STAKE

At a high level, proof-of-stake has the same end goal as proof-of-work: to help the decentralized network reach consensus securely. But it has some differences in process and personnel:

-   Proof-of-stake switches out the importance of computational power for staked ETH.
-   Proof-of-stake replaces miners with validators. Validators stake their ETH to activate the ability to create new blocks.
-   Validators don't compete to create blocks, instead they are chosen at random by an algorithm.
-   Finality is clearer: at certain checkpoints, if 2/3 validators agree on the state of the block it is considered final. Validators must bet their entire stake on this, so if they try to collude down the line, they'll lose their entire stake

## PROOF-OF-STAKE (POS)

Ethereum is moving to a consensus mechanism called proof-of-stake (PoS) from [proof-of-work (PoW)](https://ethereum.org/en/developers/docs/consensus-mechanisms/pow/). This was always the plan as it's a key part in the community's strategy to scale Ethereum via [the Eth2 upgrades](https://ethereum.org/en/eth2/). However getting PoS right is a big technical challenge and not as straightforward as using PoW to reach consensus across the network.

## PROOF-OF-STAKE, STAKING, AND VALIDATORS
Proof-of-stake is the underlying mechanism that activates validators upon receipt of enough stake. For Ethereum, users will need to stake 32 ETH to become a validator. Validators are chosen at random to create blocks and are responsible for checking and confirming blocks they don't create. A user's stake is also used as a way to incentivise good validator behavior. For example, a user can lose a portion of their stake for things like going offline (failing to validate) or their entire stake for deliberate collusion
