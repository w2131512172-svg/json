# BUGFIX001：Fairness Guard

状态：DRAFT

---

## 1. 触发原因

Case003 后期出现过以下问题：

- 后期新增关键人物。
- 后期新增关键设定。
- 疑点越挖越多。
- 玩家无法通过已有证据闭环。

Case004 必须避免同类问题。

---

## 2. 本次修复目标

为 Case004 添加公平性护栏：

1. 玩家材料。
2. 线索卡。
3. NPC 三阶段问话。
4. 证据依赖图。
5. CaseForge 通用验证清单。

---

## 3. 已添加内容

### 玩家材料

- `player_materials/case_brief.md`
- `player_materials/clue_board.md`
- `player_materials/relationship_map.md`
- `player_materials/timeline_board.md`
- `player_materials/case_closure_template.md`

### 线索卡

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

### NPC 问话

- `npc/interrogation_cards.md`

### 依赖与验证

- `database/evidence_dependency.md`
- `CaseForge/validation/check_player_fairness.md`
- `CaseForge/validation/check_no_late_additions.md`

---

## 4. 当前判定

```text
Fairness Guard：INSTALLED
Playable：NOT YET
Need Playtest：YES
```

---

## 5. 后续建议

下一步应进行：

1. Run 001 表层三案路线模拟。
2. Run 002 尸检突破路线模拟。
3. 根据玩家是否过早发现共同犯罪，调整 false_order。
