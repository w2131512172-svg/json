# Case003 Package

案件名：第三次葬礼
模板类型：Fragmented Circular Narrative
版本：v0.3 Verified Playable Draft
状态：VERIFIED_PLAYABLE_DRAFT

---

## 1. 当前判定

```text
Case003：VERIFIED_PLAYABLE_DRAFT
Template：Fragmented Circular Narrative
Playable：YES
Release Candidate：NO
Frozen：NO
BUGFIX001：VERIFIED
Run 004：PASS
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
- `player_materials/final_questions.md`
- `player_materials/rumor_clippings.md`

### 玩家可见碎片卡

- `evidence/README.md`
- `evidence/fragment_cards/F01_white_cloth_name.md`
- `evidence/fragment_cards/F02_second_gong.md`
- `evidence/fragment_cards/F03_account_page.md`
- `evidence/fragment_cards/F04_paper_effigy.md`
- `evidence/fragment_cards/F05_coffin_register.md`
- `evidence/fragment_cards/F06_child_witness.md`
- `evidence/fragment_cards/F07_bridge_stele.md`
- `evidence/fragment_cards/F08_keeper_statement.md`
- `evidence/fragment_cards/F09_old_coat.md`
- `evidence/fragment_cards/F10_stage_backdoor.md`
- `evidence/fragment_cards/F11_driver_route.md`
- `evidence/fragment_cards/F12_missing_portrait.md`
- `evidence/fragment_cards/F13_night_knock.md`
- `evidence/fragment_cards/F14_red_silk.md`
- `evidence/fragment_cards/F15_old_rope.md`
- `evidence/fragment_cards/F16_third_funeral_list.md`

### NPC 与调查

- `npc/perspective_interrogation_cards.md`
- `investigation/flow.md`
- `investigation/anti_timeline_rules.md`
- `investigation/final_review_scene.md`

### 测试与补丁

- `playtest.md`
- `playtest_runs/run_001_fragment_collection.md`
- `playtest_runs/run_002_false_order_route.md`
- `playtest_runs/run_003_causality_closure.md`
- `playtest_runs/run_004_after_bugfix_closure.md`
- `patches/BUGFIX001_closure_support.md`

---

## 3. 当前可用能力

当前已经支持：

- 玩家非剧透开局。
- 多地点调查入口。
- 16 个碎片事件。
- 16 张玩家可见碎片卡。
- 5 条视角线。
- 9 个因果节点。
- 6 条错误顺序路线。
- 6 个真相释放节点。
- 9 名核心 NPC。
- 分阶段问话卡。
- 玩家碎片板。
- 玩家关系图。
- 玩家结案模板。
- 最终结案问题清单。
- 传闻剪报。
- 最终核验场景。
- 防时间轴打穿规则。
- 四条模拟 playtest 路线。

---

## 4. Playtest 结果

```text
Run 001：SOFT PASS
Run 002：PASS
Run 003：SOFT PASS
Run 004：PASS
```

### Run 001 结论

碎片收集路线可以运行，但旧款线入口和碎片释放节奏需要继续观察。

### Run 002 结论

错误顺序路线成立，DM 可自然纠偏，不需要剧透。

### Run 003 结论

玩家可以从碎片进入因果闭环，但最终结案引导和责任层级拆分需要强化。

### Run 004 结论

BUGFIX001 已验证。

最终问题清单、最终核验场景、传闻剪报能够承接后期结案，责任层级比 Run 003 更清晰。

---

## 5. 当前结论

Case003 已具备 DM 主持式可试玩能力。

当前仍不是 Release Candidate，也未冻结。

---

## 6. 尚未完成

后续建议：

1. 真实玩家试玩。
2. 根据真实试玩调整 reveal_map。
3. 继续观察早期旧款线入口是否偏弱。
4. 补地点关系图或图片资源。
5. 根据真实试玩结果决定是否推进 Release Candidate。

---

## 7. 风险点

### 风险 1：信息混乱度过高

碎片环形叙事容易让玩家前期迷失。需要继续检查碎片释放节奏。

### 风险 2：误导过强

纸扎铺线、传闻线、葬礼线都可能让玩家误锁单一路线，需要 reveal_map 保证可纠偏。

### 风险 3：核心真相过早被看穿

如果玩家很快抓住身份错位，案件可能提前进入后期。需要通过旧款线和责任层级保持难度。

### 风险 4：没有时间轴不等于没有结构

DM 必须坚持因果结构清晰，避免“为了非线性而混乱”。

---

## 8. 下一步建议

推荐顺序：

1. 补 `assets/location_map_prompt.md`。
2. 跑一次真实玩家试玩。
3. 根据真实试玩反馈做 BUGFIX002。
4. 决定是否推进 v0.4 Release Candidate。

---

## 9. 封包声明

Case003《第三次葬礼》目前为已验证可试玩草稿，不是冻结封包。

```text
我的因果，由我完成。
我的闭环，由我见证。
```

—— Jhin
