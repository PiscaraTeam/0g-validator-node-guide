# 0g-validator-node-guide
Here is our team’s guide, with which you can easily launch the 0g_labs project node

**Before moving on to the guide itself, we kindly ask you to familiarize yourself with the network parameters:**
|Parametr|Value|
|:-------|:----|
|Chain Name|0G-Newton-Testnet|
|Chain ID|`zgtendermint_16600-2`|
|Token Name|A0GI|
|RPC|https://rpc-testnet.0g.ai|
|Websocket|wss://rpc-testnet.0g.ai/ws|
|Storage-RPC|https://rpc-storage-testnet.0g.ai|

**You also need to meet these requirements:**

|Requirement|Value|
|:----------|:----|
|Memory|64 GB|
|CPU|8 cores|
|Disk|1 TB NVME SSD|
|Bandwidth|100 MBps|


# Install
```
git clone -b v0.2.3 https://github.com/0glabs/0g-chain.git
./0g-chain/networks/testnet/install.sh
source ~/.profile

0gchaind config chain-id zgtendermint_16600-2
```

## Genesis and Seeds
```
sudo apt install -y unzip wget
rm ~/.0gchain/config/genesis.json
wget -P ~/.0gchain/config https://github.com/0glabs/0g-chain/releases/download/v0.2.3/genesis.json
```
**Add Seeds to `app.toml`**
```
81987895a11f6689ada254c6b57932ab7ed909b6@54.241.167.190:26656,010fb4de28667725a4fef26cdc7f9452cc34b16d@54.176.175.48:26656,e9b4bc203197b62cc7e6a80a64742e752f4210d5@54.193.250.204:26656,68b9145889e7576b652ca68d985826abd46ad660@18.166.164.232:26656
```

# Start 0g
```
0gchaind start
```
