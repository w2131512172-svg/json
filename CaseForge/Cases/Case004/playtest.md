# Case004 Playtest Plan

状态：SIMULATED_RUNS_001_004_COMPLETE

---

## 1. 测试目标

验证 Case004 是否满足：

```text
共同犯罪 + 蒙太奇 + 多案合一
```

同时避免 Case003 后期发散问题。

---

## 2. Run 001：表层三案路线

文件：`playtest_runs/run_001_surface_three_cases.md`

### 玩家行为模拟

玩家按常规刑侦处理：

1. 查坠楼现场。
2. 锁定沈知白。
3. 查仓库火灾。
4. 怀疑林若晴。
5. 查旧录像。
6. 怀疑齐牧。

### 测试目标

确认玩家能自然走入三案并列误导。

### 结果

```text
Run 001：SOFT PASS
```

结论：表层三案误导成立，但纠偏入口依赖尸检。

---

## 3. Run 002：尸检突破路线

文件：`playtest_runs/run_002_autopsy_breakthrough.md`

### 玩家行为模拟

玩家第一时间查尸检，发现：

```text
坠落伤 + 烟尘吸入
```

### 测试目标

确认高敏玩家能提前发现“坠楼即死”不成立。

### 结果

```text
Run 002：PASS
```

结论：高敏玩家可提前进入正确方向，但仍需拆责任链。

---

## 4. Run 003：重复物路线

文件：`playtest_runs/run_003_blue_tarp_route.md`

### 玩家行为模拟

玩家追踪蓝色防雨布。

### 测试目标

确认防雨布能自然连接三案，而不是显得过度刻意。

### 结果

```text
Run 003：PASS
```

结论：防雨布路线是稳定三案合一入口，不会直接剧透完整真相。

---

## 5. Run 004：误锁齐牧路线

文件：`playtest_runs/run_004_false_qi_mu_route.md`

### 玩家行为模拟

玩家认为齐牧是最终幕后黑手。

### 测试目标

确认 reveal_map 能纠偏：

```text
齐牧知道真相，但介入太晚，不可能造成死亡链起点。
```

### 结果

```text
Run 004：PASS
```

结论：齐牧误导成立，但可通过介入时间纠偏。

---

## 6. Run 005：共同犯罪结案路线

### 玩家行为模拟

玩家发现陆承舟坠楼后仍活着，开始追问：

```text
谁切断了救援？
```

### 测试目标

确认玩家能从单凶思维切换到责任链思维。

### 状态

```text
NOT_RUN
```

---

## 7. 当前测试结论

```text
Run 001：SOFT PASS
Run 002：PASS
Run 003：PASS
Run 004：PASS
Run 005：NOT_RUN
```

Case004 已具备可试玩骨架。

但尚未验证最终共同犯罪结案路线。

---

## 8. 失败指标

如果出现以下情况，需要重写：

1. 玩家认为新增隐藏人物才是真凶。
2. 玩家无法理解仓库为何是死亡完成点。
3. 玩家始终认为齐牧是万能幕后黑手。
4. 玩家无法区分沈知白和林若晴的责任层级。
5. 玩家觉得结局靠作者解释，而不是靠已收集证据推出。

---

## 9. 当前状态

```text
Playtest：RUN_001_004_SIMULATED
Need Fragment Cards：NO
Need NPC Cards：NO
Need Player Materials：NO
Need Run 005：YES
Need Real Player Test：YES
```
