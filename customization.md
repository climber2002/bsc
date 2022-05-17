## Test hello json/rpc endpoint

curl http://localhost:8575 \
  -X POST \
  -H "Content-Type: application/json" \
  --data '{"method":"eth_hello","params":["Andy"],"id":1,"jsonrpc":"2.0"}'

## Test counter

curl http://localhost:8575 \
  -X POST \
  -H "Content-Type: application/json" \
  --data '{"method":"eth_call","params":[{"from":null,"to":"0xA86FB9Ea961B1404262B621335bd8b54FCE50f97","data":"0x5b34b966"}, "latest"],"id":2,"jsonrpc":"2.0"}'