# V2Ray Heroku

## Introduce

Deploying v2ray websocket on Heroku

**Heroku provides us free docker containers, so we shouldn't abuse that:)**

**You can deploy two apps, then Heroku shouldn't think you are abusing their services.**

**Heroku's network is not stable, think before you go.**

## Mirror

This mirror will not let Heroku to think we are abusers.

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https%3A%2F%2Fgithub.com%2Fshuairuan%2Fv2ray-heroku)

## ENV 设定

### UUID

`UUID` > `一个 UUID，供用户连接时验证身份使用`。

## 注意

WebSocket 路径为 `/`。

`alterId` 为 `64`。

V2Ray 将在部署时自动安装最新版本。

**出于安全考量，除非使用 CDN，否则请不要使用自定义域名，而使用 Heroku 分配的二级域名，以实现 V2Ray Websocket + TLS。**
