# 使用说明

## 适用任务

新课程上线前，同时审查小红书笔记、朋友圈长图、短视频口播和直播间话术。

## 准备输入

机构地区与业务类型、渠道、原文案/脚本、课程与价格、优惠规则、案例授权状态、预期受众。使用前先脱敏姓名、联系方式和与任务无关的敏感信息。

## 操作步骤

1. 确认适用地区与业务类型
2. 提取宣传承诺
3. 检查敏感词与事实依据
4. 检查案例肖像授权
5. 标记风险等级
6. 给出守边界改写
7. 人工复核清单

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

合规负责人/法律专业人员复核所有高风险宣传承诺、真实案例、未成年人代言和优惠稀缺性表述后，成果才可进入正式业务使用。
