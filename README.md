# nexus

## 父镜像地址
```shell script
https://github.com/sonatype/docker-nexus3
```
## 镜像名称
```shell script
registry.cn-beijing.aliyuncs.com/meowbite/nexus:20191001
```

## 使用方法
```shell script
docker pull registry.cn-beijing.aliyuncs.com/meowbite/nexus:20191001

docker run -d -p 8081:8081 --name nexus registry.cn-beijing.aliyuncs.com/meowbite/nexus:20191001
```

## 验证
```shell script
#开启防火墙
iptables -A INPUT -p tcp --dport 8081 -j ACCEPT
#验证
curl 127.0.0.1:8081
```

