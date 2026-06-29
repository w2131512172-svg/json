# Case002 Package

案件名：第十九层
版本：v0.1 Draft
状态：DRAFT

---

## 1. 当前结论

Case002 已完成第一版案件骨架。

当前判定：

```text
Case002：DRAFT
Playable：BASIC
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

### 玩家材料

- `player_materials/case_brief.md`
- `player_materials/investigation_log.md`

---

## 3. 案件核心

本案是一起伪装成入室盗窃的重大刑事杀人案。

核心结构：

```text
周启山：主谋
何锐：执行者
陈昊：协助掩护者
顾明远：原始目标
赵雅琴：撞破异常后被灭口
顾念：发现执行者后被灭口
```

---

## 4. 当前可玩范围

当前已经支持：

- 开局案件简报
- 基础地点调查
- NPC 质询
- 证据发现
- 死亡时间线推理
- 入室盗窃假象拆解
- 公司线动机追查
- 结案判定
- S/A/B/C/D 评分框架

---

## 5. 尚未完成

后续需要：

1. 增加 `playtest.md`。
2. 跑一次标准路线 Playtest Run 001。
3. 检查证据是否过早暴露真凶。
4. 检查误导项是否合理但不恶意。
5. 补充更细的法医报告。
6. 补充公司财务线细节。
7. 补充玩家可见证物文本。
8. 决定是否冻结 v0.1。

---

## 6. 风险点

### 风险 1：主谋证据可能偏直给

周启山与转账、陈昊、举报材料之间的连接需要在 playtest 中控制释放节奏。

### 风险 2：何锐过早暴露

何锐拥有备用权限、车辆记录和伤口三重线索，玩家可能很快锁定执行者。但这可以接受，因为本案重点不是“谁挥刀”，而是“谁让他挥刀”。

### 风险 3：三人死亡顺序需要更精细法医支持

目前已有顾念通话、顾明远血迹、赵雅琴回家记录，但可继续补强尸温、胃内容物、血液凝固等法医细节。

---

## 7. 下一步建议

推荐顺序：

1. 创建 `playtest.md`。
2. 创建 `playtest_runs/run_001_standard_route.md`。
3. 补充 `database/forensics.md`。
4. 补充 `evidence/` 目录下玩家可见证物卡。
5. 进行一次模拟游玩。

---

## 8. 封包声明

Case002《第十九层》目前不是冻结封包，而是第一版可开发案件包。

```text
我的因果，由我完成。
我的闭环，由我见证。
```

—— Jhin
