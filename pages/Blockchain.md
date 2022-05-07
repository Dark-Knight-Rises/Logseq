- A decentralized computation and information sharing platform that enables multiple authoritative domains, who do not trust each other, to cooperate, coordinate and collaborate in a rational decision making process. #defination #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-05-08T18:30:00.000Z
  card-last-reviewed:: 2022-05-07T20:16:31.490Z
  card-last-score:: 1
- A blockchain is an <ins>open</ins>, <ins>distributed ledger</ins>  that can record transactions between two parties <ins>efficiently</ins>  and in a <ins>verifiable</ins> and <ins>permanent</ins> way. (lansiti, lakhani 2017) #defination #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-05-08T18:30:00.000Z
  card-last-reviewed:: 2022-05-07T20:20:39.031Z
  card-last-score:: 1
	- open: accesible to all
	- distributed: no single party control
	- efficient: fast and scalable
	- verifiable: everyone can check the validity of information.
	- permanent: the info is persistent
- Centralized vs Decentralized vs Distributed architectures
	- Centralized: complete reliance on single point. it is not safe
	- Decentralized: multiple points of coordination.
	- Distributed: everyone collectively execute the job
- Blockchain can be defined as a {{cloze decentralized database}}  with {{cloze strong consistency support}}. #card #defination
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-05-08T18:30:00.000Z
  card-last-reviewed:: 2022-05-07T20:16:14.581Z
  card-last-score:: 1
- Every node maintains a local copy of the global data-sheet.
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
- Coursera
	- Bitcoin enabled a {{cloze decentralized system}} for exchange of value #card
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
	  card-next-schedule:: 2022-05-08T18:30:00.000Z
	  card-last-reviewed:: 2022-05-07T20:19:49.456Z
	  card-last-score:: 1
	- What/Who are miners in a blockchain? {{cloze Computers that validate and process blockchain transactions and solve the cryptographic puzzle to add new blocks }}
	- What are UTXOs in a Bitcoin
	  Blockchain? {{cloze These form the inputs and outputs for transactions  }}
-