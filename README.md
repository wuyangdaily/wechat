# 企业微信代理

[![Build](https://github.com/wuyangdaily/wechat/actions/workflows/build.yml/badge.svg)](https://github.com/wuyangdaily/wechat/actions/workflows/build.yml)
[![Docker Pulls](https://img.shields.io/badge/dynamic/json?url=https://hub.docker.com/v2/repositories/wuyangdaily/wechat&query=$.pull_count&label=下载次数&logo=docker)](https://hub.docker.com/r/wuyangdaily/wechat)

```bash
docker run -d \
  --name wechat \
  -p 7080:80 \
  --restart=always \
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
