# App Release Hub

App Release Hub 是一个面向 Android 开发者的多应用市场发布自动化工具，支持自托管部署。它通过统一的构建与发布流程，帮助开发者将 APK / AAB 一键发布到华为、小米、vivo、OPPO 等主流应用市场，同时支持本地构建（Flutter / Android）与自定义构建脚本，实现从构建到发布的全流程自动化。

## 核心特性

- 多应用市场统一发布入口
- 自托管后端，密钥不托管到第三方公共服务
- 支持本地构建、手动上传产物、自定义 Shell 构建
- 支持 Build Profile（构建方案）管理
- 插件化市场适配层（Market Adapters）
- 发布任务追踪、日志查看、失败重试
- 适配 Flutter、Android 原生及自定义项目流程

## 适用场景

适用于已经拥有各大应用市场开发者账号、应用和备案资料的开发者或团队，用于统一管理 Android 应用在多个国内应用市场的构建与发布流程。

## 项目目标

本项目希望解决以下问题：

- 多个平台后台重复上传与提审操作繁琐
- 不同技术栈项目的构建方式不统一
- Flutter、原生 Android、多渠道、多 flavor 项目难以复用统一发版流程
- 发布过程缺乏统一日志、状态追踪与可维护的配置体系

## 设计原则

- 自动检测优先，允许用户手动覆盖
- 提供默认模板，也支持结构化配置与 Shell 模式
- 构建与发布解耦
- 本地构建优先，自托管发布服务负责分发
- 安全优先，敏感配置仅保存在用户自有环境中

## 计划支持的平台

- Huawei AppGallery
- Xiaomi
- vivo
- OPPO

## 计划支持的构建模式

- 手动上传 APK / AAB
- 项目目录自动识别
- 图形化构建配置
- 结构化 JSON 构建配置
- 自定义 Shell 构建脚本

## 仓库规划

```text
app-release-hub/
├─ apps/
│  ├─ desktop/
│  └─ server/
├─ packages/
│  ├─ core/
│  ├─ adapters/
│  ├─ sdk/
│  └─ crypto/
├─ deploy/
├─ docs/
│  └─ development-plan.md
├─ README.md
├─ .gitignore
└─ LICENSE
```

## 开发计划

详见 [docs/development-plan.md](docs/development-plan.md)

## License

Apache-2.0
