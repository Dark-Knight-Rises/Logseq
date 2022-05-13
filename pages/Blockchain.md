filters:: {"now" true}

- What is  Blockchain? #card
  collapsed:: true
	- A blockchain is an <ins>open</ins>, <ins>distributed ledger</ins>  that can record transactions between two parties <ins>efficiently</ins>  and in a <ins>verifiable</ins> and <ins>permanent</ins> way. (lansiti, lakhani 2017) #defination
	  card-last-score:: 3
	  card-repeats:: 2
	  card-next-schedule:: 2022-05-12T19:18:03.198Z
	  card-last-interval:: 4
	  card-ease-factor:: 2.36
	  card-last-reviewed:: 2022-05-08T19:18:03.198Z
		- open: accesible to all
		- distributed: no single party control
		- efficient: fast and scalable
		- verifiable: everyone can check the validity of information.
		- permanent: the info is persistent
- What are Centralized vs Decentralized vs Distributed architectures? #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-05-11T18:30:00.000Z
  card-last-reviewed:: 2022-05-11T16:11:21.507Z
  card-last-score:: 1
  collapsed:: true
	- Centralized: complete reliance on single point. it is not safe
	- Decentralized: multiple points of coordination.
	- Distributed: everyone collectively execute the job
- Every node maintains a local copy of the global data-sheet.
  collapsed:: true
	- we call this a Public Ledger.
		- a database of "historical information" available to everyone is called {{cloze public ledger}} #card
		  card-last-interval:: 4
		  card-repeats:: 1
		  card-ease-factor:: 2.6
		  card-next-schedule:: 2022-05-11T20:20:57.888Z
		  card-last-reviewed:: 2022-05-07T20:20:57.888Z
		  card-last-score:: 5
		- Example: say, the historical info of banking transactions, the old transactions are used to validate the new transactions.
		- We need to ensure a no. of different aspects in this public ledger.
			- Protocols for commitment: ensure that every valid transaction from the clients are committed and included in the blockchain within a finite time.
			- Consensus: ensure that the local copies are consistent and updated.
			- Security: the data needs to be tamper proof. note that the clients may act maliciously or can be compromised.
			- Privacy and Authenticity: the data (or transactions) belong to various clients; privacy and authenticity needs to be ensured.
	- the system ensures consistency among the local copies.
- Fundamentals of blockchain
  collapsed:: true
	- Cryptographically secured hash functions
		- Hash functions: map any sized data to a fixed size. H(x)=x%n. where x and n are integers and % is the remainder after dividing by n. H(x) is within range [0,n-1]
		- Cryptographically secured: given a x. H(x) can be computed but, given H(x) x cannot be computed.
			- x is called message and H(x) is called message digest.
			- a small change in data results in a significant change in output, called {{cloze Avalanche Effect}} #card
			  card-last-interval:: 4
			  card-repeats:: 1
			  card-ease-factor:: 2.36
			  card-next-schedule:: 2022-05-14T10:29:42.045Z
			  card-last-reviewed:: 2022-05-10T10:29:42.046Z
			  card-last-score:: 3
			- the first use of cryptographically secured chain of blocks was in 1991 <ins>Time-Stamp a digital document</ins> by <ins>Harber and Stornetta</ins>
	- Merkle trees, Ralph Merkle. in 1979. aka {{cloze hash trees}}
		- Every leaf node is labeled with the hash of a data block.
		- Every non leaf node is labeled with the cryptographic hash of the labels of its child nodes.
		- ![Screenshot (16).png](../assets/Screenshot_(16)_1652437959505_0.png)
		- Bayer, Harber and Stornetta used Merkle tree in 1992 for timestamping and verifying a digital document
			- Improved the efficiency by combining timestamping of several documents into one block.
		- Other users of Merkle tree.
			- Peer to peer networks. Data blocks received in undamaged and unaltered. Other peers do not lie about a block.
			- ((627d27d4-7bee-4aea-8fad-d44d6afc5596)) implementation shared information are unaltered. No one can lie about a transaction.
		-
- Bitcoin
  id:: 627d27d4-7bee-4aea-8fad-d44d6afc5596
	- Bitcoin is a completely decentralized peer to peer permission less cryptocurrency put forth in 2009. #card #defination
	  card-last-interval:: 4
	  card-repeats:: 1
	  card-ease-factor:: 2.36
	  card-next-schedule:: 2022-05-14T10:28:38.605Z
	  card-last-reviewed:: 2022-05-10T10:28:38.605Z
	  card-last-score:: 3
		- Completely decentralized. No central party for ordering or recording anything.
		- Peer to peer. Software that runs on machines of all stakeholders to form the system.
		- Permission less. No identity, no need to sign up anywhere to use, no access control. Anyone can participate in any role.
		-
- Coursera
  collapsed:: true
	- Blockchain can be defined as a {{cloze decentralized database}}  with {{cloze strong consistency support}}. #card #defination
	  card-last-interval:: 4
	  card-repeats:: 2
	  card-ease-factor:: 2.6
	  card-next-schedule:: 2022-05-12T19:20:20.412Z
	  card-last-reviewed:: 2022-05-08T19:20:20.412Z
	  card-last-score:: 5
	- Bitcoin enabled a {{cloze decentralized system}} for exchange of value #card
	  card-last-interval:: 4
	  card-repeats:: 2
	  card-ease-factor:: 2.6
	  card-next-schedule:: 2022-05-14T10:29:56.235Z
	  card-last-reviewed:: 2022-05-10T10:29:56.235Z
	  card-last-score:: 5
	- Transaction confirmation is independently performed by all miner nodes. True or False? {{cloze True}} #card
	  card-last-interval:: 4
	  card-repeats:: 1
	  card-ease-factor:: 2.6
	  card-next-schedule:: 2022-05-11T20:20:09.538Z
	  card-last-reviewed:: 2022-05-07T20:20:09.538Z
	  card-last-score:: 5
	- The algorithm for consensus in the Bitcoin blockchain is called {{cloze Proof of Work}} protocol. #card
	  card-last-interval:: 4
	  card-repeats:: 1
	  card-ease-factor:: 2.6
	  card-next-schedule:: 2022-05-11T20:19:58.140Z
	  card-last-reviewed:: 2022-05-07T20:19:58.140Z
	  card-last-score:: 5
	- Transaction 0 in every block in the bitcoin blockchain {{cloze is called the coinbase transaction, does not have any input UTXO and is for paying the miner fees.}} #card
	  card-last-interval:: 4
	  card-repeats:: 2
	  card-ease-factor:: 2.36
	  card-next-schedule:: 2022-05-14T10:31:04.730Z
	  card-last-reviewed:: 2022-05-10T10:31:04.731Z
	  card-last-score:: 3
	- What/Who are miners in a blockchain? {{cloze Computers that validate and process blockchain transactions and solve the cryptographic puzzle to add new blocks }} #card
	  card-last-interval:: 4
	  card-repeats:: 1
	  card-ease-factor:: 2.36
	  card-next-schedule:: 2022-05-12T19:17:09.318Z
	  card-last-reviewed:: 2022-05-08T19:17:09.318Z
	  card-last-score:: 3
	- What are UTXOs in a Bitcoin 
	  card-last-interval:: 4
	  card-repeats:: 1
	  card-ease-factor:: 2.36
	  card-next-schedule:: 2022-05-12T19:16:06.911Z
	  card-last-reviewed:: 2022-05-08T19:16:06.911Z
	  card-last-score:: 3
	  Blockchain? {{cloze These form the inputs and outputs for transactions  }} #card
	- What is the genesis block? {{cloze The first block of a Blockchain}} #card
	  card-last-interval:: 4
	  card-repeats:: 1
	  card-ease-factor:: 2.36
	  card-next-schedule:: 2022-05-12T19:16:36.510Z
	  card-last-reviewed:: 2022-05-08T19:16:36.510Z
	  card-last-score:: 3
	- Solidity has data, functions or methods with modifiers, along with getter and setter functions. True or False? {{cloze True}} #card
	- What allows for the execution of code in the Ethereum Blockchain, while enhancing the basic value transfer capability of the Bitcoin Blockchain? {{cloze Smart Contracts}} #card
	- How many types of accounts are on Ethereum? {{cloze There are two types of Accounts: Externally Owned Accounts and Contract Accounts.}} #card
	- The {{cloze accounts (address)}} can send transactions for ether transfer or they can send transactions to invoke a smart contract code. #card
	- What is the smallest denomination of cryptocurrency on Ethereum? {{cloze Wei}} #card