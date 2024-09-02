```bash
cd 7000
redis-server redis.conf
cd 7001
redis-server redis.conf
redis-cli -p 7001
replicaof 127.0.0.1 7000
ctrl-C
cd 26379
redis-server sentinel.conf --sentinel
cd 26380
redis-server sentinel.conf --sentinel
cd 26381
redis-server sentinel.conf --sentinel
redis-cli -p 26379
sentinel get-master-addr-by-name mymaster
```
