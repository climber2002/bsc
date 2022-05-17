## Test hello json/rpc endpoint

curl http://localhost:8575 \
  -X POST \
  -H "Content-Type: application/json" \
  --data '{"method":"eth_hello","params":["Andy"],"id":1,"jsonrpc":"2.0"}'

## Test counter

### incrementCount

curl http://localhost:8575 \
  -X POST \
  -H "Content-Type: application/json" \
  --data '{"method":"eth_call","params":[{"from":"0x207CF3c2db602e1f04c924bC7F6057ecD40d57a1","to":"0xA86FB9Ea961B1404262B621335bd8b54FCE50f97","data":"0x5b34b966","gas":"0xc350","gasPrice":"0x2540be400"}, "latest"],"id":2,"jsonrpc":"2.0"}'


curl https://data-seed-prebsc-1-s1.binance.org:8545/ \
  -X POST \
  -H "Content-Type: application/json" \
  --data '{"method":"eth_call","params":[{"from":"0x207CF3c2db602e1f04c924bC7F6057ecD40d57a1","to":"0xA86FB9Ea961B1404262B621335bd8b54FCE50f97","data":"0x5b34b966","gas":"0xc350","gasPrice":"0x2540be400"}, "latest"],"id":2,"jsonrpc":"2.0"}'

### getCount

curl http://localhost:8575 \
  -X POST \
  -H "Content-Type: application/json" \
  --data '{"method":"eth_call","params":[{"from":null,"to":"0xA86FB9Ea961B1404262B621335bd8b54FCE50f97","data":"0xa87d942c","gas":"0x333333"}, "latest"],"id":1,"jsonrpc":"2.0"}'


curl https://data-seed-prebsc-1-s1.binance.org:8545/ \
  -X POST \
  -H "Content-Type: application/json" \
  --data '{"method":"eth_call","params":[{"from":null,"to":"0xA86FB9Ea961B1404262B621335bd8b54FCE50f97","data":"0xa87d942c"}, "latest"],"id":1,"jsonrpc":"2.0"}'