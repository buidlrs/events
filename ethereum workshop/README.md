# Workshop slide

[google drive slides](https://docs.google.com/presentation/d/1WGOnMhJYl62mlR3V2SMC9ul01du2OIu_hNPPxAk6j0g/edit?usp=sharing)

# Workshop prerequisites

* Although you can work on any platform (Windows, Mac OSX, Linux), a **Debian** based operating system (Ubuntu, Linux Mint, Kali) is preferred

   
* It would be great if you also setup a latest version of `nodejs` and `npm`. Here is a [install guide](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-16-04) for Ubuntu system.


* You can go ahead and complete the Ethereum ecosystem setup if you want to come prepared.


# Setup the Ethereum ecosystem

The Ethereum  ecosystem can be setup locally for development purpose or we can connect to a real blockchain.
The local blockchain can be setup using an in-memory blockchain called Ganache.

Make sure that you have a latest version of `nodejs` and `npm`. Here is a [install guide](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-16-04) for Ubuntu system.

## Install local blockchain (Ganache)

Ganache is not a dependency of the application. So it needs to be installed explictly and globally.

`npm install ganache-cli web3@0.20.2`


## Install mainnet/testnet blockchain client (Optional)

Mac OSX:
```
brew tap ethereum/ethereum
brew install ethereum
```

Ubuntu:

```
sudo apt-get install software-properties-common
sudo add-apt-repository -y ppa:ethereum/ethereum
sudo apt-get update
sudo apt-get install ethereum
```

## Run the Ethereum node:

```
geth --rinkeby --syncmode "fast" --rpc --rpcapi db,eth,net,web3,personal --cache=1024  --rpcport 8545 --rpcaddr 127.0.0.1 --rpccorsdomain "*"
```

# Setup a development environment

We can start the Ethereum development from scratch or use an existing framework such as truffle.
 

## Truffle framework

Truffle framework makes the development and deployment process smoother by creating a framework for development.
Truffle framework will help to easily create and deploy the DApp.

```
npm install -g truffle

```

Create an issue if there is any flaw in the documentation or the contract.

You are also welcome to contribute to the project:

* Create a feature issue

* Fork the repo

* Commit your changes with appropriate message and also point the created issue

    Ex: fixes proof of ownership contract: issue #1

* Create a Pull request (PR) from your repo to this repo

* Point the issue in a comment of the PR.


Thanks! 
  
