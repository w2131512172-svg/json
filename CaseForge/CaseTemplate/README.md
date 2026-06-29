# CaseForge CaseTemplate

状态：TEMPLATE
用途：案件工程骨架

> 本目录是 CaseForge 的通用案件模板。
> 只允许包含结构、字段、规则、占位说明，不包含任何具体案件剧情、凶手、证据答案或真相。

---

## 目录结构

```text
CaseTemplate/
├── database/
│   ├── npc.md
│   ├── evidence.md
│   ├── timeline.md
│   ├── location.md
│   ├── dm_response.md
│   └── ending.md
├── player_materials/
│   ├── case_brief.md
│   ├── investigation_log.md
│   └── case_closure_template.md
├── design/
│   └── design.md
├── playtest/
│   ├── playtest.md
│   └── runs/.gitkeep
├── patches/.gitkeep
├── render/.gitkeep
└── PACKAGE.md
```

---

## 使用方式

1. 复制 `CaseTemplate/`。
2. 重命名为 `Cases/CaseXXX/`。
3. 按顺序填写：
   - `design/design.md`
   - `database/npc.md`
   - `database/evidence.md`
   - `database/timeline.md`
   - `database/location.md`
   - `database/dm_response.md`
   - `database/ending.md`
   - `player_materials/*`
4. 执行 `playtest/playtest.md` 中的测试路线。
5. 通过后创建 `PACKAGE.md` 并进入冻结。

---

## 模板原则

- 案件数据优先，表现形式次之。
- 玩家材料不得剧透 DM 内部数据库。
- DM 不因玩家猜中姓名而直接判定成功，必须检查证据链。
- 高密度地点必须分层调查。
- 关键证据必须有可获得入口。
- Playtest 结果决定是否封包。

---

## Render 说明

`render/` 目录暂时作为占位。

Renderable Object 不是图片素材库，而是用于未来记录“可观察对象”的结构化描述。它应服务于推理，而不是装饰。
