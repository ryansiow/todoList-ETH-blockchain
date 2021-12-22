# Todo List Dapp powered by ETH blockchain

## Tech stack
- Geth: Ethereum client
- Truffle: Backend development
- Ganache: Instantly create a private blockchain (for fast development purpose)
- Metamask: web browser extension to handle wallets (eth addresses)
- NodeJS to build the frontend

In order to successfully run this Dapp, you will need to downloads all the frameworks mentioned above:
- Geth: https://geth.ethereum.org/docs/install-and-build/installing-geth
- Truffle: http://trufflesuite.com/docs/truffle/getting-started/installation
- Ganache: http://trufflesuite.com/docs/ganache/quickstart.html
- Metamask: https://metamask.io/


## Commands
1. To run, make sure you have a private blockchain up and running thanks to ganache. The installation is straight forward:
  - hostname: 127.0.0.1
  - port number: 7545
  - network id: anything you want
  - automine: true
  - error on transaction failure: true
  - hardfork: Muir Glacier

2. In the truffle-config.js, change the address at line 50 to the first address you see in your private blockchain instantiation.
3. Connect this address to your Metamask wallet. Check this [link](https://metamask.zendesk.com/hc/en-us/articles/360043227612-How-to-add-a-custom-network-RPC) to see how to add a custom network RPC.  
4. run `truffle migrate` it will upload the smart contracts to the blockchain
5. run `npm run dev` to launch the frontend.

If you make some change in the smart contract, you can do `truffle migrate --reset`
