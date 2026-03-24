# Development Plan - App Release Hub

## 项目目标

构建一个支持 Android 多应用市场发布的自托管工具，提供统一构建与发布能力。

---

## Phase 1 - 基础架构（Week 1-2）

- 初始化 Monorepo 结构
- 设计核心数据模型
- 基础后端服务搭建
- 文件上传能力

---

## Phase 2 - 构建系统（Week 3）

- BuildProfile 设计与实现
- 支持 Flutter / Android / 自定义命令
- 构建日志与错误处理

---

## Phase 3 - 华为 Adapter（Week 4）

- APK / AAB 上传
- 提交审核
- 状态查询

---

## Phase 4 - 小米 Adapter（Week 5）

- 接口接入
- 签名与参数映射

---

## Phase 5 - 发布系统（Week 6）

- 多平台发布
- 任务调度
- 状态聚合

---

## Phase 6 - 桌面端（Week 7）

- 应用管理 UI
- 构建配置 UI
- 发布任务 UI

---

## Phase 7 - 部署与开源准备（Week 8）

- Docker Compose
- install 脚本
- 文档完善

---

## MVP 范围

必须：
- 华为 + 小米
- 本地构建
- 一键发布

---

## 后续规划

- 支持更多平台
- CI/CD 集成
- 远程构建 Agent
