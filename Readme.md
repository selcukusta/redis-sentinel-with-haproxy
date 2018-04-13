# Build fault-tolerance Redis cluster with Sentinel on Docker
## Topology
![topology](https://raw.githubusercontent.com/selcukusta/redis-sentinel-with-haproxy/master/redis-sentinel-mode-topology.png)
## Run
`docker-compose up -d`
## Tail sentinel logs
`clear && tail -f /var/log/sentinel.log`
## Get redis replication info per seconds
`while true; do redis-cli info replication; sleep 1; clear; done`