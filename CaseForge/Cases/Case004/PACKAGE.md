# Case004 Package

案件名：错帧

模板类型：Joint Crime Montage Multi-Case

版本：v0.1 Concept Draft

状态：CONCEPT_DRAFT

---

## 1. 当前判定

```text
Case004：CONCEPT_DRAFT
Template：Joint Crime Montage Multi-Case
Playable：NO
Release Candidate：NO
Frozen：NO
Core Truth：Drafted
Montage Frame：Drafted
Joint Crime Chain：Drafted
```

---

## 2. 设计目标

Case004 目标是融合三种结构：

1. 共同犯罪。
2. 蒙太奇误导。
3. 多案合一。

玩家表面上会面对三起案件：

```text
A 案：雨夜坠楼案
B 案：仓库纵火案
C 案：旧录像失踪案
```

最终真相：

```text
三案不是独立事件，而是同一晚同一死亡事件在不同时间片、不同伪装、不同责任人手中形成的连锁闭环。
```

---

## 3. 已建立模块

### 核心入口

- `player.md`
- `secret.md`
- `assets_plan.md`
- `PACKAGE.md`

### 核心数据库

- `database/cases_surface.md`
- `database/montage_fragments.md`
- `database/true_order.md`
- `database/false_order.md`
- `database/joint_crime_chain.md`
- `database/npc.md`
- `database/evidence.md`
- `database/locations.md`
- `database/reveal_map.md`
- `database/ending.md`

### 调查与测试

- `investigation/flow.md`
- `investigation/dm_rules.md`
- `playtest.md`

---

## 4. 当前可用能力

当前支持：

- 非剧透开局。
- 三案并列假象。
- 固定 8 名主要人物。
- 第一幕全部关键人物登场。
- 第一幕埋入全部关键物证影子。
- 蒙太奇片段顺序误导。
- 共同犯罪责任链草案。
- 多案合一最终答案方向。

---

## 5. 尚未完成

后续需要补：

1. 玩家可见线索卡。
2. NPC 分阶段问话卡。
3. 地点调查细节。
4. 证据释放节奏。
5. Playtest 路线。
6. 结案问题清单。
7. 真实试玩后 BUGFIX001。

---

## 6. 风险点

### 风险 1：复杂度过高

共同犯罪 + 蒙太奇 + 多案合一容易导致玩家早期迷失。

### 风险 2：误导过强

必须保证玩家能在中段通过物证重复点发现“三案同源”。

### 风险 3：责任链不清

共同犯罪必须拆分责任层级，避免玩家误以为“所有人都一样有罪”。

### 风险 4：蒙太奇不公平

所有错序片段必须可被玩家通过细节校正，不能靠结尾硬解释。

---

## 7. 下一步建议

推荐顺序：

1. 补 `player_materials/case_brief.md`。
2. 补 `evidence/fragment_cards/`。
3. 补 NPC 问话卡。
4. 跑 Run 001：普通玩家按表层三案调查。
5. 跑 Run 002：高敏玩家尝试三案合一。
6. 根据测试调整 reveal_map。

---

## 8. 封包声明

Case004《错帧》目前是概念草稿，不可直接作为正式 DM 案件运行。

```text
我的因果，由我完成。
我的闭环，由我见证。
```

—— Jhin
