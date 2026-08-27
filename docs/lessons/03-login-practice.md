# 第 3 次课：登录练习

## 任务

在干净项目骨架中独立实现登录模块，不直接复制课堂完整代码。

## 必做验收

- `POST /api/auth/login` 接收 JSON 格式邮箱和密码。
- 使用 MyBatis Mapper + XML 查询 `users` 表。
- Controller、Service、Mapper 分层明确。
- 成功响应不包含密码。
- 页面能够提示失败信息并按角色跳转。

## 提交

提交后端源码、前端 `login.js` 和 HTTP Client 测试文件。
