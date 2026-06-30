# Fragmented Circular Narrative Template

模板类型：多线环形叙事悬疑 / 无标准时间轴 / 因果闭环推理

适用案件：Case003 及后续高难度非线性案件。

---

## 1. 模板目标

本模板用于开发一种不同于 Case001、Case002 的推理案件。

它不以精确时间轴为核心，而以碎片、视角、误读、因果链为核心。

玩家一开始看到的不是完整案件，而是多个看似独立的故事片段。

最终目标是让玩家意识到：

```text
这些线不是并列案件，而是同一个核心事件在不同人物、不同误解、不同利益中的回声。
```

---

## 2. 与常规案件模板的区别

### 常规刑侦模板

核心问题：

```text
谁在什么时间、什么地点、用什么方式做了什么？
```

常见结构：

- timeline.md
- evidence.md
- npc.md
- location.md
- ending.md

### 碎片环形叙事模板

核心问题：

```text
哪个事件是因？哪个事件是果？谁误解了谁？哪些线其实是同一个闭环的不同侧面？
```

核心结构：

- fragments.md
- perspectives.md
- causality.md
- false_order.md
- reveal_map.md
- anti_timeline_rules.md

---

## 3. 玩家体验目标

玩家前期应感到：

- 案件像是多个不相关事件。
- 每条线都有自己的嫌疑人和动机。
- NPC 说法互相矛盾，但不一定是单纯撒谎。
- 没有一个人掌握完整真相。
- 时间顺序难以确定。

玩家中期应发现：

- 某些物品在多条线中重复出现。
- 某些证词说的是同一事件，但名称不同。
- 某些角色以为自己参与了 A，其实触发了 B。
- 某些“结果”其实是更早事件的“原因”。

玩家后期应完成：

- 碎片归组。
- 视角校正。
- 因果链重建。
- 环形闭合。
- 真相陈述。

---

## 4. 禁止事项

本模板不建议：

- 过早提供完整时间戳。
- 过早给出统一案发顺序。
- 让某个 NPC 单独说出完整真相。
- 用监控、门锁、GPS 等硬证据一刀切打穿案件。
- 把碎片叙事最终还原成普通线性刑侦题。

---

## 5. 推荐目录结构

```text
CaseForge/Cases/CaseXXX/
├─ player.md
├─ secret.md
├─ PACKAGE.md
├─ assets_plan.md
│
├─ database/
│  ├─ fragments.md
│  ├─ perspectives.md
│  ├─ causality.md
│  ├─ false_order.md
│  ├─ npc.md
│  ├─ evidence.md
│  ├─ location.md
│  ├─ reveal_map.md
│  ├─ dm_response.md
│  └─ ending.md
│
├─ player_materials/
│  ├─ case_brief.md
│  ├─ clue_board.md
│  ├─ relationship_map.md
│  └─ case_closure_template.md
│
├─ evidence/
│  ├─ README.md
│  └─ fragment_cards/
│
├─ npc/
│  └─ perspective_interrogation_cards.md
│
├─ investigation/
│  ├─ flow.md
│  └─ anti_timeline_rules.md
│
├─ playtest.md
├─ playtest_runs/
└─ patches/
```

---

## 6. 难度定位

推荐难度：高难 / 超高难。

适合玩家：

- 能处理多线信息。
- 能忍受前期混乱。
- 不依赖精确时间轴。
- 善于识别叙事误导和因果倒置。

---

## 7. 设计口号

```text
不是寻找时间顺序。
而是寻找因果闭环。
```
