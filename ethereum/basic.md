In the Ethereum universe, there is a single, canonical computer (called the Ethereum Virtual Machine, or EVM) whose state everyone on the Ethereum network agrees on. Everyone who participates in the Ethereum network (every Ethereum node) keeps a copy of the state of this computer.

Ethereum currently uses a [proof-of-work](https://ethereum.org/en/developers/docs/consensus-mechanisms/pow/) consensus mechanism.

## ETHER
The purpose of ether, the cryptocurrency, is to allow for a market for computation. Such a market provides an economic incentive for participants to verify and execute transaction requests and provide computational resources to the network.


## SMART CONTRACTS
application developers upload programs (reusable snippets of code) into EVM storage, and users make requests to execute these code snippets with varying parameters. We call the programs uploaded to and executed by the network smart contracts.


## Accounts
Where ether is stored. Users can initialize accounts, deposit ether into the accounts, and transfer ether from their accounts to other users. Accounts and account balances are stored in a big table in the EVM; they are a part of the overall EVM state

## Transactions
A "transaction request" is the formal term for a request for code execution on the EVM, and a "transaction" is a fulfilled transaction request and the associated change in the EVM state. Any user can broadcast a transaction request to the network from a node. For the transaction request to affect the agreed-upon EVM state, it must be validated, executed, and "committed to the network" by another node


## MINTING ETHER
Minting is the process in which new ether gets created on the Ethereum ledger. The underlying Ethereum protocol creates the new ether, and it is not possible for a user to create ether.

## BURNING ETHER
As well as creating ether through block rewards, ether can get destroyed by a process called 'burning'. When ether gets burned, it gets removed from circulation permanently.

## TRANSFERRING ETHER
Each transaction on Ethereum contains a value field, which specifies the amount of ether to be transferred, denominated in wei, to send from the sender's address to the recipient address.
https://etherscan.io/address/0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae
