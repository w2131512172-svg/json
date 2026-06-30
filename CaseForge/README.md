# CaseForge

这是一个用于开发和运行推理案件的仓库。

---

## 1. 目录规则

- `Cases/CaseXXX/player.md`：玩家可见入口。
- `Cases/CaseXXX/secret.md`：DM 数据库，案件结束前玩家不要查看。
- `Cases/CaseXXX/assets_plan.md`：图片与证物资源规划。
- `Cases/CaseXXX/PACKAGE.md`：案件状态、测试结果与封包记录。

---

## 2. 案件模板类型

CaseForge 当前支持两类案件模板。

### A. Standard Investigation Template

适合：

- 封闭空间案。
- 常规刑侦案。
- 时间线还原案。
- 证据链闭环案。

代表：

- Case001《雨夜咖啡馆》
- Case002《第十九层》

核心文件：

- `database/timeline.md`
- `database/evidence.md`
- `database/npc.md`
- `database/location.md`
- `database/dm_response.md`
- `database/ending.md`

### B. Fragmented Circular Narrative Template

适合：

- 多线叙事悬疑。
- 环形叙事案件。
- 无标准时间轴案件。
- 多视角误读案件。
- 因果闭环推理。

模板路径：

- `templates/fragmented_circular_narrative/`

核心文件：

- `database/fragments.md`
- `database/perspectives.md`
- `database/causality.md`
- `database/false_order.md`
- `database/reveal_map.md`
- `investigation/anti_timeline_rules.md`

设计原则：

```text
不是寻找时间顺序。
而是寻找因果闭环。
```

---

## 3. 冻结规则

当 `secret.md` 标记为 `FROZEN` 后，DM 不再修改以下内容：

- 真相
- 时间线 / 因果链
- NPC 知识边界
- 证据内容
- 调查结果
- 结案判定逻辑

如果游戏过程中发现逻辑漏洞，优先判定为案件设计 Bug，而不是临时修改设定。

---

## 4. 开发建议

### 常规刑侦案

优先开发：

1. 真相。
2. 时间线。
3. 证据链。
4. NPC 口供。
5. 结案判定。

### 碎片环形叙事案

优先开发：

1. 核心因果闭环。
2. 多条错误视角线。
3. 碎片事件。
4. 错误顺序与误读路线。
5. 真相释放地图。
6. 玩家碎片板与结案模板。

---

## 5. CaseForge 原则

```text
我的因果，由我完成。
我的闭环，由我见证。
```

—— Jhin
