# 🧠 knowledge-capture

> Turn every AI conversation into a reusable knowledge asset.

A Claude Skill for content creators — whenever you finish a valuable AI conversation (discussion, code collaboration, workflow design, or brainstorming), it automatically distills the conversation into a structured Markdown document ready to drop into your knowledge base.

---

## ✨ What it does

- **Auto-detects conversation type** — discussion, methodology, code project, workflow design, and more — then matches the right document structure
- **Distills, doesn't transcribe** — extracts core insights, decisions, and reusable patterns instead of copying the chat log
- **Keeps key quotes** — preserves a few representative original sentences as evidence, in blockquote format
- **Builds knowledge networks** — automatically tags related knowledge nodes and suggests further thinking, so every document connects to a bigger picture
- **Surfaces content material** — pulls out usable topic ideas, quotes, and case studies to feed your content pipeline
- **Filters noise** — skips batch-generated outputs, dead-end attempts, repetitive back-and-forth, and invalidated ideas
- **Language-aware** — detects the conversation language and outputs the document in the same language

**Output format**: Standard Markdown `.md` file, named `YYYY-MM-DD_title.md`, ready to import into Obsidian, Notion, or any knowledge base tool.

---

## 💡 Best practice: one project, one conversation

For the cleanest results, keep each conversation focused on a single project or topic. Mixing unrelated threads in one chat increases noise and makes distillation less accurate.

---

## 🚀 Installation

### Claude.ai (Web / Desktop)

1. Go to **Settings → Capabilities**, enable **Code execution and file creation**
2. Go to **Customize → Skills**, upload the `.skill` file
3. Done — say "capture this conversation" in any chat to trigger it

### Claude Code (CLI)

```bash
# Install globally
git clone https://github.com/carlxien-blip/knowledge-capture ~/.claude/skills/knowledge-capture

# Or install for a specific project only
git clone https://github.com/carlxien-blip/knowledge-capture .claude/skills/knowledge-capture
```

### Other AI tools (Manus, etc.)

The `.skill` file is just a zip — unzip it and copy the contents of `SKILL.md` into any tool that supports custom system prompts.

---

## 💬 How to use

After finishing a conversation, just say:

> "Capture this conversation"  
> "Save this to my knowledge base"  
> "Distill this chat into a document"

The Skill will ask one question — full conversation or a specific range — then handle everything else automatically.

---

## 📄 Document structure

### Discussion / Methodology

```
# Title
> One-line summary
## Core Insights
## Deep Dive (with key quotes)
## Related Knowledge Nodes
## Further Thinking
## Content Material (topics / quotes / cases)
```

### Project / Code / Workflow

```
# Title
> One-line summary
## Project Overview
## Implementation Process
## Core Code / Config
## Lessons Learned
## Reusable Patterns
## Related Knowledge Nodes
## Further Thinking
```

---

## 🔗 Resources

- [Anthropic Official Skills Repository](https://github.com/anthropics/skills)
- [How to use Skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude)
- [Agent Skills Open Standard](https://agentskills.io)

---

## 📝 License

MIT
