# Package Template

案件编号：CaseXXX
案件名：待填写
版本：v0.1 Release Candidate
状态：UNFROZEN

---

## 1. 封包前条件

封包前必须满足：

- [ ] 核心数据库完成。
- [ ] 玩家材料完成。
- [ ] 至少一轮标准路线 Playtest 完成。
- [ ] 致命 Bug 已修复。
- [ ] ending.md 可执行结案判定。
- [ ] 没有无法获得的关键证据。

---

## 2. 已完成模块

### 核心数据库

- [ ] `database/npc.md`
- [ ] `database/evidence.md`
- [ ] `database/timeline.md`
- [ ] `database/location.md`
- [ ] `database/dm_response.md`
- [ ] `database/ending.md`

### 玩家材料

- [ ] `player_materials/case_brief.md`
- [ ] `player_materials/investigation_log.md`
- [ ] `player_materials/case_closure_template.md`

### 测试与补丁

- [ ] `playtest/playtest.md`
- [ ] `playtest/runs/*`
- [ ] `patches/*` 如有

---

## 3. 冻结范围

封包后冻结：

- 核心真相
- 核心事件方式
- 核心时间线
- 核心执行者/真相主体
- 核心动机
- 核心证据链
- 主要 NPC 关系
- 主要误导链
- 结案判定逻辑

---

## 4. 允许小修

- 错别字
- Markdown 格式
- 玩家说明
- DM 提示语气
- Render 需求记录
- 非关键体验说明

---

## 5. 禁止大改

- 更换核心真相
- 更改核心手法
- 更改关键时间线
- 新增改变结案逻辑的证据
- 删除已通过 Playtest 的主线结构

---

## 6. 封包声明

```text
CaseXXX：待封包
Release Candidate：NO
Frozen：NO
```
