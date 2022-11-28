### Requirements
- Install https://github.com/tsenart/vegeta  

### Benchmark
```sh
KEY=[enter api key here] && echo POST https://bsc-mainnet.nodereal.io/v1/"$KEY" | vegeta attack -body ./body.json -duration=5s -rate=100 | tee results.bin | vegeta report
```