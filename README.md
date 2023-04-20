

## bitcoind setup notes

* A random RPC cookie will always be generated, even if `rpcauth` is set (either can be used for RPC auth)

## bitcoin-cli cheatsheet

`bitcoin-cli getnewaddress`

`bitcoin-cli generatetoaddress 50 <addr>`

`bitcoin-cli listreceivedbyaddress 1 true | jq '.[].address'` (to get all receive addresses even ones which have never been used)

`bitcoin-cli gettransaction <txid>`

`bitcoin-cli getblock <blockhash>`

`bitcoin-cli sendtoaddress <addr> <amount>`

  * May require `bitcoin-cli settxfee 0.0001` with some fee amount to work
