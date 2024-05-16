# What is a blockchain?

A blockchain is a decentralized, digital ledger that records transactions across a network of computers. It is maintained by a network of nodes that all have a copy of the ledger.

Each block contains a record of transactions, and once a block is added to the blockchain, it becomes extremely difficult to change or delete that record. The blocks are linked together using cryptographic hashes, making it difficult to alter or manipulate the data. Blockchain technology is special because it is decentralized and data can't be changed once recorded. These features make blockchain transparent, secure, and ensure data remains accurate for many different uses.

![Blockchain Image](https://www.chainalysis.com/wp-content/uploads/2022/02/bloggraphic-blockchains-01-1-1500x818.png)

## How does a blockcahin work?

A blockchain is composed of **scripts** , which are programs that perform typical database functions such as entering, accessing, saving, and storing information. These scripts manage the data within the blockchain network. Additionally, a blockchain is distributed, meaning that multiple copies of the ledger are stored on numerous machines (nodes) within the network. For a blockchain to be considered valid, all these copies across different machines must match. This distributed nature ensures transparency, security, and decentralization in the blockchain system.

## Transaction Process

The process involved in the collection of transaction information in a blockchain starts with organizing this data into a block, similar to a row in a spreadsheet containing information. Once a block is filled with transactions, the data is processed through a cryptographic hashing algorithm, resulting in the creation of a unique alphanumeric string known as the **hash**. Subsequently, this hash is included in the header of the next block and hashed along with the other data within that block. This process continues, creating a chain of blocks where each block is cryptographically linked to the previous one through the inclusion of the hash from the preceding block. This chaining of blocks ensures the integrity and security of the data stored in the blockchain, as any alteration in one block would invalidate all subsequent blocks, making it highly secure and resistant to tampering.

![Blockchain Image](https://assets.euromoneydigital.com/dims4/default/5cad168/2147483647/strip/true/crop/800x500+0+0/resize/840x525!/quality/90/?url=http%3A%2F%2Feuromoney-brightspot.s3.amazonaws.com%2F74%2F45%2F14e0c55c46fbb79d982db7667db6%2Ftransactionsblockchainv2.png)

The process of transaction depends on the blockchain. For example Bitcoin blockchain involves the following process.

- Initiating a Transaction: A user initiates a transaction using their cryptocurrency wallet application. This application provides an interface to interact with the blockchain.
- Memory Pool: The transaction is sent to a memory pool, also known as the Mempool. This is where transaction are stored and queued until a miner or validator picks them up. The mempool acts as a temporary storage for transactions waiting to be verified.
- Block Creation: Once a miner or validator selects the transaction from the mempool, it is entered into a block. The block is filled with transaction until it reaches its capacity.
- Block Closure and Encryption: Once the block is full, it is closed and encrypted using an encryption algorithm. This ensures the integrity and security of the transaction within the block.
- Mining: The encrypted block is then processed through a process called mining. Mining involves solving complex mathematical problems to validate the transaction within the block and ensure the integrity of the blockchain. This process is energy-intensive and requires significant computational power.
- Blockchain Update: After the block is mined , the blockchain is updated to include the new block. This update ensures that all nodes on the network have the same version of the blockchain, maintaining the integrity and consistency of the ledger.

### Bitcoin Mining and Proof-of-Work

1. **Network and Hashing**:
    - The entire Bitcoin network is a bunch of computers (miners) working together.
    - They’re all trying to solve a complex puzzle, which involves finding a specific type of hash.

2. **Nonce**:
    - A nonce is a special number that miners adjust to try and find the right hash.
    - They start with a nonce of zero and add it to their generated hash.
    - If the resulting hash doesn’t meet the required criteria (i.e., isn't lower than a target value), they increase the nonce by one and try again.

3. **Proof-of-Work**:
    - Miners keep adjusting the nonce and generating new hashes until one of them hits the jackpot – a hash that meets the criteria.
    - The first miner to find a valid hash wins a reward.
    - This process of generating tons of hashes is called "proof-of-work" because it proves the miner has done a lot of computational work.

4. **Energy Consumption**:
    - Since it takes a massive amount of attempts to find the right hash, Bitcoin mining consumes a lot of computational power and energy.

### Block Confirmation

1. **Closing a Block**:
    - Once a miner finds the right hash, a block of transactions is closed and added to the blockchain.
    - However, this block isn’t fully confirmed yet.

2. **Confirmation Process**:
    - For a block to be fully confirmed, it needs to be followed by five more blocks, each also validated by the network.
    - This process ensures the security and integrity of the blockchain.
    - Since each block takes about 10 minutes to validate, it takes roughly an hour for full confirmation.

### Ethereum and Proof-of-Stake

1. **Different Approach**:
    - Ethereum uses a different method called "proof-of-stake".
    - Instead of competing to solve a puzzle, the network randomly selects one user who has staked some ether (Ethereum’s currency) to validate the block.

2. **Efficiency**:
    - This method is much faster and uses far less energy compared to Bitcoin’s proof-of-work.
    - It’s more eco-friendly because it doesn’t require massive amounts of computational power.

## Blockchain Decentralization

In a blockchain network, the data (e.g., transaction records, information) is not stored in a single centralized location. Instead, it is distributed and replicated across multiple nodes (computers or devices) in the network. By having the data spread across multiple nodes, blockchain creates redundancy, which ensures the integrity and fidelity of the data. If someone tries to alter the data at one node, the other nodes will not accept the altered data, preventing the change from being propagated to the rest of the network. Since there is no central authority or single point of control, no single node can unilaterally alter or modify the data stored in the blockchain. This decentralized nature makes the blockchain resistant to data tampering or manipulation by any single entity.
The records stored in a blockchain, such as transactions in a cryptocurrency, are essentially irreversible and immutable. Once data is recorded on the blockchain, it becomes extremely difficult (or practically impossible) to alter or delete it because of the cryptographic proofs and the consensus mechanisms used by the network.

## Blockchain Transparency

The Bitcoin blockchain is spread out, not controlled by one person or place. This means anyone can see all the money movements. You can do this in two ways:

- Run your own personal blockchain computer (called a node) that gets copies of all the money movements.
- Use online explorers e.g. [Blockchain explorers](https://www.blockchain.com/explorer?utm_campaign=dcomnav_explorer) that show live money movements on the blockchain.

Every node computer has a copy of all the money movement records. When new verified records come in, the node updates itself. So if you want, you can follow a bitcoin and see where it goes. Even if you don't know who owns that bitcoin address. Sometimes hackers steal cryptocurrencies from exchanges. The hackers' identities are secret, but not their bitcoin addresses. Since the addresses are public on the blockchain, we can trace where the stolen crypto went. The blockchain records are locked with secret codes. Only the real owner of an address can open it and show their identity. This way, people using the blockchain can stay anonymous, but everyone can still see all the money movements transparently.

## Blockchain Security

Blockchains are secure in a few ways. First, new blocks are always added one after the other in a line. Once a block is added, you cannot change the ones before it. If someone tries to change data in a block, it will change that block's code (called a hash). Since each new block contains the previous block's hash, changing one block's data would mess up all the following blocks. The blockchain network would see the hashes don't match and reject the changed block.

However, no blockchain is 100% safe. They use code to make security. If there are mistakes in the code, hackers could possibly break in. Imagine a hacker runs a computer (node) on a blockchain network. They want to change the blockchain and steal crypto from others. If they change their copy, they need to convince over half of the other nodes that their changed copy is the real one. This is very hard because the blockchain networks create new blocks super fast - like millions per second for Bitcoin. By the time the hacker acts, the real blockchain is already way ahead.

So while not perfect, blockchains use many smart ways like hashes, ordering blocks, and lightning speed to make it extremely difficult for hackers to break in and change data.

## Blcokchain Origins

In 1991, two researchers named Stuart Haber and W. Scott Stornetta first described blockchain technology. They wanted a system where document timestamps could not be changed. But blockchain didn't get its first real-world use until almost 20 years later in 2009, with the launch of Bitcoin.

Bitcoin works using a blockchain. Bitcoin's creator, going by the name Satoshi Nakamoto, described it as "a new electronic cash system that's fully peer-to-peer, with no third party involved."

The key thing is that Bitcoin uses blockchain to openly record a list of payments or other transactions between people. So while the idea started in 1991, blockchain technology truly came alive with Bitcoin's creation in 2009 as a way to transparently track digital money movements without needing a middleman like a bank.

## Blockchain Vs. Banks

Here's a table comparing Blockchain vs. Banks using the points provided:

| Feature | Banks | Bitcoin |
|---------|-------|---------|
| Hours Open | Typical 9am-5pm weekdays, limited weekends, closed on bank holidays | Always open 24/7, 365 days |
| Transaction Fees | Card payments, checks, ACH, wire transfers can cost $1-$45 | Variable fees from $0-$50 set by miners/users |
| Transaction Speed | 24-72 hours, not processed on weekends/holidays | 15 minutes to over an hour based on network |
| Know Your Customer Rules | Required to record customer ID before opening account | No ID required, even AI can participate |
| Ease of Transfers | Need ID, bank account, mobile phone | Just need internet and mobile phone |
| Privacy | Limited to bank's server security and user's practices | Can be fully anonymous if purchased privately |
| Security | Depends on bank's servers and user's practices | More secure as network grows, user controls security |
| Approved Transactions | Banks can deny/freeze transactions and accounts | No restrictions, users transact freely |
| Account Seizures | Governments can seize accounts due to KYC laws | Hard to seize anonymous Bitcoin |
