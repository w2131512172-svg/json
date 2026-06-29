# BUGFIX 001：Playable Route Support

案件：Case002《第十九层》
状态：PLANNED
来源：Playtest Run 004

---

## 1. 问题摘要

Run 004 模拟真实玩家盲测结果为：

```text
SOFT PASS
```

案件核心逻辑可运行，但玩家可见材料不足，导致部分环节仍依赖 DM 临场概括。

---

## 2. 需要修复的问题

### GAP 001：社会关系背景不足

玩家若优先调查家庭关系、校园矛盾，当前可见材料较少。

修复文件：

- `player_materials/social_background.md`

---

### GAP 002：公司线背景不足

玩家若追查死者工作单位，当前只有索引和摘要，缺少正式背景材料。

修复文件：

- `player_materials/company_background.md`
- `evidence/E11_company_context.md`

---

### GAP 003：法医复检没有玩家证物卡

DM 数据库有复检内容，但玩家可见材料只有初检。

修复文件：

- `evidence/E10_forensics_review.md`

---

### GAP 004：NPC 问话需要标准化

当前 NPC 可主持，但缺少分阶段问话卡。

修复文件：

- `npc/interrogation_cards.md`

---

## 3. 修复后验收标准

BUGFIX001 完成后，应满足：

1. 玩家从家庭线切入不会空转。
2. 玩家从公司线切入有足够材料继续查。
3. 玩家申请法医复检时有正式证物卡可释放。
4. DM 询问 NPC 时不需要临场生成核心回答。
5. Run 005 补丁后盲测达到 PASS 或高质量 SOFT PASS。

---

## 4. 当前状态

```text
BUGFIX001：PLANNED
Applied：NO
```
