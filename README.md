<p align="center"> 
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=js,python" />
  </a>
</p>

#Content#

1) **new.log** and **private-keys.log** contain the Ethereum wallet addresses and private keys generated using the Ethereumjs library: ethereumjs-wallet (see https://github.com/ethereumjs/ethereumjs-wallet)
2) All generation_.js files create pre-signed transactions from the wallet addresses in **new.log** and private keys in **private-keys.log** that deploy and invoke functions in smart contracts. We used the: ethereumjs-tx library (https://github.com/ethereumjs/ethereumjs-tx) to create pre-signed transactions. Creating pre-signed transactions allows the reliable evaluation of blockchains as the time to sign a transaction is disregarded.
3) We need to ensure the accounts in the genesis block matches the pre-signed transaction's "from" address, for the transactions to be committed. Therefore, we create a custom genesis.json with the sole Python file in this repository.

*We hope this repository helps you write your own Web3js code that enables you in evaluating your smart contracts and blockchain.* 
