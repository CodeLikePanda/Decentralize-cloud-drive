This is an Dcentralized cloud stroage application written in React.js, node.js, Express.js, Hardhat

Process to follow while deploying this application:
1. Download or Clone repository in your local envirment.
2. Download all dependencies:
2.1 In terminal at directory 6sem_project type: npm i
2.2 In terminal at directory ./client/ type: npm i
3. Use following commands in terminal:
3.1 npx hardhat run --network localhost scripts/deploy.js (copy generated address, we will call it smart_contract_address)
3.2 npx hardhat node
3.3 Inside ./client/ npm start (this step will work after whole step 4 completion )
4. Download metamask extension in your browser
4.1 Set new network manually in metamask with following details
4.1.1 netowrk name: Hardhat
4.1.2 new rpc url: http://127.0.0.1:8545/
4.1.3 chain id: 1337
4.1.4 currency symbol: Eth
4.2 Set metamask account
4.2.1 Open terminal where you exceuted npx hardhat node command.
4.2.2 Copy any address private key and add it at "add account" in metamask
4.2.3 Select "import account" and paste the following private key
4.2.4 Now you are all set with metamask account
5. Copy smart_contract_address and paste it at location: ./client/scr/App.js in varaible "contractAddress"
6. refresh all pages and terminal.
7. Open website using react.js and you are all set...


Smart contract is at ./contract/Upload.sol written in solidity, to test smart contract use: Remix IDE
