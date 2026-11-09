# 使用说明

## 适用任务

同一晚数学卷40分钟、英语抄写30分钟、语文阅读30分钟，总计超过建议范围。

## 准备输入

各科作业清单、预计用时、知识点目标、题型、提交方式、班级水平、家长反馈和周末安排。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 建立周作业表
2. 汇总时间
3. 检查目标对齐
4. 标记重复/低效
5. 评估反馈闭环
6. 给出减负增效方案

## 校验命令

```powershell
node scripts/validate_input.js examples/typical_input.json
node scripts/validate_output.js examples/typical_output.json
```

## 状态使用

- `completed`：核心成果完整。
- `completed_with_limits`：只完成可验证部分，并说明受阻范围。
- `needs_input`：缺少关键输入。
- `needs_confirmation`：资料冲突或需人工确认。
- `failed`：工具或计算失败，提供恢复动作。

## 人工确认

业务负责人复核输入事实、关键假设和最终成果适用范围后，成果才可进入正式业务使用。
