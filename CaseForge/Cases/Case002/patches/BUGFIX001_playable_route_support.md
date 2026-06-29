# BUGFIX 001：Playable Route Support

案件：Case002《第十九层》
状态：APPLIED
来源：Playtest Run 004

---

## 1. 问题摘要

Run 004 模拟真实玩家盲测结果为：

```text
SOFT PASS
```

案件核心逻辑可运行，但玩家可见材料不足，导致部分环节仍依赖 DM 临场概括。

---

## 2. 已修复问题

### GAP 001：社会关系背景不足

修复文件：

- `player_materials/social_background.md`

结果：玩家从家庭关系、校园矛盾、邻里关系切入时，有正式玩家材料可释放。

---

### GAP 002：公司线背景不足

修复文件：

- `player_materials/company_background.md`
- `evidence/E11_company_context.md`
- `evidence/E12_communication.md`

结果：玩家从死者工作单位、失踪资料、通讯异常切入时，有连续调查材料支撑。

---

### GAP 003：法医复检没有玩家证物卡

修复文件：

- `evidence/E10_forensics_review.md`

结果：玩家申请复检或质疑死亡时间线时，有正式证物卡可释放。

---

### GAP 004：NPC 问话需要标准化

修复文件：

- `npc/interrogation_cards.md`

结果：NPC 已支持初问、追问、破绽/收束三阶段问话。

---

## 3. 修复后验收标准

BUGFIX001 完成后，应满足：

1. 玩家从家庭线切入不会空转。
2. 玩家从公司线切入有足够材料继续查。
3. 玩家申请法医复检时有正式证物卡可释放。
4. DM 询问 NPC 时不需要临场生成核心回答。
5. Run 005 补丁后盲测达到 PASS 或高质量 SOFT PASS。

当前 1-4 已完成。

第 5 项待 Run 005 验证。

---

## 4. 当前状态

```text
BUGFIX001：APPLIED
Applied：YES
Need Verification：Run 005
```
