# 作业负担与有效性审查示例

## 典型场景

同一晚数学卷40分钟、英语抄写30分钟、语文阅读30分钟，总计超过建议范围。

## 具体示例

系统汇总三科后建议将英语抄写改为10分钟错词复习，并保留需教师确认的学科必做项。

## 脱敏输入示例

```json
{
  "contract_version": "1.2.0",
  "data_status": "confirmed",
  "contains_sensitive_data": false,
  "requested_output_language": "zh-CN",
  "assignments": [
    {}
  ],
  "grade": "年级已核对（脱敏示例）",
  "student_group": "学生群体已核对（脱敏示例）",
  "learning_objectives": [
    {}
  ],
  "parent_feedback": "家长反馈摘要已核对（脱敏示例）",
  "schedule_context": "周内时间安排已核对（脱敏示例）"
}
```

## 预期处理

1. 运行输入契约校验。
2. 逐项核对输入来源、版本和口径。
3. 按`references/PROFESSIONAL_PLAYBOOK.md`完成专业分析。
4. 输出周作业负荷表、跨学科冲突、替代任务建议等核心成果。
5. 由业务负责人确认输入事实、关键假设和最终成果适用范围后才可作为正式业务结论。

## 不应出现的输出

- 虚构政策、价格、人员、课程或客户事实。
- 以“暂无”“待完善”等占位文本冒充完成。
- 无依据的确定性判断或伪造人工签批。
