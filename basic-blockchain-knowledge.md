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

## Decentralized Alternative Currency

Blockchain technology forms the foundation for cryptocurrencies like Bitcoin. This provides an alternative to traditional fiat currencies controlled by central authorities like the Federal Reserve.

In the central authority system with the U.S. dollar, users' data and money are controlled by banks and the government. If a bank is hacked or fails, users' private information and money is at risk. When banks failed in 2008, they were bailed out using taxpayer money.

Blockchain and cryptocurrencies solve these issues by operating in a decentralized manner across a network of computers, with no central controlling authority. This reduces risk and processing fees.
For people in countries with unstable currencies or financial systems, cryptocurrencies provide a more stable currency and infrastructure. They can access applications and networks to do business domestically and globally.

Using cryptocurrency wallets allows saving and spending, especially profound for the unbanked who lack state identification to access traditional financial services in unstable regions or war-torn areas without robust ID systems.

## Simple Medical Records on Blockchain

Doctors can use blockchain to safely store their patients' medical records. When a medical record is made and signed, it can be saved on the blockchain. The blockchain proves the record cannot be changed. The medical records would be locked with a private code so only certain people can see them. This keeps the records private.

Patients will know their medical records are secure on the blockchain and have not been changed. They can also choose who can see their private medical records by controlling the code. So blockchain allows safe storage of medical records that cannot be altered, while also keeping the records private and giving patients control over who views them.

Here's an explanation of using blockchain for property records in simple terms:

## Simple Property Ownership Records on Blockchain

Have you been to a government office to record who owns a property? It is hard work and not efficient. A physical deed paper has to be taken to an office worker. They type the details into a central database by hand. If there is a dispute over who owns the property, the records have to be checked against this database.This takes a lot of time and money. There can also be mistakes because humans type the records. Mistakes make tracking property ownership harder.

Blockchain can remove the need to scan papers and look for physical files. If property ownership is recorded on the blockchain, owners can trust the records are accurate and saved permanently.

In countries with war or no government offices to record properties, proving who owns what is nearly impossible. If people in those areas use blockchain, clear timelines of property ownership can be made that everyone can see.

Here's an explanation of smart contracts using simple language:

## Simple Automatic Agreements with Smart Contracts

A smart contract is a computer code that can be built into the blockchain. It helps carry out an agreement between people automatically. They work based on conditions that users agree to. When those conditions are met, the terms of the agreement happen automatically.

For example, let's say a renter wants to lease an apartment using a smart contract. The landlord agrees to give the door code to the renter after receiving the security deposit. The smart contract will automatically send the door code to the renter once the deposit is paid. It can also be set to change the code if rent is not paid or other conditions are met.

So smart contracts make agreements happen automatically on the blockchain based on the conditions people agree to, without needing a middle person.

Here's an explanation of using blockchain for supply chains in simple terms:

## Tracking Food and Goods on the Blockchain

Like in the IBM Food Trust example, suppliers can use blockchain to record where materials come from that they buy. This allows companies to prove that their products and labels like "Organic", "Local", and "Fair Trade" are real.

The food industry is increasingly using blockchain to track the path food takes from farms to consumers and ensure it is safe.

Suppliers put information about where food or goods originate on the blockchain ledger. Companies can then verify the journey and authenticity of those items by checking the blockchain records. This way, blockchain provides a transparent and permanent record of where products come from and their path through the supply chain before reaching stores and customers. Companies and consumers can have confidence in trusting product claims.

So blockchain brings more transparency and trust to supply chains by tracking the true origins and journey of foods and goods.

Here's an explanation of using blockchain for voting in simple terms:

## Secure and Transparent Voting with Blockchain

Blockchain could be used for a modern voting system. Using blockchain for voting can help prevent election fraud and increase voter participation, as tested in the November 2018 elections in West Virginia.

With blockchain voting, it would be extremely difficult to tamper with or change any votes cast. The blockchain records would make the whole voting process transparent. Fewer people would be needed to conduct an election, and officials could get results almost instantly. This would remove the need for recounts or worries about fraud impacting the election results. The blockchain provides a permanent, unchangeable record of all votes.

So blockchain allows secure, transparent and efficiently counted votes that are resistant to tampering or fraud, while requiring fewer resources to conduct an election. This could boost trust and participation in the voting process.

## Pros and Cons of Blockchain

Here are the pros and cons of blockchain presented in a tabular form:

| Pros | Cons |
|-|-|
| Improved accuracy by removing human involvement in verification | Significant technology cost associated with some blockchains |
| Cost reductions by eliminating third-party verification | Low transactions per second |
| Decentralization makes it harder to tamper with | History of use in illicit activities, such as on the dark web |
| Transactions are secure, private, and efficient | Regulation varies by jurisdiction and remains uncertain |
| Transparent technology | Data storage limitations |
| Provides a banking alternative and a way to secure personal information for citizens of countries with unstable or underdeveloped governments | |


Here are the drawbacks of blockchains explained in simple terms, not in a tabular form:

## Downsides of Blockchain Technology

### **High Technology Costs**

 While blockchain can save money on transaction fees, the technology itself is very expensive. The Bitcoin network, which uses a system called "proof-of-work" to validate transactions, consumes huge amounts of computer power. In fact, the energy used by all the devices on the Bitcoin network is more than the entire country of Pakistan uses in a year! However, some solutions are being developed to address these high energy costs. For example, bitcoin-mining farms are being set up to use renewable energy sources like solar power, excess natural gas from fracking sites, or wind farm energy.
  
  So while the blockchain technology behind Bitcoin provides benefits, the massive energy consumption required is a major drawback that is starting to be addressed through alternative energy sources powering the mining operations.

  Here's an explanation of the speed and data inefficiency drawbacks of blockchains using simple terms:

### **Blockchain Can Be Slow and Limited**

Bitcoin is a good example of how blockchains can be inefficient. Bitcoin's system for validating transactions takes around 10 minutes to add a new block of transactions to the blockchain. At this rate, the Bitcoin network can only handle about 3 transactions per second.

Other cryptocurrencies like Ethereum perform better than Bitcoin, but blockchains still limit how many transactions they can process. For comparison, the traditional Visa payment system can handle 65,000 transactions per second!

Solutions to increase blockchain transaction speeds have been in development for years. Some newer blockchains can already process over 30,000 transactions per second. Ethereum is also upgrading to potentially allow 100,000 transactions per second by splitting up its database. Another issue is that each block on a blockchain can only hold a limited amount of data. The debate around increasing this "block size" is an ongoing challenge for scaling blockchains to handle more data.

So while very secure, the relatively slow transaction speeds and limited data capacity of current blockchains are drawbacks that developers are still trying to overcome through technological improvements.

Here's an explanation of the illegal activity drawback of blockchains in simple terms:

### **Blockchain Anonymity Enables Some Illegal Uses**

While the privacy and anonymity that blockchains provide protect users' data, it also allows some illegal trading and activities to occur on blockchain networks.

The most well-known example is the Silk Road online marketplace on the dark web that operated from 2011 to 2013. It allowed people to buy and sell illegal drugs and launder money using Bitcoin and other cryptocurrencies anonymously before the FBI shut it down.

The dark web and cryptocurrencies make it harder to track illegal purchases and sales compared to traditional financial regulations. Banks have to verify customer identities and check against lists of criminals or terrorists when accounts are opened.

However, only a very small portion (0.24%) of all cryptocurrency transactions in 2022 involved illegal activity according to research firm Chainalysis.

This anonymity feature can be seen as both positive, providing access to finance, and negative by enabling some criminal uses. Many argue the benefits of giving the unbanked access to financial services outweigh the relatively low levels of illegal cryptocurrency activity compared to untraceable cash transactions.

So while blockchains enable privacy, their anonymity also creates some opportunities for illegal uses that authorities try to monitor and prevent where possible.

Here's an explanation of the regulation concerns around blockchains and cryptocurrencies in simple terms:

### **Government Regulation a Potential Worry**

Many people involved with cryptocurrencies have concerns about government regulation. While it is becoming very difficult to completely shut down a decentralized network like Bitcoin as it grows larger, governments could theoretically make it illegal to own cryptocurrencies or participate in their networks.

However, this regulatory concern has reduced over time as major companies like PayPal have started allowing customers to use cryptocurrencies on their platforms. This mainstream adoption makes a cryptocurrency ban less likely.

So while there were initial worries that governments may try to restrict or prohibit blockchains and cryptocurrencies, the widespread growth and increasing acceptance by major businesses has eased some of those regulatory concerns. But regulatory uncertainty around blockchains and cryptocurrencies still remains in many jurisdictions*.
