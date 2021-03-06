# Gameunits Gaming Blockchain Node on Ubuntu VM

This template delivers the Gameunits network to your VM in about 20 minutes. Everything you need to get started using the Gameunits blockchain from the command line is included. You may build from source. Once installed, 'gameunitsd' will begin syncing the public gaming blockchain. You may then connect via SSH to the VM and launch 'gameunitsd' to interface with the blockchain.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fgameunits-on-ubuntu%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fgameunits-on-ubuntu%2Fazuredeploy.json" target="_blank"><img src="http://armviz.io/visualizebutton.png"/></a>

![Gameunits](https://raw.githubusercontent.com/gameunits/gameunits-logos/master/artwork.png "Gameunits")

# What is Gameunits?
----------------

Gameunits is a peer-to-peer digital gaming currency with a distributed, decentralized public ledger, that unlike traditional banking systems, are viewable and easily audited by the people.
The ability to manage transactions and issue additional Gameunits is all handled by the network of users utilizing Gameunits . Because the Gameunits network is run by the people, holders of Gameunits receive a 2-25% yearly interest through a process called staking.

- 60 second block targets
- Proof of Stake blockchain security model

Services include:
- Full Gameunits Blockchain node.
- P2P communication via the TOR Network

For more information, as well as an immediately useable, binary version of
the Gameunits client sofware, see http://www.gameunits.org.


# Template Parameters

When you click the Deploy to Azure icon above, you need to specify the following template parameters:

* `adminUsername`: This is the account for connecting to your Gameunits host.
* `adminPassword`: This is your password for the host.  Azure requires passwords to have One upper case, one lower case, a special character, and a number.
* `dnsLabelPrefix`: This is used as both the VM name and DNS name of your public IP address.  Please ensure an unique name.
* `installMethod`: This tells Azure to install Gameunits from source or binarys.
* `vmSize`: This is the size of the VM to use.  Recommendations: Use the D series for installations from source.

# Getting Started Tutorial

* Click the `Deploy to Azure` icon above
* Complete the template parameters, choose your resource group, accept the terms and click Create
* Wait about 15 minutes for the VM to spin up and install the software
* Connect to the VM via SSH using the DNS name assigned to your Public IP
* Launch Gameunits run 'gameunitsd help'
