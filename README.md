###Introduction:

This repo has docker-compose file to create 3 node zookeeper cluster.
echo node internally referenced with alias names zk_1 zk_2 zk_3


###Pre-req:
1. update your environment proxy in env file



###deploying app in docker swarm:
```
 docker stack deploy -c docker-compose.yml zoo
```

### check app stack status
```
docker statck ls
```

#### verify nodes conectvity
login to each container and verify able to ping other nodes with alias names i.e zk_1,zk_2 etc.
```
docker exec -it < container-id > /bin/bash 
ping zk_1
````


##References:





