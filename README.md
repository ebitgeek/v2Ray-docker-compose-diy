# V2Ray Docker-Compose DIY ❤
个性化定制了了一下 V2Ray Docker 一键启动

## server (服务端)
打开 *server.conf.jsonc* 
- 生成一个新的uuid 替换 `id` 项

### 启动服务端
终端输入
```shell
docker-compose up -d 
```

## client (客户端)
打开  *client.conf.jsonc* 
- 替换 `uuid` (必须与服务端相同)
- 修改 `address` 为服务端地址

### 启动客户端
终端输入
```shell
docker-compose up -d -e VMODE=client
```
