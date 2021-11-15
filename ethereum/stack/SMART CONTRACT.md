
A "smart contract" is simply a program that runs on the Ethereum blockchain. It's a collection of code (its functions) and data (its state) that resides at a specific address on the Ethereum blockchain.

Smart contracts are a type of  [Ethereum account](https://ethereum.org/en/developers/docs/accounts/). This means they have a balance and they can send transactions over the network. However they're not controlled by a user, instead they are deployed to the network and run as programmed. User accounts can then interact with a smart contract by submitting transactions that execute a function defined on the smart contract. Smart contracts can define rules, like a regular contract, and automatically enforce them via the code. Smart contracts cannot be deleted by default, and interactions with them are irreversible



Ethereum has developer-friendly languages for writing smart contracts:

-   Solidity
-   Vyper

## COMPOSABILITY

Smart contracts are public on Ethereum and can be thought of as open APIs. That means you can call other smart contracts in your own smart contract to greatly extend what's possible. Contracts can even deploy other contracts

### Storage

Persistent data is referred to as storage and is represented by state variables. These values get stored permanently on the blockchain.

### Memory

Values that are only stored for the lifetime of a contract function's execution are called memory variables. Since these are not stored permanently on the blockchain, they are much cheaper to use

There are two types of function calls:

-   `internal`  – these don't create an EVM call
    -   Internal functions and state variables can only be accessed internally (i.e. from within the current contract or contracts deriving from it)
-   `external`  – these do create an EVM call
    -   External functions are part of the contract interface, which means they can be called from other contracts and via transactions.


### View functions

These functions promise not to modify the state of the contract's data.

### What is considered modifying state:

1.  Writing to state variables.
2.  [Emitting events](https://solidity.readthedocs.io/en/v0.7.0/contracts.html#events).
3.  [Creating other contracts](https://solidity.readthedocs.io/en/v0.7.0/control-structures.html#creating-contracts).
4.  Using `selfdestruct`.
5.  Sending ether via calls.
6.  Calling any function not marked `view` or `pure`.
7.  Using low-level calls.
8.  Using inline assembly that contains certain opcodes
