## CLI MINER

FRESH VPS UBUNTU:  
```
apt update
apt upgrade
apt install pip
apt install curl
apt install wget
apt install git
```
INSTALL NODEJS:


```
apt install nodejs

node -v

apt install npm

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash

source ~/.bashrc

nvm install lts/hydrogen


```


CLONE REPO:


```
git clone https://github.com/agrandil/xc.git
cd xc
npm install
```

IF FAILED?????

```
npm cache clean --force
```


#### Run it

Miner supports both META and FOMO coins:

```
node mine.js --meta --chain=mainnet --phrase="secretphrase"
node mine.js --fomo --chain=mainnet --phrase="secretphrase"
```

or you can run it in the boss mode, mining both:

```
node mine.js --fomo --meta --chain=mainnet --phrase="secretphrase"

```

Where secretphrase is 24 words secret phrase for your wallet private key or private key in the format of "suiprivkey1....." ( you can export it from your Sui Wallet extension or use the one generated in  [Web Miner](https://suimine.xyz/) )

Be sure you have some SUI in your wallet for the gas, 1 SUI is enough for submiting many hashes.

#### Merge META or FOMO coins

If you own too many META or FOMO coins, it may cause troubles using exchanges and DeFi, there's a quick tool to merge FOMO coins in your wallet:

```
node merge.js --meta --chain=mainnet --phrase="secretphrase"
node merge.js --fomo --chain=mainnet --phrase="secretphrase"
```

It merges up to 500 coin objects into single one. But you can run it few times, until it merges every META or FOMO you have.


## License

Apache

**LFG**
