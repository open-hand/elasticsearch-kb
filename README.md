# choerodon elasticsearch kb

这是应用于知识服务的全文检索的elasticsearch，内部集成中文分词插件ik和修改了部分es属性

elasticsearch.yml

```xml
cluster.name: "docker-cluster" //集群名称
network.host: 0.0.0.0 //绑定host，0.0.0.0代表当前节点的ip
http.cors.enabled: true //支持跨域
http.cors.allow-origin: "*" //跨域匹配所有路由
```

## ARM 支持

```
cd docker/
docker buildx build --platform linux/arm64,linux/amd64 -t registry.cn-shanghai.aliyuncs.com/c7n/elasticsearch-kb:7.9.2-elasticsearch-kb  . --push
```