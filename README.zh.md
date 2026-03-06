# Agent Skills

个人 [Claude Code](https://claude.ai/code) 自定义 skill 合集。

> [English README](README.md)

## 安装

```bash
npx skills add zjjfly/agent-skills
```

## Skills 列表

### draft-merger

将同一文档的多份草稿合并为一份完整、精炼的最终版本。

**触发条件：** "merge these drafts"、"combine these versions"、"I have multiple drafts"、"把这几份稿子合并"、"合并稿子"，或者用户提供了多个明显是同一内容不同版本的文件时。

**处理流程：**
1. 读取并评估所有草稿，总结每份草稿的亮点
2. 选择最强的草稿作为基础版本（或使用用户指定的版本）
3. 从其他草稿中提取有价值的内容补充进来——独特的例子、更有力的论据、缺失的背景信息
4. 对合并结果进行润色，确保连贯性、一致性和流畅度
5. 输出最终合并文档，并附上 **合并说明** 小节，解释关键编辑决策

**适用范围：** 文章、报告、提案等各类文字内容。不适用于代码或数据文件的合并。
