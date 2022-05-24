curl http://localhost:8575 \
  -X POST \
  -H "Content-Type: application/json" \
  --data '{"method":"eth_callWithTraceInfo","params":[{"from":"0x207CF3c2db602e1f04c924bC7F6057ecD40d57a1","to":"0x0459c84c277cf9518b780b1f0395f282a2e9c771","data":"0xda3e33970000000000000000000000006ce8da28e2f864420840cf74474eff5fd80e65b80000000000000000000000009ac64cc6e4415144c455bd8e4837fea55603e5c3ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff","gas":"0xc350","gasPrice":"0x2540be400"}, "latest"],"id":2,"jsonrpc":"2.0"}'