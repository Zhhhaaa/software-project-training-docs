# 系统架构

```text
浏览器
  ↓  http://localhost:8081
Nginx
  ├─ /        提供 HTML、CSS、JavaScript、图片
  └─ /api/    转发给 Spring Boot
                  ↓  http://localhost:8080
              Spring Boot + MyBatis
                  ↓  localhost:3307
              MySQL 8.0
```

## 目录约定

```text
sunshine-airlines-web/    前端静态页面和 JavaScript
sunshine-airlines-api/    Spring Boot 后端项目
nginx/                    Nginx 程序和配置
```

前端请求统一使用 `/api/...`，不要在 JavaScript 中写死 `http://localhost:8080`。
