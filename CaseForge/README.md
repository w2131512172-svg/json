# CaseForge

这是一个用于开发和运行推理案件的仓库。

## 目录规则

- `Cases/Case001/player.md`：玩家可见入口。
- `Cases/Case001/secret.md`：DM数据库，案件结束前玩家不要查看。
- `Cases/Case001/assets_plan.md`：图片与证物资源规划。

## 冻结规则

当 `secret.md` 标记为 `FROZEN` 后，DM 不再修改以下内容：

- 真相
- 时间线
- NPC知识边界
- 证据内容
- 调查结果

如果游戏过程中发现逻辑漏洞，优先判定为案件设计Bug，而不是临时修改设定。
