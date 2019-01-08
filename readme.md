## RvnDB on RVN testnet
### Install
* git clone https://github.com/raven-community/rvndb-testnet.git
* cd rvndb-testnet
* npm install
* npm install -g pm2
* pm2 install pm2-logrotate

### Configure
* Set your ravencoin RPC host, RPC username, and RPC password in process.json
* Set the script location and cwd in process.json
* Set the block height to start syncing from in rvndb.json
* Set ports in config.js if using testnet ports, or configure RVN node to use mainnet ports instead

### Run
* pm2 start process.json

### Debug / Monitor
* pm2 logs rvnd

Forked from: https://github.com/21centurymotorcompany/bitd