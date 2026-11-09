# 输入输出契约

## 输入字段

| 键 | 名称 | 类型 | 必填 |
|---|---|---|---|
| `region` | 机构地区 | string | 是 |
| `business_type` | 业务类型 | string | 是 |
| `channel` | 发布渠道 | string | 是 |
| `content_text` | 原始宣传内容 | string | 是 |
| `course_and_price` | 课程与价格信息 | string | 是 |
| `promotion_rules` | 优惠与名额规则 | string | 否 |
| `case_authorization_status` | 案例与肖像授权状态 | string | 否 |
| `target_audience` | 目标受众 | string | 是 |

## 状态

- `completed`：核心成果完整，关键结论人工确认要求满足。
- `completed_with_limits`：至少一项实质成果，说明限制、已完成和受阻范围。
- `needs_input`：必填字段缺失。
- `needs_confirmation`：资料冲突或人工确认未完成。
- `failed`：计算或工具失败。

## 输出

- `合规风险表`：结构化条目数组，不允许空壳或占位文本。
- `问题原文与原因`：结构化条目数组，不允许空壳或占位文本。
- `可保留表达`：结构化条目数组，不允许空壳或占位文本。
- `建议改写版`：结构化条目数组，不允许空壳或占位文本。
- `缺失证据清单`：结构化条目数组，不允许空壳或占位文本。
- `发布前审批单`：结构化条目数组，不允许空壳或占位文本。

完整机器契约见`contract/input.schema.json`、`contract/output.schema.json`和`contract/runtime_contract.json`。
