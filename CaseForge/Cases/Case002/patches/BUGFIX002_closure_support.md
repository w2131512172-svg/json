# BUGFIX 002：Closure Support

案件：Case002《第十九层》
状态：PLANNED
来源：Playtest Run 005

---

## 1. 问题摘要

Run 005 结果：

```text
PASS
BUGFIX001：VERIFIED
```

补丁后盲测路线已经跑通，但发现三个收尾缺口：

1. 玩家侧缺少正式结案模板。
2. 证物目录未覆盖新增 E10-E12。
3. PACKAGE 未更新 Run 005 结果。

---

## 2. 需要修复的问题

### GAP 001：玩家结案模板缺失

修复文件：

- `player_materials/case_closure_template.md`

目标：让玩家按结构提交答案，降低表达成本，也方便 DM 判定。

---

### GAP 002：证物目录未更新

修复文件：

- `evidence/README.md`

目标：把 E10-E12 纳入索引。

---

### GAP 003：PACKAGE 状态未反映 Run 005

修复文件：

- `PACKAGE.md`

目标：记录 Run 005 PASS 与 BUGFIX001 VERIFIED。

---

## 3. 验收标准

BUGFIX002 完成后，应满足：

1. 玩家可使用正式模板提交结案。
2. 证物目录完整列出 E01-E12。
3. PACKAGE 能准确反映当前测试状态。
4. 可继续进入 Run 006：恶意/乱序路线压力测试。

---

## 4. 当前状态

```text
BUGFIX002：PLANNED
Applied：NO
```
