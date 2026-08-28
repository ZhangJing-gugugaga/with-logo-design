# test-results — with-logo-design 压力测试结果

> 阶段 4 (darwin 兼容测试) 产物（v2 更新）

## 测试集

12 条 prompt（test-prompts.json），覆盖：
- 应调用（7 条）：奶茶店logo、咖啡标志、民宿正负形、律所标识、logo手法问答、**案例库引用(宠物店)**、**内部张力(极简vs十二生肖)**
- 不应调用（2 条）：海报、小红书文案
- 兄弟 skill 混淆（1 条）：VI 系统（含 logo 但范围更大）
- 边界（2 条）：动态3D logo、人民币国徽配色

## 预期结果

| 类别 | 数量 | 预期行为 |
|---|---|---|
| should_invoke | 7 | 激活 with-logo-design |
| should_not_invoke | 2 | 不激活 |
| sibling_trap | 1 | 激活但聚焦 logo 部分，说明与 doubao-creative-design 边界 |
| boundary | 2 | 激活但说明边界；违规内容拒绝 |

## v2 自测判定

- ✅ 描述字段含明确中英触发词，可被正确路由
- ✅ 案例库引用：t11 验证 AI 会读 examples/case-library.md 并按行业反查表执行
- ✅ 内部张力：t12 验证 AI 能判断品牌调性二选一，不硬拼
- ✅ 边界（B 段）明确列出不适用场景、内部张力、作者盲点
- ✅ 与 doubao-creative-design 的区分已写清（构思方法论 vs 视觉生成）
- ✅ 违规场景（人民币国徽）在 B 段显式禁止

## 待办

- 安装后可运行端到端盲测（由主流程或独立 agent 执行）
