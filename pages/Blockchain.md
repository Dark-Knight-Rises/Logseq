- ## What is Blockchain? #card
  card-last-interval:: 4.43
  card-repeats:: 2
  card-ease-factor:: 2.6
  card-next-schedule:: 2022-05-21T05:53:06.562Z
  card-last-reviewed:: 2022-05-16T19:53:06.562Z
  card-last-score:: 5
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
- ### What is a Block? #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-05-20T18:30:00.000Z
  card-last-reviewed:: 2022-05-19T19:45:16.626Z
  card-last-score:: 1
	- A block is a container data structure that contains a series of transactions.
	- Structure of a Block. Reference ((627d27d4-7bee-4aea-8fad-d44d6afc5596))
		- Block header
			- Metadata about a block.
				- Every block inherits from the previous block. We use previous block's hash to create the new block's hash, to make the blockchain tamper proof.
				- Mining statistics used to construct the block.
				- ((62815db8-e5e9-4072-abd6-b9c02584cf3e)) root.
		- List of transactions
	- In ((627d27d4-7bee-4aea-8fad-d44d6afc5596))
		- A block may contain more than 500 transactions on average. The average size of a block is around 1 MB (an upper bound proposed by Satoshi Nakamoto in 2010).
		- May grow up up to 8 MB or sometimes higher.
		- Larger blocks can help in processing large number of transactions in one group.
- ### What are Centralized vs Decentralized vs Distributed architectures? #card
  card-last-interval:: 10.8
  card-repeats:: 3
  card-ease-factor:: 2.7
  card-next-schedule:: 2022-05-30T14:47:46.423Z
  card-last-reviewed:: 2022-05-19T19:47:46.424Z
  card-last-score:: 5
  collapsed:: true
	- Centralized: complete reliance on single point. it is not safe
	- Decentralized: multiple points of coordination.
	- Distributed: everyone collectively execute the job
- ### Public Ledger
  collapsed:: true
  id:: 62815db8-9249-48af-8574-2f94b3c0e028
	- It is a database of "historical information" available to everyone is called {{cloze public ledger}}
	  card-last-score:: 5
	  card-repeats:: 2
	  card-next-schedule:: 2022-05-18T09:21:58.355Z
	  card-last-interval:: 4
	  card-ease-factor:: 2.7
	  card-last-reviewed:: 2022-05-14T09:21:58.355Z
	- Example: say, the historical info of banking transactions, the old transactions are used to validate the new transactions.
	- We need to ensure a no. of different aspects in this public ledger, total {{cloze 4}}
		- Protocols for commitment
			- Ensure that every valid transaction from the clients are committed and included in the blockchain within a finite time.
		- Consensus
			- Ensure that the local copies are consistent and updated.
		- Security
			- The data needs to be tamper proof. note that the clients may act maliciously or can be compromised.
		- Privacy and Authenticity
			- The data (or transactions) belong to various clients; therefore privacy and authenticity needs to be ensured.
- ### Fundamentals of blockchain
	- <ins> Cryptographically secured Hash functions</ins>
		- Cryptographically secured
			- Let's say 'x' is a message and H(x) is called message digest.
			- Given a x. H(x) can be computed but, given H(x) x cannot be computed.
			- A small change in data results in a significant change in output, called {{cloze Avalanche Effect}} #card
			  card-last-interval:: 4
			  card-repeats:: 2
			  card-ease-factor:: 2.46
			  card-next-schedule:: 2022-05-20T19:51:04.001Z
			  card-last-reviewed:: 2022-05-16T19:51:04.002Z
			  card-last-score:: 5
		- Hash functions
			- Map any sized data to a fixed size. H(x)=x%n. where x and n are integers and % is the remainder after dividing by n. H(x) is within range [0,n-1]
		- The first use of cryptographically secured chain of blocks was in 1991 <ins>Time-Stamp a digital document</ins> by <ins>Harber and Stornetta</ins>
	- Merkle trees
	  id:: 62815db8-e5e9-4072-abd6-b9c02584cf3e
		- Ralph Merkle. in 1979. aka {{cloze hash trees}}
		- Every leaf node is labeled with the hash of a data block.
		- Every non leaf node is labeled with the cryptographic hash of the labels of its child nodes.
		- ![Screenshot (16).png](../assets/Screenshot_(16)_1652437959505_0.png)
		- Bayer Harber and Stornetta used Merkle tree in 1991 for timestamping and verifying a digital document
			- Improved the efficiency by combining timestamping of several documents into one block.
		- Other uses of Merkle tree.
			- Peer to peer networks.
				- Data blocks received are undamaged and unaltered. Other peers do not lie about a block.
			- ((627d27d4-7bee-4aea-8fad-d44d6afc5596)) implementation
				- Shared information is unaltered. No one can lie about a transaction.
		-
- ## Bitcoin
  id:: 627d27d4-7bee-4aea-8fad-d44d6afc5596
	- Bitcoin is a completely decentralized peer to peer permission less cryptocurrency put forth in 2009. #card #defination
	  card-last-interval:: 4
	  card-repeats:: 2
	  card-ease-factor:: 2.22
	  card-next-schedule:: 2022-05-20T19:50:36.192Z
	  card-last-reviewed:: 2022-05-16T19:50:36.192Z
	  card-last-score:: 3
		- Completely decentralized. No central party for ordering or recording anything.
		- Peer to peer. Software that runs on machines of all stakeholders to form the system.
		- Permission less. No identity, no need to sign up anywhere to use, no access control. Anyone can participate in any role.
	- The Bitcoin Transaction lifecycle.
		- The Sender
		  collapsed:: true
			- 'A' opens his Bitcoin wallet.
			- Provides the address of 'B' and the amount to transfer and hits send.
		- The Network
			- The wallet constructs the transaction. Digitally signs using A's private key and broadcasts it to the network.
			- The network nodes validate the transaction based on the existing blockchain and propagate the transaction to the miners.
			- ((627e3823-ddf7-43fc-aece-6aba09957784)) include the transaction to the next block to be mined.
		- The Miners
		  id:: 627e3823-ddf7-43fc-aece-6aba09957784
			- The miners collect all the transactions for the time duration, say for 10 minutes.
			- They construct a new block and try to connect it with the existing blockchain through a cryptographic hash function. Which is known as the {{cloze Mining Procedure}}
			- Once the mining is over and the hash is obtained, the block is included in the existing blockchain.
				- The updated blockchain is then propagated in the network.
		- The Receiver
			- 'B' opens his Bitcoin wallet and refreshes, the blockchain gets updated.
			- The transaction reflects at 'B's wallet.
	-
- ## Smart Contracts
	- The term was coined by Nick Szabo in 1996
		- He claimed that smart contracts can be realized with the help of a ((62815db8-9249-48af-8574-2f94b3c0e028))
		- Smart Contracts can be realized using blockchain
	- Example
		- Contracts in a Centralized Platform - (Crowdfunding)
			- You have an interesting project, but you do not have sufficient money to execute the project.
			- Submit the project in a crowdfunding platform.
			- Multiple supporters commit to support the project with small funds.
			- The platform ensures that you get the complete money if the project is successful.
		- Problems with this Centralized platform
			- Both the product team and the supporters need to trust the crowdfunding platform.
			- The product team expects the money to get paid based on the project progress.
			- The supporters expect the money to go to the project.
			- However, the crowdfunding platform, the middleman, takes significant charge to manage the entire process.
		- How can Smart Contracts solve these problems?
			- The contract is written in code which is available to all the stakeholders, the supporter and the product team. We can see an application of blockchain here.
			- If the project fails, then the code will transfer the money back to the supporter's account.
		- Advantages of using Smart Contracts
			- Immutable
				- No party will be able to change the contract once it is fixed and written to the ((62815db8-9249-48af-8574-2f94b3c0e028)) , the blockchain.
			- Distributed
				- All the steps of the contract can be validated by every participating party. No one can claim later that the contract was not validated.
	- Platforms
		- Ethereum
		- Rootstock
		- Hyperledger
		- Ripple
- ## Coursera
	- Blockchain can be defined as a {{cloze decentralized database}}  with {{cloze strong consistency support}}. #card #defination
	  card-last-interval:: 9.84
	  card-repeats:: 3
	  card-ease-factor:: 2.46
	  card-next-schedule:: 2022-05-24T05:22:48.735Z
	  card-last-reviewed:: 2022-05-14T09:22:48.735Z
	  card-last-score:: 3
	- Bitcoin enabled a {{cloze decentralized system}} for exchange of value #card
	  card-last-interval:: 10.8
	  card-repeats:: 3
	  card-ease-factor:: 2.7
	  card-next-schedule:: 2022-05-27T14:51:14.226Z
	  card-last-reviewed:: 2022-05-16T19:51:14.226Z
	  card-last-score:: 5
	- Transaction confirmation is independently performed by all miner nodes. True or False? {{cloze True}} #card
	  card-last-interval:: 10.24
	  card-repeats:: 3
	  card-ease-factor:: 2.56
	  card-next-schedule:: 2022-05-30T00:48:11.471Z
	  card-last-reviewed:: 2022-05-19T19:48:11.471Z
	  card-last-score:: 3
	- The algorithm for consensus in the Bitcoin blockchain is called {{cloze Proof of Work}} protocol. #card
	  card-last-interval:: 11.2
	  card-repeats:: 3
	  card-ease-factor:: 2.8
	  card-next-schedule:: 2022-05-30T23:48:00.700Z
	  card-last-reviewed:: 2022-05-19T19:48:00.700Z
	  card-last-score:: 5
	- Transaction 0 in every block in the bitcoin blockchain {{cloze is called the coinbase transaction, does not have any input UTXO and is for paying the miner fees.}} #card
	  card-last-interval:: 9.84
	  card-repeats:: 3
	  card-ease-factor:: 2.46
	  card-next-schedule:: 2022-05-26T15:51:49.305Z
	  card-last-reviewed:: 2022-05-16T19:51:49.305Z
	  card-last-score:: 5
	- What/Who are miners in a blockchain? {{cloze Computers that validate and process blockchain transactions and solve the cryptographic puzzle to add new blocks }} #card
	  card-last-interval:: 8.32
	  card-repeats:: 3
	  card-ease-factor:: 2.08
	  card-next-schedule:: 2022-05-28T02:49:26.997Z
	  card-last-reviewed:: 2022-05-19T19:49:26.997Z
	  card-last-score:: 3
	- What are UTXOs in a Bitcoin 
	  card-last-interval:: 9.28
	  card-repeats:: 3
	  card-ease-factor:: 2.32
	  card-next-schedule:: 2022-05-29T01:48:25.079Z
	  card-last-reviewed:: 2022-05-19T19:48:25.079Z
	  card-last-score:: 3
	  Blockchain? {{cloze These form the inputs and outputs for transactions  }} #card
	- What is the genesis block? {{cloze The first block of a Blockchain}} #card
	  card-last-interval:: -1
	  card-repeats:: 1
	  card-ease-factor:: 2.22
	  card-next-schedule:: 2022-05-20T18:30:00.000Z
	  card-last-reviewed:: 2022-05-19T19:48:49.556Z
	  card-last-score:: 1
	- Solidity has data, functions or methods with modifiers, along with getter and setter functions. True or False? {{cloze True}} #card
	  card-last-interval:: 4
	  card-repeats:: 2
	  card-ease-factor:: 2.7
	  card-next-schedule:: 2022-05-23T19:47:05.162Z
	  card-last-reviewed:: 2022-05-19T19:47:05.162Z
	  card-last-score:: 5
	- What allows for the execution of code in the Ethereum Blockchain, while enhancing the basic value transfer capability of the Bitcoin Blockchain? {{cloze Smart Contracts}} #card
	  card-last-interval:: 4.43
	  card-repeats:: 2
	  card-ease-factor:: 2.6
	  card-next-schedule:: 2022-05-21T05:54:44.688Z
	  card-last-reviewed:: 2022-05-16T19:54:44.688Z
	  card-last-score:: 5
	- How many types of accounts are on Ethereum? {{cloze There are two types of Accounts: Externally Owned Accounts and Contract Accounts.}} #card
	  card-last-interval:: -1
	  card-repeats:: 1
	  card-ease-factor:: 2.5
	  card-next-schedule:: 2022-05-20T18:30:00.000Z
	  card-last-reviewed:: 2022-05-19T19:46:47.951Z
	  card-last-score:: 1
	- The {{cloze accounts (address)}} can send transactions for ether transfer or they can send transactions to invoke a smart contract code. #card
	  card-last-interval:: 3.98
	  card-repeats:: 2
	  card-ease-factor:: 2.36
	  card-next-schedule:: 2022-05-23T18:46:19.959Z
	  card-last-reviewed:: 2022-05-19T19:46:19.960Z
	  card-last-score:: 3
	- What is the smallest denomination of cryptocurrency on Ethereum? {{cloze Wei}} #card
	  card-last-interval:: -1
	  card-repeats:: 1
	  card-ease-factor:: 2.6
	  card-next-schedule:: 2022-05-20T18:30:00.000Z
	  card-last-reviewed:: 2022-05-19T19:46:55.280Z
	  card-last-score:: 1
	- {{cloze Ethereum full node}} hosts the software needed for transaction initiation, validation, mining, block creation, and smart contract execution. #card
	  card-last-interval:: 4.43
	  card-repeats:: 1
	  card-ease-factor:: 2.6
	  card-next-schedule:: 2022-05-21T05:49:41.095Z
	  card-last-reviewed:: 2022-05-16T19:49:41.095Z
	  card-last-score:: 5
	- {{cloze Miner nodes}} receive, verify, gather and execute transactions. #card
	  card-last-interval:: 4.43
	  card-repeats:: 1
	  card-ease-factor:: 2.6
	  card-next-schedule:: 2022-05-21T05:44:00.490Z
	  card-last-reviewed:: 2022-05-16T19:44:00.490Z
	  card-last-score:: 5
	- Any changes to the value of a state variable in a smart contract are stored on the blockchain. True or False? {{cloze True}} #card
	  card-last-interval:: 4.43
	  card-repeats:: 1
	  card-ease-factor:: 2.6
	  card-next-schedule:: 2022-05-21T05:43:48.301Z
	  card-last-reviewed:: 2022-05-16T19:43:48.301Z
	  card-last-score:: 5
	- What are miners who solved the puzzle but didn't win the block creation called? {{cloze Ommers}} #card
	  card-last-interval:: 4.43
	  card-repeats:: 1
	  card-ease-factor:: 2.6
	  card-next-schedule:: 2022-05-21T05:37:14.874Z
	  card-last-reviewed:: 2022-05-16T19:37:14.875Z
	  card-last-score:: 5