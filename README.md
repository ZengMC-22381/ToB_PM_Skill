# prd-writer-b2b

一个面向 ToB / 中后台产品经理的 PRD 写作 Skill。

## 核心特点

- 主结构稳定：版本信息 / 需求背景 / Roadmap / 需求详情
- 表达偏产品视角，不默认下沉到接口和表结构
- 支持先读取现有业务逻辑，再输出独立的新 PRD
- 最终统一以 `.md` 文件交付，不把完整正文直接输出在答案中

## 目录说明

```text
prd-writer-b2b/
├── SKILL.md
├── README.md
├── examples/
│   ├── label-management-prd.md
│   ├── approval-workflow-config-prd.md
│   └── role-permission-management-prd.md
└── references/
    ├── prd-template.md
    ├── writing-style.md
    ├── input-checklist.md
    ├── context-reading-guide.md
    ├── current-state-summary-template.md
    └── current-state-usage.md
```

## 推荐用法

### 从零起草

```text
请使用 prd-writer-b2b Skill，基于以下信息生成一份独立的 PRD md 文件。
```

### 基于旧资料写增量需求

```text
请使用 prd-writer-b2b Skill。
先根据参考资料理解当前业务逻辑，再输出一份独立的新 PRD md 文件。
注意：参考资料仅用于参考，不要与新 PRD 混写。
```
