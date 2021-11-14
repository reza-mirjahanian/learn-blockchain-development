Ethereum has two account types:

-   Externally-owned – controlled by anyone with the private keys
-   Contract – a smart contract deployed to the network, controlled by code.


Both account types have the ability to:

-   Receive, hold and send ETH and tokens
-   Interact with deployed smart contracts

### Key differences

**Externally-owned**

-   Creating an account costs nothing
-   Can initiate transactions
-   Transactions between externally-owned accounts can only be ETH/token transfers

**Contract**

-   Creating a contract has a cost because you're using network storage
-   Can only send transactions in response to receiving a transaction
-   Transactions from an external account to a contract account can trigger code which can execute many different actions, such as transferring tokens or even creating a new contract



### EXTERNALLY-OWNED ACCOUNTS AND KEY PAIRS
An account is made up of a cryptographic pair of keys: public and private. They help prove that a transaction was actually signed by the sender and prevent forgeries. Your private key is what you use to sign transactions, so it grants you custody over the funds associated with your account. You never really hold cryptocurrency, you hold private keys – the funds are always on Ethereum's ledger.

The contract address is usually given when a contract is deployed to the Ethereum Blockchain. The address comes from the creator's address and the number of transactions sent from that address (the “nonce”)

Transactions are cryptographically signed instructions from accounts. An account will initiate a transaction to update the state of the Ethereum network. The simplest transaction is transferring ETH from one account to another

An Ethereum transaction refers to an action initiated by an externally-owned account, in other words an account managed by a human, not a contract. For example, if Bob sends Alice 1 ETH, Bob's account must be debited and Alice's must be credited. This state-changing action takes place within a transaction.

A submitted transaction includes the following information:

-   `recipient`  – the receiving address (if an externally-owned account, the transaction will transfer value. If a contract account, the transaction will execute the contract code)
-   `signature`  – the identifier of the sender. This is generated when the sender's private key signs the transaction and confirms the sender has authorised this transaction
-   `value`  – amount of ETH to transfer from sender to recipient (in WEI, a denomination of ETH)
-   `data`  – optional field to include arbitrary data
-   `gasLimit`  – the maximum amount of gas units that can be consumed by the transaction. Units of gas represent computational steps
-   `maxPriorityFeePerGas`  - the maximum amount of gas to be included as a tip to the miner
-   `maxFeePerGas`  - the maximum amount of gas willing to be paid for the transaction (inclusive of  `baseFeePerGas`  and  `maxPriorityFeePerGas`)

## TYPES OF TRANSACTIONS

On Ethereum there are a few different types of transactions:

-   Regular transactions: a transaction from one wallet to another.
-   Contract deployment transactions: a transaction without a 'to' address, where the data field is used for the contract code
