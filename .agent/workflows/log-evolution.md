---
description: 记录 EwAI 共生进化日志与更新看板
---

# 记录 EwAI 共生进化日志 (Workflow)

当宏佑要求“记录进化日志”或发生值得记录的“自主行动/模式变迁”时，执行此工作流。

## 1. 核心文件路径 (SSOT)
- **数据源**: `/Users/mac/WPSSyncdisk/EwAI-OS/data/logs/EwAI_Co_Evolution_Log.md`
- **看板视图**: `/Users/mac/WPSSyncdisk/EwAI-OS/public/EwAI_Dashboard.html`

## 2. 执行步骤

### 第一步：分析本次事件
- **用户触发**: 记录用户的原始问题或需求意图。
- **智能体行动**: 概括 Agent 采取的自主操作和工具调用。
- **模式变迁**: 识别协作模式的深度变化（如：询问->托管，工具->生态）。

### 第二步：同步更新 Markdown 日志
- 在 `EwAI_Co_Evolution_Log.md` 的表格底部追加新行。
- 确保格式正确，包含日期、触发、行动、模式和成果。

### 第三步：更新 HTML 进化看板
- 在 `EwAI_Dashboard.html` 的 `.status-grid` 容器中追加对应的 `.status-card`。
- 递增 `animation-delay`（如每张卡片增加 0.1s）。
- 确保 CSS 样式和布局的一致性。

### 第四步：反馈
- 告知用户已完成双端更新，并建议其刷新看板查看。
