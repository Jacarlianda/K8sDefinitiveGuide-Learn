```
master 高可用建议部署3台，负责集群管理和控制，不可宕机，否则无法管理应用
kube-apiserver 集群控制入口，对资源的增删改查操作的唯一入口
kube-cntroller-manager k8s里面所有资源对象的自动化控制中心
kube-scheduler 负责资源调度
etcd 保存资源对象数据
```

```
node 执行master分配的任务，宕机时，会被master转移到其他node上
kubelet 创建、启停pod对应的容器，与master密切协作
kube-proxy 负责service通信跟负载均衡
docker 创建、管理容器
```





