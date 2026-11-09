# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `assignments` | 跨学科作业清单 | array | 是 |
| `grade` | 年级 | string | 是 |
| `student_group` | 学生群体 | string | 是 |
| `learning_objectives` | 目标 | array | 是 |
| `parent_feedback` | 家长反馈摘要 | string | 否 |
| `schedule_context` | 周内时间安排 | string | 是 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `周作业负荷表`：结构化条目数组，不允许空壳或占位文本。
- `跨学科冲突`：结构化条目数组，不允许空壳或占位文本。
- `低效任务清单`：结构化条目数组，不允许空壳或占位文本。
- `替代任务建议`：结构化条目数组，不允许空壳或占位文本。
- `分层规则`：结构化条目数组，不允许空壳或占位文本。
- `家长沟通模板`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
