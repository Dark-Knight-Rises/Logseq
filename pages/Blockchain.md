- A decentralized computation and information sharing platform that enables multiple authoritative domains, who do not trust each other, to cooperate, coordinate and collaborate in a rational decision making process. #defination #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-05-09T18:30:00.000Z
  card-last-reviewed:: 2022-05-08T19:19:47.549Z
  card-last-score:: 1
- A blockchain is an <ins>open</ins>, <ins>distributed ledger</ins>  that can record transactions between two parties <ins>efficiently</ins>  and in a <ins>verifiable</ins> and <ins>permanent</ins> way. (lansiti, lakhani 2017) #defination #card
  card-last-interval:: 4
  card-repeats:: 2
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-05-12T19:18:03.198Z
  card-last-reviewed:: 2022-05-08T19:18:03.198Z
  card-last-score:: 3
	- open: accesible to all
	- distributed: no single party control
	- efficient: fast and scalable
	- verifiable: everyone can check the validity of information.
	- permanent: the info is persistent
- Centralized vs Decentralized vs Distributed architectures
  collapsed:: true
	- Centralized: complete reliance on single point. it is not safe
	- Decentralized: multiple points of coordination.
	- Distributed: everyone collectively execute the job
- Blockchain can be defined as a {{cloze decentralized database}}  with {{cloze strong consistency support}}. #card #defination
  card-last-interval:: 4
  card-repeats:: 2
  card-ease-factor:: 2.6
  card-next-schedule:: 2022-05-12T19:20:20.412Z
  card-last-reviewed:: 2022-05-08T19:20:20.412Z
  card-last-score:: 5
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
		- Example: say, the historical info if of banking transactions, the old transactions are used to validate the new transactions.
		- We need to ensure a no. of different aspects in this public ledger.
			- Protocols for commitment: ensure that every valid transaction from the clients are committed and included in the blockchain within a finite time.
			- Consensus: ensure that the local copies are consistent and updated.
			- Security: the data needs to be tamper proof. note that the clients may act maliciously or can be compromised.
			- Privacy and Authenticity: the data (or transactions) belong to various clients; privacy and authenticity needs to be ensured.
	- the system ensures consistency among the local copies.
- Fundamentals of blockchain
	- cryptographically secured hash functions
		- Hash functions: map any sized data to a fixed size. H(x)=x%n. where x and n are integers and % is the remainder after dividing by n. H(x) is within range [0,n-1]
		- Cryptographically secured: given a x. H(x) can be computed but, given H(x) x cannot be computed.
			- x is called message and H(x) is called message digest.
			- a small change in data results in a significant change in output, called {{cloze Avalanche Effect}} #card
			- the first use of cryptographically secured hash functions
- Coursera
  collapsed:: true
	- Bitcoin enabled a {{cloze decentralized system}} for exchange of value #card
	  card-last-interval:: -1
	  card-repeats:: 1
	  card-ease-factor:: 2.5
	  card-next-schedule:: 2022-05-09T18:30:00.000Z
	  card-last-reviewed:: 2022-05-08T19:15:50.734Z
	  card-last-score:: 1
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
	  card-last-interval:: -1
	  card-repeats:: 1
	  card-ease-factor:: 2.5
	  card-next-schedule:: 2022-05-09T18:30:00.000Z
	  card-last-reviewed:: 2022-05-08T19:19:11.999Z
	  card-last-score:: 1
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