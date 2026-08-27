# 第 1 次课：项目启动

## 本次目标

理解系统架构，完成 Nginx 静态页面访问，创建 Spring Boot 项目并设计登录接口。

## 完成标准

- 浏览器能打开 `http://localhost:8081/Login.html`。
- Spring Boot 项目能启动。
- 通过 Nginx 能访问 `http://localhost:8081/api/health`。
- 写出 `POST /api/auth/login` 的请求和响应字段。

## 接口契约

```json
{
  "email": "user@example.com",
  "password": "123456"
}
```

成功时返回用户基本信息和角色，不返回密码。
