# AI 编程规则集合

*[English Documentation / 英文文档](README.md)*

专为 Cursor IDE 设计的 AI 编程规则和工作流综合集合，通过专业化的 AI 代理提升开发效率。

## 🚀 项目概述

本仓库包含专业化的 AI 编程规则，旨在改变你在开发环境中与 AI 的交互方式。每个规则专注于特定开发任务，实现更高效的 AI 辅助。

## ⚡ 快速开始

1. **选择安装方法**（见下方安装方法部分）
2. **从分类中选择规则**，匹配你的需求
3. **在 Cursor 中使用** `@规则名称` 来激活特定行为
4. **探索示例**，查看使用方法部分中每个分类的示例

### 🎯 热门组合
- **新项目**: `@spec-workflow` → `@6A-workflow` → `@code-expert`
- **代码审查**: `@linus-coding-style` → `@code-refactorer`
- **文档编写**: `@prd-writer` → `@content-writer`
- **学习提升**: `@chatgpt-study-mode` → `@book-recommendation-expert`

## 📂 规则分类

### 🔄 开发工作流

#### 规格工作流 → [spec-workflow.md](spec-workflow.md)
系统化的规格驱动开发工作流，通过三阶段迭代流程将功能想法转化为需求、设计和实施计划。

#### RIPER-5 工作流 → [英文版](riper-5-workflow-EN.md) | [中文版](riper-5-workflow-CN.md)
5模式AI开发协作框架（研究→创新→规划→执行→反思），旨在防止未授权代码更改的同时保持结构化开发流程。

#### 6A 工作流 → [中文版](6A-workflow-CN.md)
全面的六阶段开发流程（对齐→架构→原子化→审批→自动化→评估），用于复杂项目管理和系统化实施。

### 🔧 代码增强与质量

#### 代码专家 → [code-expert.md](code-expert.md)
强调增量进步、测试驱动开发和实用代码质量标准的先进开发指南，适用于专业软件开发。

#### 代码重构器 → [code-refactorer.md](code-refactorer.md)
通过系统化分析和风险管理改进，在不改变功能的前提下提升现有代码结构、可读性和可维护性。

#### Linus 编程风格 → [中文版](linus-coding-style-CN.md)
体现 Linus Torvalds 的代码质量哲学，专注于"好品味"、简洁性，通过更好的数据结构消除特殊情况。

### 📝 文档与内容

#### PRD 写作器 → [prd-writer.md](prd-writer.md)
创建包含结构化章节、用户故事和验收标准的综合产品需求文档（PRD），遵循行业最佳实践。

#### 内容写作器 → [content-writer.md](content-writer.md)
具有双模式（大纲/写作）的内容营销和文案写作代理，专为创建清晰解释复杂主题的引人入胜内容而优化。

#### 消息卡片设计师 → [中文版](message-card-CN.md)
专业的 UI 设计师，专注于创建玻璃拟态风格的消息卡片，具有先进的视觉设计原则和响应式布局。

### 🎓 学习与教育

#### ChatGPT 学习模式 → [英文版](chatgpt-study-mode-EN.md) | [中文版](chatgpt-study-mode-CN.md)
教育型 AI 助手，通过问题、提示和协作发现来指导学习，而不是提供直接答案。

#### 美国伙伴语言教练 → [American-Buddy-Language-Coach.md](American-Buddy-Language-Coach.md)
友好的美式英语语言教练，专门从事休闲对话、俚语、习语和文化参考，用于沉浸式语言学习。

#### 图书推荐专家 → [Book-Recommendation-Expert.md](Book-Recommendation-Expert.md)
个性化图书推荐系统，提供详细的图书分析、益处和跨各种类型和兴趣的定制建议。

### 🚀 AI 增强

#### GPT 天才提升 → [GPT-GeniusBoost.md](GPT-GeniusBoost.md)
为高智商用户设计的先进 AI 助手，寻求跨所有领域的全面、深入分析和详细探索。

### 🎯 专业工具

#### 项目命名大师 → [Project-Naming-Master.md](Project-Naming-Master.md)
使用多种语言、神话和创意词汇形成技术创建令人难忘、有意义的项目名称的专家。

## 🛠️ 安装方法

### 方法一：单个规则
```bash
# 创建规则目录
mkdir -p .cursor/rules

# 复制特定规则文件
cp spec-workflow.md .cursor/rules/
cp code-expert.md .cursor/rules/
# ... 根据需要复制其他规则
```

### 方法二：完整集合
```bash
# 克隆仓库
git clone https://github.com/yourusername/cursor-spec-workflow-rule.git

# 创建规则目录
mkdir -p .cursor/rules

# 创建所有规则的符号链接
ln -s /path/to/cursor-spec-workflow-rule/*.md .cursor/rules/
```

### 方法三：Git 子模块（推荐）
```bash
# 添加为子模块
git submodule add https://github.com/yourusername/cursor-spec-workflow-rule.git .cursor/ai-rules

# 创建符号链接
ln -s .cursor/ai-rules/*.md .cursor/rules/
```

### 方法四：直接下载
```bash
# 直接下载特定规则
curl -o .cursor/rules/spec-workflow.md https://raw.githubusercontent.com/yourusername/cursor-spec-workflow-rule/main/spec-workflow.md
```

## 🎯 使用方法

在 Cursor 中使用 `@` 符号引用特定规则：

### 开发工作流
```
@spec-workflow 我想为用户认证创建一个规格
@riper-5-workflow 帮助我系统性地规划新功能
@6A-workflow 我需要实现一个具有适当架构的复杂系统
```

### 代码质量与增强
```
@code-expert 审查这段代码并建议改进
@code-refactorer 帮助我清理这个混乱的函数
@linus-coding-style 分析这段代码的"好品味"和简洁性
```

### 文档与内容
```
@prd-writer 为我们的新仪表板功能创建 PRD
@content-writer 帮助我编写技术文档
@message-card-designer 设计一个现代化的 UI 组件
```

### 学习与教育
```
@chatgpt-study-mode 通过引导学习帮助我理解这个概念
@american-buddy-language-coach 练习休闲英语对话
@book-recommendation-expert 推荐学习软件架构的书籍
```

### AI 增强与工具
```
@gpt-geniusboost 提供这个复杂主题的全面分析
@project-naming-master 帮助我为新项目找到一个好名字
```

## 📋 规则对比

| 规则 | 分类 | 最适用于 | 持续时间 | 语言 |
|------|------|----------|----------|------|
| **规格工作流** | 开发 | 功能规划 | 多会话 | 英文 |
| **RIPER-5** | 开发 | 受控开发 | 按任务 | 中/英文 |
| **6A 工作流** | 开发 | 复杂项目管理 | 多会话 | 中文 |
| **代码专家** | 代码质量 | 专业开发 | 按任务 | 英文 |
| **代码重构器** | 代码质量 | 代码改进 | 单会话 | 英文 |
| **Linus 编程风格** | 代码质量 | 代码质量分析 | 单会话 | 中文 |
| **PRD 写作器** | 文档 | 产品文档 | 单会话 | 英文 |
| **内容写作器** | 文档 | 技术写作 | 1-2会话 | 英文 |
| **消息卡片设计师** | 文档 | UI 设计 | 单会话 | 中文 |
| **ChatGPT 学习模式** | 学习 | 教育指导 | 按会话 | 中/英文 |
| **美国伙伴** | 学习 | 语言学习 | 持续 | 英文 |
| **图书推荐** | 学习 | 阅读建议 | 单会话 | 英文 |
| **GPT 天才提升** | AI 增强 | 深度分析 | 按查询 | 英文 |
| **项目命名大师** | 工具 | 项目命名 | 单会话 | 英文 |

## 🤝 贡献

1. Fork 仓库
2. 创建功能分支
3. 遵循既定的规则格式，包含 YAML frontmatter
4. 提交 pull request

## 📄 许可证

该项目是开源的，遵循 [MIT 许可证](LICENSE)。 