# 企业微信代理

[![Build](https://github.com/wuyangdaily/wechat/actions/workflows/build.yml/badge.svg)](https://github.com/wuyangdaily/wechat/actions/workflows/build.yml)
[![docker pulls](https://img.shields.io/docker/pulls/wuyangdaily/wechat.svg?logo=docker&label=Wechat下载次数)](https://hub.docker.com/r/wuyangdaily/wechat)

```bash
docker run -d \
    --name wechat \
    --restart=always \
    -p 7080:80 \
    wuyangdaily/wechat:latest
```

```yaml
version: '3.3'
services:
    wechat:
        container_name: wechat
        restart: always
        ports:
            - '7080:80'
        image: 'wuyangdaily/wechat:latest'
```
