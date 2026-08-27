# 第 4 次课：登录状态

## 本次目标

完成当前用户获取、退出登录、业务接口保护和 7 天自动登录。

## 核心接口

```text
POST /api/auth/login
GET  /api/auth/me
POST /api/auth/logout
```

登录成功后由后端将用户必要信息保存到 Session。浏览器通过 Cookie 携带 `JSESSIONID`，后端据此识别当前用户。

!!! warning "安全边界"

    不能把浏览器 localStorage 中的 `roleId` 当作后端身份依据。权限判断必须由 Session 和后端拦截器完成。
