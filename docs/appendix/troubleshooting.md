# 常见问题

## 页面可打开，接口返回 502

Spring Boot 没有启动，或后端端口不是 `8080`。

## 页面可打开，接口返回 404

检查 JavaScript 请求地址、Controller 映射和请求方式是否一致。

## 修改 JavaScript 后效果未变化

浏览器按 `Ctrl + F5` 强制刷新，避免缓存旧脚本。

## MySQL 连接失败

检查 MySQL80 服务、端口 `3307`、数据库名和 `application.yaml` 配置。
