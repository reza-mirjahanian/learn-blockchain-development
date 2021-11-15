
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


## TRANSACTION LIFECYCLE

Once the transaction has been submitted the following happens:

1.  Once you send a transaction, cryptography generates a transaction hash:  `0x97d99bc7729211111a21b12c933c949d4f31684f1d6954ff477d0477538ff017`
2.  The transaction is then broadcast to the network and included in a pool with lots of other transactions.
3.  A miner must pick your transaction and include it in a block in order to verify the transaction and consider it "successful".
    -   You may end up waiting at this stage if the network is busy and miners aren't able to keep up.
4.  Your transaction will receive "confirmations". The number of confirmations is the number of blocks created since the block that included your transaction. The higher the number, the greater the certainty that the network processed and recognised the transaction.
    -   Recent blocks may get re-organised, giving the impression the transaction was unsuccessful; however, the transaction may still be valid but included in a different block.
    -   The probability of a re-organisation diminishes with every subsequent block mined, i.e. the greater the number of confirmations, the more immutable the transaction is.
