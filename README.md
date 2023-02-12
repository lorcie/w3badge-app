# W3BadgeContract Web3 Application

# Table of contents
1. [Introduction](#introduction)
2. [Architecture](#architecture)
3. [Project Setup](#project-setup)
4. [Configuration](#configuration)
5. [Run the w3badge App](#run-w3badge-app)
6. [Screenshots](#screenshots)
6. [Resources](#resources)

## Introduction <a name="introduction"></a>
W3BadgeContract is a Web3 application to showcase integration of custom Badge SmartContract on **Thirdweb** Portal SDK **Unity** game with **NFT** storage **IPFS** API  on **Polygon** Blockchain Environment thru **Metamask** wallet.

## Architecture <a name="architecture"></a>

![w3badge architecture](./screenshots/w3badge-architecture.png)

## Project Setup <a name="project-setup"></a>

To run this project locally, follow these steps.

1. Clone the project locally, change into the directory, and install the dependencies:

```sh
git clone https://github.com/lorcie/w3badge.git


== Unity Editor

First Installation : Follow instructions at this Thirdweb link https://blog.thirdweb.com/guides/get-started-with-thirdwebs-unity-sdk/

	- Install Thirdweb Unity SDK if needed by downloading and importing the Unity package and configure as webGL,...
	
	- Change Smart Contract Address parameter value (if new value) in Script SDKManager.cs

Open Unity Editor, select "Start Scene" and click "Build and Run"

You can now play the Unity game by clicking keyboard (Left, Right, Up, Down and Space to Jump) Inputs

== Admin Web APP

cd w3badge-contract

# install using NPM or Yarn
npm install

# or

yarn
```

## Configuration <a name="configuration"></a>

copy the `.env.sample` folder:

```
cp .env.sample .env
```

Customize the .env file with appropriate data about api url, wallet private key for each expected environment (local, test, prod,...)

```
NEXT_PUBLIC_CONTRACT_ADDRESS=
NEXT_PUBLIC_WALLET_ADDRESS=

```

### Contract Deployment on Local Environment

0. Prerequites

LOCAL TOOLS :  Remix, Metamask,  Node JS, Unity

LOCAL DEVELOPMENT

- Install Node JS to enable to install react and libraries

The development of the **Solidity** Smart Contract is facilitated with **Truffle** and **web3** javascript sdk

1. Start Ganache Tool

```sh
launch Ganachache Tool from windows app list
```

2. With the network running, deploy the contracts to the local network in a separate terminal window. You muat run with argument reset  to reinitialize the cache

```sh
truffle migrate --network development
```

### Contract Deployment on Thirdweb Portal with Polygon Mumbai Test Environment

0. PreRequisites

- on Thirdweb Portal, Create an Account if needed and Access Thirdweb Dashboard  to get your custom Ssmart Contract address

- Add this Smart Contract Address in your Application Code for Unity and Configuration Env File for NextJS Admin Frontend App.


1. ReCompile and Deploy from Scrtach the contract by configuring the  to the polygon matic network

```sh
npx deploy
```

```

## Run the W3Badge Polygon App <a name="run-w3badge-app"></a>

In main directory w3exchange folder

### Development Mode <a name="development-mode"></a>

- Run the development Application:

```bash
npm run start
```
You can then Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

### Production Mode <a name="production-mode"></a>

- You must first Build the Application

```bash
npm run build
```

## Screenshots <a name="screenshots"></a>
Unity Game>

![w3badge Unity Game](./screenshots/ComboUnityWeb3-Unity-Thirdweb.png)

Smart Contract>

![w3badge Custom Smart Contract](./screenshots/w3badgecontract-solidity.png)

Thirdweb Custom Smart Contract page>
![w3badge Thirdweb Configure mart contract](./screenshots/w3badgeContract-thirdweb-deploy-NFT.png)


Thirdweb NFT pages>

![w3badge Thirdweb NFT Explorer](./screenshots/w3badgeContract-thirdweb-deploy-NFT-explorer.png)


![w3badge Thirdweb NFT Deploy](./screenshots/w3badgeContract-thirdweb-deploy-NFT-list.png)


Metamask Wallet>

![w3ebadge Metamask Wallet](./screenshots/w3badgeContract-thirdweb-metamask.png)


Metamask Wallet Confirmed>

![w3badge thirdweb metamask wallet confirmed](./screenshots/w3badgeContract-thirdweb-metamask-confirmed.png)


## Resources <a name="resources"></a>

[ipfs nfs storage](https://nft.storage/files/)[https://nft.storage/files/]

[polygon smart contracts / accounts](https://mumbai.polygonscan.com/) [https://mumbai.polygonscan.com/]