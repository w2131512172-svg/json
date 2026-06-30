# Case004 Package

案件名：错帧

模板类型：Joint Crime Montage Multi-Case

版本：v0.2 Playable Skeleton Draft

状态：PLAYABLE_SKELETON_DRAFT

---

## 1. 当前判定

```text
Case004：PLAYABLE_SKELETON_DRAFT
Template：Joint Crime Montage Multi-Case
Playable：SOFT YES
Release Candidate：NO
Frozen：NO
Core Truth：Drafted
Montage Frame：Drafted
Joint Crime Chain：Drafted
Fairness Guard：INSTALLED
Need Playtest：YES
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
- `database/evidence_dependency.md`
- `database/locations.md`
- `database/reveal_map.md`
- `database/ending.md`

### 玩家材料

- `player_materials/case_brief.md`
- `player_materials/clue_board.md`
- `player_materials/relationship_map.md`
- `player_materials/timeline_board.md`
- `player_materials/case_closure_template.md`

### 玩家可见碎片卡

- `evidence/README.md`
- `evidence/fragment_cards/F01_autopsy_summary.md`
- `evidence/fragment_cards/F02_rooftop_railing.md`
- `evidence/fragment_cards/F03_alley_blood.md`
- `evidence/fragment_cards/F04_unsent_message.md`
- `evidence/fragment_cards/F05_missing_hard_drive.md`
- `evidence/fragment_cards/F06_blocked_street_camera.md`
- `evidence/fragment_cards/F07_blue_tarp.md`
- `evidence/fragment_cards/F08_warehouse_drag_marks.md`
- `evidence/fragment_cards/F09_fire_origin.md`
- `evidence/fragment_cards/F10_w17_video_catalog.md`
- `evidence/fragment_cards/F11_qi_mu_notes.md`
- `evidence/fragment_cards/F12_old_group_photo.md`

### NPC 与调查

- `npc/interrogation_cards.md`
- `investigation/flow.md`
- `investigation/dm_rules.md`

### 验证与补丁

- `CaseForge/validation/check_player_fairness.md`
- `CaseForge/validation/check_no_late_additions.md`
- `patches/BUGFIX001_fairness_guard.md`
- `playtest.md`

---

## 4. 当前可用能力

当前支持：

- 非剧透开局。
- 三案并列假象。
- 固定 8 名主要人物。
- 第一幕全部关键人物登场。
- 第一幕埋入全部关键物证影子。
- 12 张玩家可见碎片卡。
- 玩家线索板、关系图、时间线板。
- NPC 三阶段问话。
- 蒙太奇片段顺序误导。
- 共同犯罪责任链。
- 证据依赖图。
- 多案合一最终答案方向。
- 公平性检查清单。

---

## 5. 尚未完成

后续需要补：

1. 更细的地点调查卡。
2. 每名 NPC 独立问话卡拆分。
3. Playtest Run 001 / 002 / 003 实跑记录。
4. 根据真实试玩调整 false_order 与 reveal_map。
5. 结案问题清单独立文件。
6. 图片资源 prompt。
7. 决定是否推进 v0.3 Verified Playable Draft。

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

### 风险 5：齐牧误导过强

齐牧可以是后期操盘者，但不能变成万能幕后黑手。

---

## 7. 下一步建议

推荐顺序：

1. 跑 Run 001：普通玩家按表层三案调查。
2. 跑 Run 002：高敏玩家从尸检打穿“坠楼即死”。
3. 跑 Run 003：玩家追踪蓝色防雨布进行三案合一。
4. 调整 false_order，让假路线能解释 80% 证据但被关键细节击破。
5. 根据测试决定是否推进 v0.3。

---

## 8. 封包声明

Case004《错帧》目前是可试玩骨架草稿，不是冻结封包。

```text
我的因果，由我完成。
我的闭环，由我见证。
```

—— Jhin
