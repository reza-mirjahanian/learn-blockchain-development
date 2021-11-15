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
