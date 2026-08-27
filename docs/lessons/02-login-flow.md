# 第 2 次课：登录闭环

## 本次目标

完成“登录页面 - Nginx - Spring Boot - MySQL - 页面跳转”的完整链路。

## 后端要点

```text
AuthController → AuthService → UserMapper → UserMapper.xml → users 表
```

- 请求对象：`LoginRequest`
- 统一返回对象：`Result<T>`
- 查询方法：按邮箱查询用户
- 登录成功：返回不含密码的用户信息和 `roleId`

## 前端要点

- 从 `.email` 和 `.password` 读取输入。
- Ajax 以 JSON 发送 `POST /api/auth/login`。
- `code === 0` 时按 `roleId` 跳转页面。
- 失败信息显示在 `.alertInfo`。

## 验证

使用 HTTP Client 分别测试正确账号、错误密码和空参数；再从 `Login.html` 完成真实登录。
