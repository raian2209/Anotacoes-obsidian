#programação 

Protocolo para validação de transações em cryptomoedas 


### Tipos de node 

1. Full nodes: 
	- Peers in the Bitcoin peer-to-peer network are programs that have both the software logic and the data necessary for them to fully verify the correctness of a new transaction. Bitcoin peers are commonly called “full verification nodes”
	- When there are multiple alternative blocks to choose from, Bitcoin full nodes choose the chain of valid blocks with the most total          **PoW** (Prof of Work), called the best blockchain.
1. Miner node: 
	- can only receive honest income from creating blocks that follow all of Bitcoin’s consensus rules. Therefore, miners are normally incentivized to only	include valid transactions in their blocks and the blocks they build upon. This allows users to optionally make a trust-based assumption that any transaction in a block is a valid transaction.
	-  currently creates new bitcoins in each block, almost like a central bank printing new money. The amount of bitcoin created per block is limited and diminishes with time, following a fixed issuance schedule. **the reward will only be collected if the miner has only included valid transactions** 
	- Transactions are added to the new block, prioritized by the highest fee rate transactions first and a few other criteria.
	- Normally, the high cost of dishonestly creating two blocks for a small additional payment is much less profitable than honestly creating a new block, making it unlikely that a confirmed transaction will be deliberately changed
	-  **By convention, any block with more than six confirmations is considered very hard to change, because it would require an immense amount of computation to recalculate six blocks (plus one new block).**



- Bitcoin Core architecture
	 ![[Screenshot from 2024-10-01 09-02-04.png]]

- Bitcoin Core Build
	-  git clone Repositorio
	-  git tag
	- git checkout v______
	- git status
	- ./autogen.sh **Para ver opções de configuração: ./configure --help**
		- ![[Screenshot from 2024-10-01 09-19-51.png]]
	-  ./configure 
		- script to automatically discover all the necessary libraries and create a customized build script for your system
	 - make 
		 - Type make to start compiling the executable application
		 - On a fast system with more than one CPU, you might want to set the number of parallel compile jobs. For instance, make -j 2 will use two cores if they are available.
		 - If all goes well, Bitcoin Core is now compiled. You should run the unit test suite with make check to ensure the linked libraries are not broken in obvious ways.
		 - **The final step is to install the various executables on your system using the make install command. You may be prompted for your user password because this step requires administrative privileges**
	 - make check && sudo make install  
		 - The default installation of bitcoind puts it in /usr/local/bin. You can confirm that Bitcoin Core is correctly installed by asking the system for the path of the executables, as follows
		 - ![[Screenshot from 2024-10-01 09-38-06.png]]
## procurar depois: 
gossiping