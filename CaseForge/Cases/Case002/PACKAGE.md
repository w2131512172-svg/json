# Case002 Package

案件名：第十九层
版本：v0.2 Playable Draft
状态：PLAYABLE_DRAFT

---

## 1. 当前结论

Case002 已从第一版案件骨架推进到可试玩草稿。

当前判定：

```text
Case002：PLAYABLE_DRAFT
Playable：YES
Release Candidate：NO
Frozen：NO
```

---

## 2. 已完成模块

### 核心入口

- `player.md`
- `secret.md`
- `assets_plan.md`

### 核心数据库

- `database/npc.md`
- `database/evidence.md`
- `database/timeline.md`
- `database/location.md`
- `database/dm_response.md`
- `database/ending.md`
- `database/forensics.md`

### 调查流程

- `investigation/flow.md`

### 玩家材料

- `player_materials/case_brief.md`
- `player_materials/investigation_log.md`

### 玩家可见证物卡

- `evidence/README.md`
- `evidence/E01_door_lock_log.md`
- `evidence/E02_safe.md`
- `evidence/E03_blood_trace.md`
- `evidence/E04_phone.md`
- `evidence/E05_parking_cctv.md`
- `evidence/E06_call_record.md`
- `evidence/E07_forensics_preliminary.md`
- `evidence/E08_company_index.md`
- `evidence/E09_financial_record.md`

### 测试

- `playtest.md`
- `playtest_runs/run_001_standard_route.md`
- `playtest_runs/run_002_wrong_theft_route.md`
- `playtest_runs/run_003_early_executor_accusation.md`

---

## 3. 当前可玩范围

当前已经支持：

- 开局案件简报
- 基础地点调查
- NPC 质询
- 玩家可见证物释放
- 初步法医报告
- 技侦线索
- 死亡时间线推理
- 入室盗窃假象拆解
- 错误路线纠偏
- 过早结案拦截
- 公司线动机追查
- 结案判定
- S/A/B/C/D 评分框架

---

## 4. Playtest 结果

当前已完成三条模拟测试：

```text
Run 001 标准路线：SOFT PASS
Run 002 错误盗窃路线：PASS
Run 003 过早指控执行者：PASS
```

结论：

本案已经可以进行 DM 主持式试玩，但尚未达到 Release Candidate。

---

## 5. 尚未完成

后续仍建议补：

1. 更完整的 NPC 分阶段问话卡。
2. 更多玩家可见公司线材料。
3. 更细的法医复检报告卡。
4. 监控截图/门锁日志/现场平面图等图片资源。
5. 一次真实玩家试玩记录。
6. 根据真实试玩结果做 BUGFIX。
7. 决定是否冻结 v0.2 或推进 v0.3。

---

## 6. 风险点

### 风险 1：上游责任链需要控制释放

玩家可能较早锁定现场执行者，但不一定自然追到上游责任链。DM 需要利用结案反馈提醒：只抓到执行者不等于完整破案。

### 风险 2：证物卡仍偏摘要

目前证物卡可以支撑试玩，但还不是完全沉浸式 UI 文本。后续可补成正式证物档案。

### 风险 3：真实玩家可能走出未覆盖路线

目前 playtest 是模拟路线，真实玩家可能先查公司、先查学校、先查财务或乱序指控，需要进一步压力测试。

---

## 7. 下一步建议

推荐顺序：

1. 补 `npc/interrogation_cards.md`。
2. 补 `evidence/E10_forensics_dna.md`、`E11_company_materials.md`、`E12_communication.md`。
3. 做一次真实玩家试玩。
4. 根据试玩反馈决定是否进入 Release Candidate。

---

## 8. 封包声明

Case002《第十九层》目前为可试玩草稿，不是冻结封包。

```text
我的因果，由我完成。
我的闭环，由我见证。
```

—— Jhin
