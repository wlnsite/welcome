# VSCode云开发

### 首次使用
访问专用域名，如：`https://vsdemo.wlniao.net`，默认密码为：`WLNIAO`，首次登录后请通过修改`/root/passwd`文件的内容来设置下次登录的密码，修改后使用`code-server-reset`命令应用生效。

### 开发套件
- `nvm`：npm版本管理工具
- `nodejs`：默认版本14.7.1
- `dotnet`：当前为6.0版本
- `vue/cli`
- `openjdk`

### 内部命令
配置应用：`code-server-reset`，应用新的配置内容并重启服务器，如修改密码等。
重启服务：`sv restart name`，重启服务，目前仅支持`ngrok`服务
静态监听：`dotnet serve` 在当前目录开启一个Web监听服务