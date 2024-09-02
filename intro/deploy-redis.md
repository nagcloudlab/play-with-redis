# install redis in ubuntu

```bash
sudo apt-get install redis-server
```

stop redis server if it is running as a service

```bash
sudo systemctl redis-server stop
```

start redis server with configuration file in foreground

```bash
redis-server /path/to/redis.conf
```

start redis-cli

```bash
redis-cli -h localhost -p 6379
```

or using redisinsight
