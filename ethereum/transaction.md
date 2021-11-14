
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
