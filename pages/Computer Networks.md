- ## What is a network? #card
  card-last-interval:: 4
  card-repeats:: 2
  card-ease-factor:: 2.46
  card-next-schedule:: 2022-05-20T19:54:59.492Z
  card-last-reviewed:: 2022-05-16T19:54:59.493Z
  card-last-score:: 5
	- A network is a collection of devices connected to each other to allow sharing of data. #defination
- ## Types of network topology. {{cloze 6}} types
  collapsed:: true
	- STAR
		- Start topology is a network topology in which all the nodes are connected to a single device known as central device.
		- Start topology requires more cable. As compared to other top topologies and therefore it is more robust. Because if a single cable is failed. Then the entire network is not compromised.
		- If the central device is damaged, the whole network fails.
		- It is the easiest to install. And troubleshoot and therefore it is widely used in homes and offices.
	- RING
		- In this topology, the nodes are connected by exactly 2 nodes. And therefore they form a single continuous transmission path.
		- Ring topology does not need a central server.
		- If a single node is failed the entire network collapses.
		- Examples: sonet network, sdh network etc.
	- BUS
		- In this topology, all the nodes are connected by a single cable known as the bus.
		- If a device wants to send the data to other device then the message is transmitted to the bus.
		- If the bus is damaged, the whole network fails.
	- MESH
		- In this topology, all the nodes are individually connected to other nodes.
		- It does not need a central switch or hub.
		- 2 types:
			- Fully connected. In this topology: Every node is connected individually to every other node.
			- Partially connected: In this topology, every node is not connected to every other node
		- It is expensive to install as the cables are required in bulk.
	- TREE
		- It is the combination of star and bust topologies.
		- All the star networks are connected by a single bus.
		- If the bus is damaged, the entire network fails.
		- But if a star network is damaged, then only that segment fails.
	- HYBRID
		- As the name suggests. The hybrid topology is a combination of different topologies.
		- It provides flexibility.
- ## OSI (Open System Interconnections)
	- It is a network architecture model based on the ISO standards.
	- It is called the OSI model as it deals with connecting the systems that are open for communication with other systems.
	- The OSI model has seven layers. The principles used to arrive at the seven layers can be summarized briefly as below.
		- Create a new layer if a different abstraction is needed.
		- Each layer should have a well defined function.
		- The function of each layer is chosen based on internationally standardized protocols.
	- ### The seven layers.
		- A Penguin said that nobody drinks Pepsi. #mnemonic
		- Application layer.
			- Application layer enables the user to access the network.
			- It is the topmost layer of the OS I reference model.
			-