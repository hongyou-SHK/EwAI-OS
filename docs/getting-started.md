# 快速入门指南

## 🎯 什么是 EwAI-OS？

EwAI-OS (Evolve with AI Operating System) 是一个实验性项目，旨在构建一个与 AI 智能体深度协作的个人操作系统。

### 核心概念

**传统方式**：
- 每次对话都是"陌生人"
- 需要反复解释你的背景
- AI 无法跨项目保持记忆

**EwAI-OS 方式**：
- AI 拥有"持久化大脑"（`.agent/` 配置）
- 一次配置，所有项目共享
- 跨对话、跨设备的一致性体验

## 📋 前置要求

### 必需
- **操作系统**: macOS 或 Linux
- **云同步盘**: WPS、iCloud Drive、Dropbox 等（用于跨设备同步）
- **AI Agent 工具**: 支持 `.agent/` 配置的工具（推荐 Antigravity）
- **Git**: 用于版本管理

### 可选
- **GitHub 账号**: 如果想备份到云端仓库
- **浏览器**: 用于查看可视化看板

## 🚀 安装教程

### 步骤 1: 克隆项目到云同步盘

```bash
# 进入云同步目录（根据你的设置调整）
cd ~/WPSSyncdisk

# 克隆仓库（如果从 GitHub 获取）
git clone https://github.com/your-username/EwAI-OS.git

# 或者直接在云盘创建文件夹
mkdir EwAI-OS
cd EwAI-OS
```

### 步骤 2: 配置个人画像（可选）

编辑 `.agent/hongyou_profile.md`，填入你的个人信息：

```markdown
# 个人画像

## Ikigai（生命意义交集）
- 我擅长的：...
- 我热爱的：...
- 世界需要的：...
- 我能获得报酬的：...

## 家庭背景
- ...

## 技能矩阵
- ...
```

### 步骤 3: 在新项目中初始化

假设你有一个项目在 `~/Desktop/my-project/`，想接入 EwAI-OS：

```bash
# 进入项目目录
cd ~/Desktop/my-project/

# 运行初始化脚本
bash ~/WPSSyncdisk/EwAI-OS/bin/ewai-init.sh
```

**输出示例**：
```
🚀 正在链接 EwAI 大脑...
✅ 初始化成功！
📂 当前项目已接入：/Users/hongyou/WPSSyncdisk/EwAI-OS/.agent
🤖 你的 'EwAI 进化合伙人' 已就绪。
```

### 步骤 4: 验证连接

```bash
# 检查软链接是否创建成功
ls -la .agent

# 输出应显示：
# .agent -> /Users/hongyou/WPSSyncdisk/EwAI-OS/.agent
```

### 步骤 5: 测试 AI 智能体

在你的 AI 工具中打开该项目，与 AI 对话：

```
你：你是谁？
AI：你好！我是你的 "EwAI 进化合伙人"...（会根据 instructions.md 作答）
```

## 🎨 查看进化看板

用浏览器打开：

```
file:///Users/your-username/WPSSyncdisk/EwAI-OS/public/EwAI_Dashboard.html
```

你会看到一个可视化看板，展示你与 AI 的协作历程。

## 📝 日常使用

### 记录协作日志

当发生重要的人机协作事件时，更新日志：

**文件位置**: `data/logs/EwAI_Co_Evolution_Log.md`

**示例条目**：
```markdown
| 2026-01-11 | 询问方案 | AI 自主执行 | 问答→托管 | ✅ 功能上线 |
```

### 阶段性复盘

完成一个重要里程碑后，写一篇复盘：

**文件位置**: `data/reviews/`

**建议格式**：
```markdown
# [主题] 复盘

## 背景
...

## 关键技术
...

## 经验教训
...
```

## 🔧 常见问题

### Q: 软链接是什么？
A: 软链接（Symbolic Link）是文件系统层面的"快捷方式"。它不会复制文件，只是创建一个指针。优点是节省空间、实时同步。

### Q: 为什么要用云同步盘？
A: 云同步盘可以让你在多台设备间共享同一个"AI 大脑"，换电脑也不会丢失配置。

### Q: 我可以修改 .agent 里的内容吗？
A: 可以！修改后立即生效（某些工具可能需要刷新）。但建议在 `EwAI-OS/.agent/` 里直接修改，不要在项目的软链接里改。

### Q: 如何断开某个项目的连接？
A: 删除项目里的 `.agent` 软链接：
```bash
rm .agent
```

### Q: 脚本提示"未找到 EwAI 大脑核心目录"怎么办？
A: 检查脚本中的 `WPS_PATH` 是否与你的实际路径一致，手动修改 `bin/ewai-init.sh` 中的路径。

## 🎓 进阶使用

### 自定义工作流

在 `.agent/workflows/` 下创建自定义工作流，例如 `deploy.md`：

```markdown
---
description: 部署到生产环境
---

1. 运行测试
2. 构建生产包
3. 上传到服务器
```

### 扩展个人画像

在 `hongyou_profile.md` 中增加更多维度：
- 学习风格
- 沟通偏好
- 常用工具链

## 📚 延伸阅读

- [架构设计文档](../data/reviews/EwAI_Infrastructure_Review.md)
- [共生进化日志](../data/logs/EwAI_Co_Evolution_Log.md)

---

**需要帮助？** 欢迎提 Issue 或反馈！
