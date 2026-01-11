# EwAI-OS

> **Evolution with AI Operating System**  
> 一个与 AI 共同进化的个人智能体系统

## 💡 项目愿景

EwAI-OS 是一个正在演进中的实验性项目，目标是构建一套帮助个人与 AI 智能体共同进化的操作系统。

这不仅仅是一个工具集，而是一种**新的协作范式**：
- 从"问答式对话"到"目标导向执行"
- 从"临时性聊天"到"持久化记忆"
- 从"单一项目"到"跨项目生态"

## ✨ 核心特性

- 🧠 **持久化 AI 记忆** - 通过 `.agent/` 配置实现跨项目、跨对话的智能体个性化
- 📊 **可视化进化看板** - 实时追踪人机协作模式的演变过程
- 🔗 **一键初始化** - 利用软链接技术在任意项目中快速接入 AI 大脑
- 📝 **共生日志系统** - 记录从 Chatbot 到 Agent 的范式跃迁时刻

## 🚀 快速开始

### 前置要求

- macOS / Linux
- Git
- 支持 `.agent` 的 AI 智能体工具（如 Antigravity）

### 安装步骤

#### 1. 克隆仓库到你的云同步盘

```bash
# 克隆到 WPS 云盘（或其他同步目录）
cd ~/WPSSyncdisk
git clone https://github.com/your-username/EwAI-OS.git
```

#### 2. 在新项目中初始化

```bash
# 进入你的项目目录
cd /path/to/your-project

# 运行初始化脚本
bash ~/WPSSyncdisk/EwAI-OS/bin/ewai-init.sh
```

脚本会自动：
- 检测 EwAI-OS 核心目录位置
- 创建软链接：`.agent/` → `EwAI-OS/.agent/`
- 验证链接是否成功

#### 3. 验证 AI 智能体是否识别

在项目中与 AI 对话，观察它是否表现出个性化行为（根据 `.agent/instructions.md` 定义）。

#### 4. 查看进化看板

用浏览器打开：
```
file:///Users/your-username/WPSSyncdisk/EwAI-OS/public/EwAI_Dashboard.html
```

## 📂 目录结构

```
EwAI-OS/
├── .agent/          # AI 智能体核心配置（大脑）
│   ├── instructions.md       # 行为指令与沟通风格
│   ├── hongyou_profile.md    # 个人画像数据
│   └── workflows/            # 自动化工作流
│
├── bin/             # 可执行工具脚本
│   └── ewai-init.sh          # 项目初始化脚本
│
├── data/            # 运行时数据
│   ├── logs/                 # 时序日志（持续追加）
│   └── reviews/              # 阶段性复盘文档
│
├── public/          # 可视化资源
│   └── EwAI_Dashboard.html   # 进化看板
│
├── docs/            # 使用文档与教程
│   └── getting-started.md    # 新手入门指南
│
└── workspace/       # IDE 工作区配置
```

## 📖 文档

- [快速入门指南](docs/getting-started.md) - 详细的安装与使用教程
- [架构设计](data/reviews/EwAI_Infrastructure_Review.md) - 技术架构与设计哲学

## 🧪 当前状态

**版本**: 0.1.0-alpha  
**阶段**: 实验性构建中

这是一个正在演进的项目，目录结构和功能会根据实际使用情况持续迭代。

## 🤝 贡献

欢迎提出建议和反馈！这个项目目前处于早期探索阶段。

## 📄 协议

MIT License

## 🙏 致谢

- **Antigravity** - 提供了出色的 AI Agent 基础设施
- 所有探索人机共生可能性的先行者们

---

**Made with ❤️ by Hongyou**  
*"让我们一起在百岁人生的黄金赛道上，用 AI 跑出加速度。"*
