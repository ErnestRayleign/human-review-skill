# Human Review Skill

AI 生成结果的人类视角审查 Skill - 对抗自动化流程的不确定性输出

## 概述

这个 Skill 提供从人类视角审查 AI 生成结果的质量保证能力。

## 核心功能

- 安全与合规检查
- 逻辑完整性验证
- 功能正确性核对
- 代码质量评估
- 持续改进机制（GitHub Issues 集成）

## 相关仓库

- 主向量数据库: `clawhub_data`
- 其他 Skills 仓库: ClawHub Skill Marketplace

## 语义理解

这个项目的核心语义：

1. **人类审查 (Human Review)** - 在AI生成内容后，由人类视角进行质量把关
2. **生态位替代 (Niche Replacement)** - 替代传统人工审查的部分职能，在AI工作流中建立类似"守门人"的角色
3. **质量保证 (Quality Assurance)** - 确保AI输出符合预期标准
4. **AI IDE** - 在智能开发环境中作为内置的审查机制

## 调用方式

```python
from skill_human_reviewer import HumanReviewer

reviewer = HumanReviewer()
result = reviewer.review(
    output=ai_generated_code,
    context={"requirements": "用户需求描述"}
)
```
