# Quantis development tree

----

# About the repo

**This is a personal fork of the [official Quantis repository](https://github.com/QuantisNetwork/Quantis-public). It aims to fix a few things for my own use: use it at your own risks.**

Current changes from :
 - Fix chmod of executable scripts.
 - Allow comments in `masternodes.conf`
 - Fix a graphic bug on Dashboard in Darksend panel.

----

TO build use

Build with:  make -j4 -f makefile.unix RELEASE=1

Quantis is a hybrid PoW/PoS-based cryptocurrency with masternodes.

## PoW
* Algorithm: Scrypt
* PoW Supply: unlimited
* PoW Spacing: 30 Seconds
* PoW Interval: 5 blocks 
* PoW Reward:
    * &le; block 50: 5 QUAN
    * &le; block 555: 1055 QUAN
    * &le; block 1555: 55 QUAN
    * forever:  5 QUAN

## PoS
* PoS Reward:
    * 3 QUAN to masternodes
    * 2 QUAN to staking
* PoS Minimum Age: 24 hours
* PoS Maximum Age: none

## Masternodes
* Masternode Collateral: 5000 QUAN
* Masternode Enable:  block #1000, approximately

## Ports
* P2P Port: 5050
* RPC Port: 5051
