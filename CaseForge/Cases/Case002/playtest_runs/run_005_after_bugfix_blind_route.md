# Playtest Run 005：BUGFIX001 后盲测路线

案件：Case002《第十九层》
状态：PATCH VERIFICATION
路线类型：补丁后模拟真实玩家盲测

---

## 0. 测试边界

本次测试用于验证 BUGFIX001 是否解决 Run 004 中暴露的问题。

玩家仍只读取玩家可见材料：

- `player.md`
- `player_materials/case_brief.md`
- `player_materials/investigation_log.md`
- 按调查进度释放的 `player_materials/` 背景材料
- 按调查进度释放的 `evidence/` 证物卡

玩家不读取：

- `secret.md`
- `database/`
- `npc/interrogation_cards.md`
- `investigation/flow.md`
- `playtest_runs/`

---

## 1. 测试目标

验证四个修复点：

1. 玩家从家庭/校园/邻里关系切入时是否不再空转。
2. 玩家从公司线切入时是否有足够公开材料继续推进。
3. 玩家申请法医复检时是否有正式证物卡可释放。
4. NPC 问话是否可按阶段运行，不依赖 DM 临场编造。

---

## 2. 模拟路线 A：玩家先查社会关系

### 玩家行动

> 先查家庭关系、邻居说法、女儿学校关系。

### 可释放材料

- `player_materials/social_background.md`
- NPC 初问：林薇、唐静、陆骁、刘阿姨

### 测试观察

玩家可以获得足够多的背景噪音与合理误导，但这些材料不会直接替玩家解案。

社会关系线现在具备：

- 家庭压力。
- 校园矛盾。
- 邻里发现节点。
- 情绪型误导方向。

### 判定

```text
PASS
```

Run 004 的 GAP 001 已修复。

---

## 3. 模拟路线 B：玩家先查公司线

### 玩家行动

> 死者是企业高管，先查公司背景、近期项目、工作压力。

### 可释放材料

- `player_materials/company_background.md`
- `evidence/E08_company_index.md`
- `evidence/E11_company_context.md`
- `evidence/E12_communication.md`

### 测试观察

公司线不再只有一句“死者工作有问题”。

玩家可以从：

- 公司背景。
- 死者岗位。
- 文件流转异常。
- 外接设备线索。
- 通讯记录异常。

逐步形成调查方向。

### 判定

```text
PASS
```

Run 004 的 GAP 002 已修复。

---

## 4. 模拟路线 C：玩家质疑死亡顺序

### 玩家行动

> 三个人是不是同一时间死的？申请更详细法医复检。

### 可释放材料

- `evidence/E07_forensics_preliminary.md`
- `evidence/E10_forensics_review.md`
- 需要时由 `database/forensics.md` 作为 DM 后台支撑

### 测试观察

玩家现在能看到正式复检摘要，而不是只听 DM 口头总结。

复检材料能支持：

- 三人遭遇过程不同。
- 现场存在事件先后变化。
- 死亡时间线需要结合电子证据和现场证据判断。

### 判定

```text
PASS
```

Run 004 的 GAP 003 已修复。

---

## 5. 模拟路线 D：玩家集中问话 NPC

### 玩家行动

> 逐个问询关键人物，并根据已发现证据追问。

### 可使用材料

- `npc/interrogation_cards.md`
- `database/npc.md`
- `database/dm_response.md`

### 测试观察

NPC 现在具备三层响应：

1. 初问。
2. 追问。
3. 破绽/收束。

玩家不带证据时，NPC 不会过早自爆。

玩家带证据追问时，DM 有标准回答可调用。

### 判定

```text
PASS
```

Run 004 的 GAP 004 已修复。

---

## 6. 模拟综合路线

### 玩家路线

```text
案件简报
→ 先查社会关系
→ 发现社会线存在噪音但不足以解释现场
→ 转查门锁/监控
→ 锁定有权限进入路径
→ 查法医复检
→ 发现死亡过程存在先后差异
→ 查失踪物品
→ 转入公司线
→ 结合通讯/公司/财务/现场证据
→ 提交结案陈述
```

### 测试观察

补丁后，玩家可以沿非标准路线完成调查，不需要 DM 主动补设定。

当前仍可能需要 DM 控制证据释放节奏，但这属于推理游戏主持正常流程，不再属于材料缺失。

### 判定

```text
PASS
```

---

## 7. 本轮发现的新问题

### NEW GAP 001：正式结案模板缺失

当前 `ending.md` 有 DM 结案逻辑，但玩家侧缺少 `case_closure_template.md`。

影响：中等。

建议：补充玩家可见结案模板，降低玩家提交答案时的表达成本。

---

### NEW GAP 002：证物目录未更新 E10-E12

`evidence/README.md` 当前索引可能未覆盖新增 E10-E12。

影响：低。

建议：更新证物目录。

---

### NEW GAP 003：PACKAGE 状态未反映 Run 005

需要更新 `PACKAGE.md` 的测试结果与下一步建议。

影响：低。

建议：更新 PACKAGE。

---

## 8. 测试结论

```text
Run 005：PASS
BUGFIX001：VERIFIED
```

Case002 已从“可试玩草稿”推进到“高质量可试玩草稿”。

尚未建议冻结为 Release Candidate，原因：

1. 还缺玩家可见结案模板。
2. 证物目录需要更新。
3. 仍建议再跑一次恶意/乱序路线测试。

---

## 9. 下一步建议

推荐执行 BUGFIX002：Closure Support

应包括：

- `player_materials/case_closure_template.md`
- 更新 `evidence/README.md`
- 更新 `PACKAGE.md`
- 新增 `playtest_runs/run_006_chaotic_route.md`
