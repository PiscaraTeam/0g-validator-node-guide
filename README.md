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
```
