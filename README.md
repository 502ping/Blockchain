# Description
A class group project, realize a blockchian system with python 3.0 and pickledb. Functions are added like mine blocks, add transactions,  consensus and get blocks. 

# System structure
This blockchain system can be divided into three layers. 
## First layer – user interface	Nodes can log in and log out.	
Nodes can perform different operations by sending HTTP requests with data in JSON format. Nodes can also see response message in the Postman. For example, nodes can mine a new block via “/mine” and get a response about the information of the new block.
## Second layer – main structure of the blockchain and routes for receiving nodes’ requests	
Set different routes to receive HTTP requests and invoke corresponding back-end Python functions. After that, reply the node with data in JSON format. The back-end Python functions will be invoked to deal with the service logic and execute database operations.
## Third layer – data persistence	
pickleDB can store the blockchain data in the disk.

# Development environment
## Programming language
Python 3.6.
## Python packages
Flask 1.0.2 and requests 2.20.1.
## Database
pickleDB 0.8.1.
## Operation system
Windows 10 64bit build 1803 and macOS High Sierra 10.13.6.
## Integrated Development Environment
PyCharm Professional Edition 2018.2.
## Other tool(s)
Postman 6.5.3.

# HTTP request
All the operations are implemented via sending HTTP requests. Nine routes have been defined for different operations:
(1) /restart	Reset your own blockchain.
(2) /nodes/register	Registration for new nodes.
(3) /transactions/new	Create a new transaction.
(4) /mine	Mine a new block
(5) /chain	View your own blockchain information.
(6) /pool	View the current transactions pool information.
(7) /nodes/resolve	Solve conflicts with other nodes.
(8) /getblocks	Get other nodes’ blockchain information.
(9) /inv	Tell the requester about its own blockchain information. 

# Author and distribution
## XIA Yuchen
Network – realize the interactions among different nodes.
## HUANG Kaihang
Project solution and project framework – choose the appropriate technology and tools for the project.
Flask web application framework – use Flask to set up routes for different HTTP requests to invoke back-end functions.
Data persistence – store the data in the disk.
## ZENG Lin
Blockchain prototype – construct the blockchain system according to the requirements.
## HU Weihua
Mining – implement a fixed-difficulty Proof-of-Work algorithm

# Notice
