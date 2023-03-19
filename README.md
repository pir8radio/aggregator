<img align="right" src="https://i.imgur.com/6Jjtpy3.png" height="300">

# Aggregator - Signum Miner Proxy

The Signum Aggregator allows you to have many small miners on your local network and save bandwidth and resources by making them appear as one big miner to the mining pool!    Another handy use is to send one or many miners to multiple pools or totally different PoS+ blockchains or even a TESTNET pool while you mine on the main net!

### Configuration and Use
Just open the aggregator config.yaml file.  
1.) If you have many miners mining to a single pool: delete the "secondary" section of the config, and update the "primarySubmitURL" to your Signum main net pool url.   Save and run the aggregator. Set your miners config "url" setting to http://ip-of-aggregator-pc:7777  example: 'http://127.0.0.1:7777'

2.) If you want to mine on multiple chains or Main-net as well as TESTNET at the same time: Update the "primarySubmitURL" to your Signum main net pool url, update the "secondarySubmitURL" to the test net pool url or other chains pool url. Save and run the aggregator. Set your miners config "url" setting to http://ip-of-aggregator-pc:7777  example: 'http://127.0.0.1:7777'

### Requirements
- go >= 1.11

### Compile

``` shell
go build
```

## Configure

All settings to be made in config.yaml

### Run

``` shell
./aggregator
```
