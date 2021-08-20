# BSC

### reset blockchain:  
```
geth --datadir projects/local_ethereum_blockchain/node11 init projects/local_ethereum_blockchain/genesis.json
```
<br>

### run blockchain:
``` 
geth --syncmode=fast --datadir projects/local_ethereum_blockchain/node11 --nodiscover  --syncmode full --networkid 18  --rpc --rpcaddr 0.0.0.0 --rpcport 8885 --port 8886    --rpccorsdomain "*"  --rpcapi admin,db,eth,debug,miner,net,shh,txpool,personal,web3 --allow-insecure-unlock  --rpc.allow-unprotected-txs --miner.etherbase 0x96e7a43fda81207b63ebe8dbdbe9c6765f7ec980 --mine --miner.threads=1
```
