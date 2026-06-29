# Case001 Package

案件名：雨夜咖啡馆
版本：v0.1 Release Candidate
状态：FROZEN

---

## 1. 封包结论

Case001 已完成第一版可玩封包。

当前判定：

```text
Case001：PASS
Release Candidate：YES
Package：v0.1
Frozen：YES
```

本案已经通过：

- 标准路线 Playtest Run 001：SOFT PASS
- BUGFIX 001：完成
- 标准路线 Playtest Run 002：PASS

---

## 2. 已完成模块

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
- `player_materials/case_closure_template.md`

### 测试与补丁

- `playtest.md`
- `playtest_runs/run_001_standard_route.md`
- `playtest_runs/run_002_standard_route_after_bugfix.md`
- `patches/location_bugfix001.md`

---

## 3. 冻结范围

从本文件创建后，以下内容进入冻结状态：

- 核心真相
- 死亡方式
- 死亡时间线
- 核心执行者
- 核心动机
- 核心证据链
- 主要 NPC 关系
- 主要误导链
- 结案判定逻辑

除非发现致命逻辑 Bug，否则不得大改以上内容。

---

## 4. 允许的小修范围

封包后仍允许：

- 修复错别字。
- 调整 Markdown 格式。
- 优化玩家说明。
- 优化 DM 提示语气。
- 增加图片提示词。
- 增加封面/宣传文案。
- 增加非关键体验说明。
- 修复不会改变主线真相的轻微矛盾。

---

## 5. 禁止的大改范围

封包后禁止：

- 更换核心执行者。
- 更改死亡方式。
- 更改真实死亡窗口。
- 新增核心嫌疑人。
- 删除关键证据链。
- 将支线 NPC 改成共犯。
- 新增会改变结案逻辑的证据。
- 推翻已通过 Playtest 的主线结构。

---

## 6. 可玩状态

当前案件支持：

- 开局调查
- 地点探索
- 证据发现
- NPC 质询
- 时间线修正
- 阶段性推理
- 结案判定
- S/A/B/C/D 评分
- 错误嫌疑人反馈
- 证据不足反馈

---

## 7. 已知非阻塞问题

以下问题不影响 v0.1 封包：

- S级全收集条件仍可后续细化。
- 部分复盘文本可继续润色。
- 案件图片尚未生成。
- 恶意玩家路线未完整跑，但 ending.md 已具备拦截过早结案能力。

---

## 8. 后续建议

封包后推荐顺序：

1. 生成案件封面图/场景图提示词。
2. 准备玩家正式游玩入口。
3. 做一次真实玩家试玩。
4. 根据真实玩家反馈做小修。
5. 开始 Case002。

---

## 9. 封包声明

Case001《雨夜咖啡馆》v0.1 已完成第一版封包。

从这一刻起，它不再是“内容开发中”的案件，而是一个可被运行、可被试玩、可被验证的 CaseForge 第一案。

```text
我的因果，由我完成。
我的闭环，由我见证。
```

—— Jhin
