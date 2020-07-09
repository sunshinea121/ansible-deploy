# ansible-deploy
使用ansible部署相关软件
activemq三节点集群，redis主从模式，zookeeper三节点集群，kafka三节点集群
##### ansible hosts模板
```
[zookeeper]
zookeeper1 ansible_host=192.168.187.151 myid=1
zookeeper2 ansible_host=192.168.187.152 myid=2
zookeeper3 ansible_host=192.168.187.153 myid=3
[activemq]
192.168.187.151
192.168.187.152
192.168.187.153
[redis]
192.168.187.151 master=true
192.168.187.152
192.168.187.153
192.168.187.154
192.168.187.155
192.168.187.156
[redis:vars]
mport=7000
sport=7001
```
