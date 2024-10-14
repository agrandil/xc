## CLI MINER

FRESH VPS UBUNTU:  
```

apt update -y && apt upgrade -y && apt install curl -y && apt install iptables -y && apt install build-essential -y && apt install git -y && apt install wget -y && apt install lz4 -y && apt install jq -y && apt install make -y && apt install gcc -y && apt install nano -y && apt install automake -y && apt install autoconf -y && apt install tmux -y && apt install htop -y && apt install nvme-cli -y && apt install pkg-config -y && apt install libssl-dev -y && apt install libleveldb-dev -y && apt install tar -y && apt install clang -y && apt install bsdmainutils -y && apt install ncdu -y && apt install unzip -y && apt install libleveldb-dev  -y

```
INSTALL NODEJS:


```
apt install nodejs -y && apt install npm -y && curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash -y && source ~/.bashrc && nvm install lts/hydrogen


```


CLONE REPO:


```
git clone https://gitlab.com/suidouble/sui_meta.git 
cd sui_meta
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
