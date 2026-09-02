# 学习助手

一个面向 Codex 的中文个性化学习辅导 Skill。它适合概念学习、考试复习、作业理解、数学推导和代码学习，强调循序渐进、主动思考与真正理解。

> 仓库名称为“学习助手”，Skill 的内部名称和调用名为 `learning-assistant`。

## 主要功能

- 根据学习目标、已有基础和薄弱点制定学习路径
- 将复杂主题拆成可消化的小知识单元
- 通过提问、线索、练习和反馈引导用户独立解决问题
- 支持概念解释、数学推导、代码学习、作业理解和复习规划
- 可切换中性、正式、快速强攻、学术研讨或苏格拉底式辅导风格
- 对用户提供的教材、笔记、题目和代码先阅读再讲解，避免猜测内容

## 教学流程

学习助手会根据任务选择合适的流程：

1. **系统学习或复习**：了解目标与基础，规划学习蓝图，再逐步讲解和练习。
2. **具体问题辅导**：快速定位卡点，提供必要线索和分步解释，不用完整课程流程拖慢简单问题。
3. **巩固与评估**：通过复述、小测或变式练习检查理解，并根据表现调整难度。

## 安装

将本仓库下载或克隆到 Codex 的个人 Skills 目录，并保持文件夹名为 `learning-assistant`：

```text
~/.codex/skills/learning-assistant/
```

安装后重新启动 Codex，使新 Skill 生效。

## 使用示例

可以在对话中直接提出学习需求，或显式调用 Skill：

```text
使用 $learning-assistant 帮我从零学习游戏关卡设计，并制定四周学习计划。
```

```text
使用 $learning-assistant 引导我理解这道数学题，不要直接给最终答案。
```

```text
使用 $learning-assistant 用苏格拉底式提问帮我找出这段代码的问题。
```

## 目录结构

```text
learning-assistant/
├── SKILL.md
├── README.md
├── agents/
│   └── openai.yaml
└── references/
    ├── persona-style.md
    ├── study-records-and-tools.md
    └── teaching-workflows.md
```

- `SKILL.md`：Skill 的核心触发条件、原则与执行流程
- `agents/openai.yaml`：在 Codex 中显示的名称、简介和默认提示
- `references/persona-style.md`：辅导语气、互动方式和表达规范
- `study-records-and-tools.md`：学习记录与工具的工作流
- `references/teaching-workflows.md`：系统学习与具体问题的详细工作流

## 使用边界

- 以帮助用户掌握知识为目标，不用于代考或冒充用户完成评估
- 不虚构教材内容、学习进度、文件状态或用户经历
- 涉及可能变化或高准确性要求的信息时，应先核实可靠来源
- 默认使用温柔、耐心的中文学习伙伴风格，用户可随时要求改变语气

