# Blockchain-HW
UNCC FinTech Boot Camp Blockchain Homework - Program to derive ETH and BTC testnet crypto wallets from an account, and simulate transactions using a command line interface.
## Instructions
1. Ensure that you have downloaded and installed anaconda, puppeth, geth, and MyCrypto. You will need these tools in order to access ZBank's blockchain network and crypto wallets.
2. Open your Terminal and set your virtual environment to "zbanknet" with the command: conda activate zbanknet
3. Direct to the folder in which you have geth saved
4. To initialize the first node on the blockchain, run the command: ./geth init z.json --datadir znode1
5. To initialize the first node on the blockchain, run the command: ./geth init z.json --datadir znode2
6. To start mining the first node, run the command: ./geth --datadir znode1 --mine --minerthreads 1
  The --mine flag tells the node to mine new blocks.
  The --minerthreads flag tells geth how many CPU threads, or "workers" to use during mining. Since our difficulty is low, we can   set it to 1.
7. To start mining the second node, run the command: ./geth --datadir znode2 --port 30304 --rpc --bootnodes "enode://28fe67f78d070dd9247dfad901e21fc22b974e170b6a54e19d85e63b3a4f73f14c9932a369b0c0aad55a25f0626c41e0ebce1459ca07fad6213e4413289d69d3@127.0.0.1:30303"
8. Open the MyCrypto app, and create an account if you do not already have one
9. You will need to tap into the test network, in order to set this up on your app, please configure as shown in the "network-config" image in "Screenshots"
10. Once you have set up the network on your app, go to "View & Send" in the top left, and choose "Keystore File" as your        authentication method. This will prompt you to direct to the file path of one of the crypto wallets below on your device. Select the file, and enter the password when prompted (also listed below).
11. You should now be in the wallet. In order to send ETH to the other account you are not currently in, copy and paste the receiving account's public key from below into the "To Address" input box, choose how much ETH you would like to send, and click on "Send Transaction"

## Network Information
  Network Name: solonet
  Chain ID: 8144
  Blocktime: 15
  
## Accounts
node1: PW: Von021966* Public address key:  0x014CF338BD6df07002d0b5f148D054337E22e6dB
Path of the secret key file: node1\keystore\UTC--2021-02-10T18-15-04.591470500Z--014cf             338bd6df07002d0b5f148d054337e22e6db ** Port 30303

node2: PW: Von021966* Public address key:  0xBfB9Ee628d8D40999c56C5Bb86092664F831736D
Path of the secret key file: node2\keystore\UTC--2021-02-10T18-18-41.368800500Z--bfb9ee628d8d40999c56c5bb86092664f831736d


 
