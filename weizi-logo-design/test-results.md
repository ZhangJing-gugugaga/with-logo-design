# test-results — weizi-logo-design 压力测试结果

> 阶段 4 (darwin 兼容测试) 产物

## 测试集

10 条 prompt（test-prompts.json），覆盖：
- 应调用（5 条）：奶茶店logo、咖啡标志、民宿正负形、律所标识、logo手法问答
- 不应调用（2 条）：海报、小红书文案
- 兄弟 skill 混淆（1 条）：VI 系统（含 logo 但范围更大）
- 边界（2 条）：动态3D logo、人民币国徽配色

## 预期结果

| 类别 | 数量 | 预期行为 |
|---|---|---|
| should_invoke | 5 | 激活 weizi-logo-design |
| should_not_invoke | 2 | 不激活 |
| sibling_trap | 1 | 激活但聚焦 logo 部分，说明与 doubao-creative-design 边界 |
| boundary | 2 | 激活但说明边界；违规内容拒绝 |

## 自测判定

- ✅ 描述字段含明确中英触发词，可被正确路由
- ✅ 边界（B 段）明确列出不适用场景与作者盲点
- ✅ 与 doubao-creative-design 的区分已写清（构思方法论 vs 视觉生成）
- ✅ 违规场景（人民币国徽）在 B 段显式禁止

## 待办

- 安装后可运行端到端盲测（由主流程或独立 agent 执行）
