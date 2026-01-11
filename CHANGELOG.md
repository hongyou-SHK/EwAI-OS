# 更新日志

本文档记录 EwAI-OS 项目的所有重要变更。

格式遵循 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.0.0/)，
版本号遵循 [语义化版本](https://semver.org/lang/zh-CN/)。

## [未发布]

### 计划中
- GitHub Actions 自动化部署
- 多用户配置模板
- 进化看板数据自动更新

## [0.1.0] - 2026-01-11

### 新增
- 🎯 **项目初始化**：建立 EwAI-OS 核心目录结构
- 📂 **标准化架构**：采用 v3.5 产品级目录设计（bin/、data/、public/、docs/、workspace/）
- 📝 **共生日志系统**：创建 `data/logs/EwAI_Co_Evolution_Log.md` 记录人机协作演进
- 📊 **可视化看板**：`public/EwAI_Dashboard.html` 动态展示进化历程
- 🛠️ **初始化脚本**：`bin/ewai-init.sh` 实现一键项目接入
- 📖 **完整文档**：
  - `README.md` - 项目说明与快速开始
  - `docs/getting-started.md` - 详细入门指南
  - `.gitignore` - 版本控制规范
- 🧠 **AI 大脑配置**：`.agent/` 目录包含指令集、个人画像和工作流

### 改进
- ♻️ **项目重命名**：`My-AI-Life` → `EwAI-OS`（强化操作系统定位）
- 📁 **目录重构**：从平铺结构升级为分层架构
- 🔗 **路径更新**：所有内部引用更新至新目录结构

### 复盘文档
- `data/reviews/EwAI_Infrastructure_Review.md` - 基础设施技术复盘
- `data/reviews/Story_of_a_Co_Evolution.md` - 共生进化叙事（普通版）
- `data/reviews/Story_of_a_Co_Evolution_Tech.md` - 共生进化叙事（技术版）

## [0.0.1] - 2026-01-02

### 新增
- 🌱 **概念验证**：在 `My-AI-Life` 文件夹建立最初原型
- 🔧 **软链接实验**：验证 `.agent/` 跨项目共享可行性
- 📝 **个人画像**：创建 `hongyou_profile.md`

---

## 版本说明

- **[未发布]** - 正在开发中的功能
- **[0.1.0]** - 当前稳定版本（实验性构建）
- **[0.0.1]** - 概念验证阶段

## 贡献者

- **宏佑 (Hongyou)** - 项目发起人与主要维护者
- **Antigravity Agent** - 技术实现与架构设计

---

*最后更新: 2026-01-11*
