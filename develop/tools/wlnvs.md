# VSCode云开发

### 首次使用
访问专用域名，如：`https://vsdemo.wlniao.net`，默认密码为：`WLNIAO`，首次登录后请通过修改`/root/passwd`文件的内容来设置下次登录的密码，修改后使用`code-server-reset`命令应用生效。

### 存储目录
开发环境重置、升级后仅`/mnt`、`/root`两个目录下的数据会保留，资料务必存储在此目录中，云开发环境会不定期更新或重置。
- `/mnt`：公共磁盘目录，团队共享磁盘
- `/root`：个人主目录
- `/root/workspace`：默认工作空间



### 开发套件
- `nvm`：npm版本管理工具
- `nodejs`：默认版本14.7.1
- `dotnet`：当前为6.0版本
- `podman`
- `vue/cli`
- `openjdk`

### 内部命令
配置应用：`code-server-reset`，应用新的配置内容并重启服务器，如修改密码等。
重启服务：`sv restart name`，重启服务，目前仅支持`ngrok`服务
静态监听：`dotnet serve` 在当前目录开启一个Web监听服务