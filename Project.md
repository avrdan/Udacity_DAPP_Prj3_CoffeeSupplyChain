# Ethereum Dapp for Tracking Items through Supply Chain

The same project as the provided sample was used - Fair Trade coffee.
Therefore:

* the UML diagrams were created accordingyly
* the skeleton code was filled in with the appropriate contents
* all tests have been passed
* UX adapted so that it works on a Ganache test network

## Contract Address

Supply Chain contract address:
https://ropsten.etherscan.io/address/0xeb1b432d793a0b55e7e0089d2fc2937334523631

Please see the more detailed section below of the migration
to the Ropsten network. 

It includes all contract addresses.

## Libraries

No additional libraries used, as I started from the same project template.
IPFS was not used.

## Versions

* node: v12.18.1
* npm: v6.14.5
* Truffle: v5.1.13
* web3: web3.version returns api "0.20.7"

## Project Files

All project files are included in the nested folders.

The same file struture as in the original template has been kept.

Note that some paths had to be corrected for the frontend to work correctly.


I started the <b>index.html</b> using a <b>VS Code</b> plugin with the file selected.

The location from which the web interface is started matters, 

due to hardcoded paths towards the JS scripts (like for the <b>SupplyChain</b> contract).

## UML Documents

![ActivityDiagram](images/UML/Coffee_SupplyChain_ActivityDiagram.png)
*Activity Diagram*

![SequenceDiagram](images/UML/Coffee_Supply_Chain_SequenceDiagram.png)
*Sequence Diagram*

![StateDiagram](images/UML/Coffee_SupplyChain_State.png)
*State Diagram*

![Class Diagram](images/UML/Coffee_SupplyChain_DataModel.png)
*Class Diagram*

## Compilation and Test Results

![TestResults](images/TestResults.PNG)

## Deployment to Public Test Network (Ropsten)
```
Starting migrations...
======================
> Network name:    'ropsten'
> Network id:      3
> Block gas limit: 0x7a121d


1_initial_migration.js
======================

   Replacing 'Migrations'
   ----------------------
   > transaction hash:    0xf887f8c1e5e8718a03829a363a3567c241463afb85aa1d928761013a38952fc1
   > Blocks: 2            Seconds: 8
   > contract address:    0xfaAd56e8be34fCe16b4Ad2CE58EE32D08cD4daBE
   > block number:        9184785
   > block timestamp:     1606949556
   > account:             0x878c2B8b7F06fB0aF999A3FC96CBeC7Aa0580fb0
   > balance:             1.600030393
   > gas used:            225225
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.0045045 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:           0.0045045 ETH


2_deploy_contracts.js
=====================

   Replacing 'FarmerRole'
   ----------------------
   > transaction hash:    0x7ff44d73ea5727b080416758a3691205d7e5960a3df26e0a791b45ee30c807aa
   > Blocks: 0            Seconds: 0
   > contract address:    0xF3F020Cd92A585e3534579D2c25A305dd2eF7e1D
   > block number:        9184791
   > block timestamp:     1606949586
   > account:             0x878c2B8b7F06fB0aF999A3FC96CBeC7Aa0580fb0
   > balance:             1.593061453
   > gas used:            306084
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00612168 ETH


   Replacing 'DistributorRole'
   ---------------------------
   > transaction hash:    0x8fdc691069cc7871d3c0906301b7fb709485cfebc11b9f88670d096bd54a8473
   > Blocks: 1            Seconds: 12
   > contract address:    0x7C1b88606E02689c64a8f39AbDF3db20e30C55dD
   > block number:        9184792
   > block timestamp:     1606949588
   > account:             0x878c2B8b7F06fB0aF999A3FC96CBeC7Aa0580fb0
   > balance:             1.586940013
   > gas used:            306072
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00612144 ETH


   Replacing 'RetailerRole'
   ------------------------
   > transaction hash:    0x26d4a9f422f6424632a432e69fcb79b2ce4c9adafa82e257f3c10d2e228843a8
   > Blocks: 1            Seconds: 4
   > contract address:    0x62bD7907264033DE6266f03CcEE36c9E214147fC
   > block number:        9184793
   > block timestamp:     1606949603
   > account:             0x878c2B8b7F06fB0aF999A3FC96CBeC7Aa0580fb0
   > balance:             1.580818333
   > gas used:            306084
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00612168 ETH


   Replacing 'ConsumerRole'
   ------------------------
   > transaction hash:    0x0a055b6a373d80c51df58145f1591d52bbae3091022b21d69c570ebbf65003cb
   > Blocks: 1            Seconds: 8
   > contract address:    0x2f241BE597D4fD355cb4FDb1F6FA684FCdbec042
   > block number:        9184796
   > block timestamp:     1606949619
   > account:             0x878c2B8b7F06fB0aF999A3FC96CBeC7Aa0580fb0
   > balance:             1.574696653
   > gas used:            306084
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00612168 ETH


   Replacing 'SupplyChain'
   -----------------------
   > transaction hash:    0xdfb58747a5ee950858d751c3483bb771eda941cd21bfc2544428110da1bad3e9
   > Blocks: 0            Seconds: 16
   > contract address:    0xeb1B432D793A0b55E7E0089d2fc2937334523631
   > block number:        9184797
   > block timestamp:     1606949626
   > account:             0x878c2B8b7F06fB0aF999A3FC96CBeC7Aa0580fb0
   > balance:             1.532156673
   > gas used:            2126999
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.04253998 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.06702646 ETH


Summary
=======
> Total deployments:   6
> Final cost:          0.07153096 ETH
```

## Tracking the Coffee Supply Chain through the Web Interface

Example output transaction hashes.
The following shows the last 4 actions of an item with UPC 2, and the first four steps
of an item with UPC3.

All of these transactions can be doublechecked on EtherScan. For example:
https://ropsten.etherscan.io/tx/0xdd663a379f279610d91e58bb5a312e8e264991a3f1bac168c711e282bd2a642f

```
upc 2, sku 1
...
Sold - 0xdd663a379f279610d91e58bb5a312e8e264991a3f1bac168c711e282bd2a642f
Shipped - 0xbe59612b70535ef058a21d0172ee359c658b6a6c356c4313ba339501e842669b
Received - 0xdf3094411c494d5159f6291bf23227066c28d72178e5996dcc0ee3eaed8357e5
Purchased - 0xa2bf8e4e8b16fbdbe843256219e648b0cf5481168293e79a273e504fa86df84e

upc 3, sku 1
Harvested - 0x1671b1514eee8bba97dda22a58ade12bd6f8d26e218fee6b0df19a17dfb9f3a8
Processed - 0x51682c12881a65f988983b66e75f3b619cf44b0f4fcc906fe089a27a454e9a8c
Packed - 0xbeadcccfd3ba100cd85b3c83ab0a7519e93d248813aa1bb5ce3413deb77418ce
ForSale - 0xec5ebc9105d9ec7b9dc60653abe1664114d9041794b91c0805d55aea66cb5558
...
```

Metamask accounts used:

Account 7: *0x57AB752BD2edE81B10Fc8B155e24Ece6B77A9E5F*
<br>
Account 8: *0x2E3D2a2F5373B9b06a7e0d7F7b20eADdD5aD8c3d*
<br>
Account 9: *0xa0c573D7448d5fEaF0ED59286f941D8c04599C4E*
<br>
Account 10: *0x3ef782988Af42b9e1a9346F29D1396A16c5Ec943*


## Built With

* [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
* [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.

## Authors

Dan Avram