To ensure that all participants on the Ethereum network maintain a synchronized state and agree on the precise history of transactions, we batch transactions into blocks. This means dozens (or hundreds) of transactions are committed, agreed on, and synchronized on all at once.


## WHAT'S IN A BLOCK?

-   `timestamp`  – the time when the block was mined.
-   `blockNumber`  – the length of the blockchain in blocks.
-   `baseFeePerGas`  - the minimum fee per gas required for a transaction to be included in the block.
-   `difficulty`  – the effort required to mine the block.
-   `mixHash`  – a unique identifier for that block.
-   `parentHash`  – the unique identifier for the block that came before (this is how blocks are linked in a chain).
-   `transactions`  – the transactions included in the block.
-   `stateRoot`  – the entire state of the system: account balances, contract storage, contract code and account nonces are inside.
-   `nonce`  – a hash that, when combined with the mixHash, proves that the block has gone through  [proof of work](https://ethereum.org/en/developers/docs/consensus-mechanisms/pow/)
