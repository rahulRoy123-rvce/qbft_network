HOW TO SET UP A QBFT NETWORK
This guide will walk you through the steps of setting up a QBFT network using the Quorum Developer Quickstart.

PREREQUISITES
Docker and Docker Compose
Node.js version 12 or higher
Truffle
cURL command line
MetaMask

GENERATE THE TUTORIAL BLOCKCHAIN CONFIGURATION FILES
Run the following command:
npx quorum-dev-quickstart
Follow the prompts displayed to run Hyperledger Besu and logging with ELK. Enter n for Codefi Orchestrate and private transactions.

START THE NETWORK
In the directory where you generated the tutorial blockchain configuration files, run the following command:

docker-compose up
Connect to the Network
Open MetaMask and select the Custom RPC network.

ENTER THE FOLLOWING INFORMATION:

Network name: QBFT Network
Chain ID: 101
RPC URL: http://localhost:8545
Username: any username
Password: any password

DEPLOY A SMART CONTRACT
In a terminal window, navigate to the directory where you cloned the example smart contract repository.
Run the following command to deploy the smart contract:
truffle deploy

INTERACT WITH THE SMART CONTRACT
In MetaMask, you should now see the deployed smart contract.
You can interact with the smart contract by sending transactions to it.
For More Information
For more detailed instructions, please refer to: https://besu.hyperledger.org/stable/private-networks/tutorials/qbft .

Reminder: This tutorial runs a private network suitable for education or demonstration purposes and is not intended for running production networks.

ADDITIONAL NOTES
The npx quorum-dev-quickstart command will create a directory called qbft-network. This directory contains all of the files and folders you need to run the QBFT network.
The docker-compose up command will start the QBFT network. This may take a few minutes to complete.
Once the network is started, you can connect to it using MetaMask.
To deploy a smart contract, you will need to have the example smart contract repository cloned locally.
To interact with the smart contract, you can send transactions to it using MetaMask.