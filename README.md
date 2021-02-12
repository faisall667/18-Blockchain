# 18-Blockchain
ZBank is interested in blockchain technology and I was assigned to create our own chain and to send test coins on the blockchain. 

We will be using the pupeth tool to create the blockchain;

First we will initialize the puppeth tool; 

![](Screenshots/1%20Initialize%20puppeth.png)

Then we named the network; chose "Configure a new Network" and created a genesis block by choosing option 1: "Create new genesis from scratch".
We made a few attempts to make this network work, the first chain we called was "wonder" and the second one was called "themotherload"

To verify transactions we will be choosing 2. "Clique - proof of authority" 

Then we seal the account by pasting addresses from application called MyCrypto which is the wallet that contains addresses to which you can attach a particular cryptocurrency.  

![](Screenshots/2%20gen%20block%20proof%20of%20auth%20seal.png)

Next we set up our chain/network ID and export the genesis configurations in json files so we can access them on wonder/themotherload network.

![](Screenshots/3%20Manage%20genesis%20block.png)

Now that we have created our blocks we will initialize them using geth using:
  ./geth --datadir node1 init themotherload.json
./geth --datadir node2 init themotherload.json

Next we would mine the blocks using geth command and sealer addresses

![](Screenshots/4%20Mine%20blocks.png)

Now that the blockchain is running we will test it out using Mycrypto 

After opening Mycrypto, we will change network and create a custom node

![](Screenshots/5%20Create%20custom%20node.png)

Now we can send transactions on our private blockchain






