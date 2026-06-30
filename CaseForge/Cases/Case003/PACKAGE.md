# Case003 Package

案件名：第三次葬礼
模板类型：Fragmented Circular Narrative
版本：v0.1 Draft
状态：DRAFT

---

## 1. 当前判定

```text
Case003：DRAFT
Template：Fragmented Circular Narrative
Playable：NO
Release Candidate：NO
Frozen：NO
```

---

## 2. 已完成模块

### 核心入口

- `player.md`
- `secret.md`
- `assets_plan.md`
- `PACKAGE.md`

### 核心数据库

- `database/fragments.md`
- `database/perspectives.md`
- `database/causality.md`
- `database/false_order.md`
- `database/reveal_map.md`
- `database/npc.md`
- `database/evidence.md`
- `database/location.md`
- `database/dm_response.md`
- `database/ending.md`

### 玩家材料

- `player_materials/case_brief.md`
- `player_materials/clue_board.md`
- `player_materials/relationship_map.md`
- `player_materials/case_closure_template.md`

### NPC 与调查

- `npc/perspective_interrogation_cards.md`
- `investigation/flow.md`
- `investigation/anti_timeline_rules.md`

---

## 3. 当前可用能力

当前已经支持：

- 玩家非剧透开局。
- 多地点调查入口。
- 16 个碎片事件。
- 5 条视角线。
- 9 个因果节点。
- 6 条错误顺序路线。
- 6 个真相释放节点。
- 9 名核心 NPC。
- 分阶段问话卡。
- 玩家碎片板。
- 玩家关系图。
- 玩家结案模板。
- 防时间轴打穿规则。

---

## 4. 尚未完成

后续需要：

1. 创建 `playtest.md`。
2. 创建 `playtest_runs/run_001_fragment_collection.md`。
3. 创建 `playtest_runs/run_002_false_order_route.md`。
4. 创建 `playtest_runs/run_003_causality_closure.md`。
5. 补充玩家可见碎片卡目录。
6. 测试玩家是否会过早时间轴化。
7. 测试玩家是否能从碎片组合获得推进感。
8. 决定是否推进 v0.2 Playable Draft。

---

## 5. 风险点

### 风险 1：信息混乱度过高

碎片环形叙事容易让玩家前期迷失。需要 playtest 检查碎片释放节奏。

### 风险 2：误导过强

林小满线、诈尸传闻线、葬礼线都可能让玩家误锁单一路线，需要 reveal_map 保证可纠偏。

### 风险 3：核心真相过早被看穿

如果玩家很快抓住身份错位，案件可能提前进入后期。需要通过旧款线和责任层级保持难度。

### 风险 4：没有时间轴不等于没有结构

DM 必须坚持因果结构清晰，避免“为了非线性而混乱”。

---

## 6. 下一步建议

推荐顺序：

1. 补 `evidence/README.md` 与 `evidence/fragment_cards/`。
2. 创建 `playtest.md`。
3. 跑 Run 001：碎片收集路线。
4. 跑 Run 002：错误顺序路线。
5. 根据测试结果做 BUGFIX001。

---

## 7. 封包声明

Case003《第三次葬礼》目前为第一版开发草稿，不是可玩封包。

```text
我的因果，由我完成。
我的闭环，由我见证。
```

—— Jhin
