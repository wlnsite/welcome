# Wedog容器自动化工具
### 配置说明
配置文件`*.conf`统一放在`/wedog`目录，并挂载容器内的/wedog目录




### 开启Wedog监听服务
```
docker run -d -p6338:6338 --restart=always  \
  -v /wedog:/wedog \
  -v /usr/bin/docker:/usr/bin/docker \
  -v /var/run/docker.sock:/var/run/docker.sock \
  --name wedog wlniao/wedog
```

### 一次性更新容器
```
docker run --rm -it \
  -v /wedog:/wedog \
  -v /usr/bin/docker:/usr/bin/docker \
  -v /var/run/docker.sock:/var/run/docker.sock \
  wlniao/wedog wedog test
```
`test`为要更新的容器名称