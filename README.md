# 🧠 knowledge-capture

> 把每一次与 AI 的对话，变成可复用的知识资产。

一个为内容创作者设计的 Claude Skill——每当你结束一段有价值的 AI 对话（无论是讨论、代码协作、工作流搭建还是灵感碰撞），它都能自动将对话提炼成结构化的 Markdown 知识文档，直接投入你的知识库。

---

## ✨ 它能做什么

- **自动识别对话类型**：普通讨论、方法论、代码项目、工作流设计……自动匹配对应的文档结构
- **提炼而不是复述**：不是粘贴对话记录，而是萃取核心观点、决策逻辑、可复用模式
- **保留关键原句**：少量最有代表性的原始表达作为佐证，以 blockquote 格式呈现
- **构建知识网络**：自动标注关联知识节点和延伸思考，让每篇文档都能接入更大的知识体系
- **挖掘内容素材**：顺手提炼出可用的选题方向、金句、案例，直接服务内容生产

**输出格式**：标准 Markdown `.md` 文件，命名规范 `YYYY-MM-DD_标题.md`，可直接导入 Obsidian、Notion、飞书等任何知识库工具。

---

## 💡 使用建议：养成「单项目单对话」的习惯

为了让 Skill 提炼出更准确、更干净的知识文档，建议：

**一个项目 / 一个任务 → 开一个独立的对话窗口**

把不同主题的讨论混在同一个对话里，会增加噪音识别的难度，提炼结果也会更模糊。独立的对话窗口 = 更清晰的知识边界 = 更高质量的文档。

---



### Claude.ai（网页/App）

1. `Settings → Capabilities`，开启 **Code execution and file creation**
2. `Customize → Skills`，上传 `.skill` 文件
3. 完成，开始聊天

### Claude Code（命令行）

```bash
# 个人全局安装
git clone https://github.com/你的用户名/knowledge-capture ~/.claude/skills/knowledge-capture

# 或只在当前项目使用
git clone https://github.com/你的用户名/knowledge-capture .claude/skills/knowledge-capture
```

---

## 💬 使用方法

对话结束后，直接说：

> "帮我沉淀这段对话"  
> "整理成知识文档"  
> "做个知识沉淀"  
> "存入知识库"

Skill 会自动开始工作，生成 `.md` 文件供下载。

---

## 📄 文档结构示例

### 观点 / 方法论类对话

```
# 文档标题

> 一句话摘要

## 核心观点
## 详细展开（含关键原句）
## 关联知识节点
## 延伸思考
## 可用素材（选题/金句/案例）
```

### 项目 / 代码 / 工作流类对话

```
# 文档标题

> 一句话摘要

## 项目概述
## 实现过程
## 核心代码/配置
## 踩坑记录
## 可复用的模式
## 关联知识节点
## 延伸思考
```

---

## 🗂️ 适合放入知识库的内容类型

| 对话类型 | 示例 |
|---------|------|
| 💡 灵感 / 观点 | 和 AI 讨论某个行业趋势、产品想法 |
| 📚 方法论 | 探索一套工作流程、学习某个框架 |
| 🛠️ 工作流搭建 | 用 AI 设计自动化流程 |
| 💻 代码 / 技术 | 调试代码、搭建项目架构 |
| 🔍 案例研究 | 分析某个工具、产品、行业案例 |

---

## 🔗 相关资源

- [Anthropic 官方 Skills 仓库](https://github.com/anthropics/skills)
- [如何在 Claude.ai 使用 Skills](https://support.claude.com/en/articles/12512180-use-skills-in-claude)
- [Agent Skills 开放规范](https://agentskills.io)

---

## 📝 License

MIT
