# 教学技能库

集中维护用于备课、讲解、例题分析和复习的 Agent Skills。每个技能位于独立目录，可以单独使用和更新。

## 已有技能

| 技能 | 来源与用途 | 入口 |
|---|---|---|
| `bnu-math-grade9-volume1` | 北师大版数学九年级上册，2026年7月版；教师备课与讲解 | [SKILL.md](skills/bnu-math-grade9-volume1/SKILL.md) |

## 目录

```text
skills/
└── bnu-math-grade9-volume1/
    ├── SKILL.md
    ├── chapters/
    ├── glossary.md
    ├── patterns.md
    └── cheatsheet.md
```

后续技能在 `skills/` 下新增目录，每个目录保留自己的 `SKILL.md` 及相对引用的资料文件。

## 使用

将所需技能目录链接到 Agent 的技能目录。以本仓库位于 `~/Dev/github/teaching-skills` 为例：

```bash
mkdir -p ~/.agents/skills
ln -s ~/Dev/github/teaching-skills/skills/bnu-math-grade9-volume1 \
  ~/.agents/skills/bnu-math-grade9-volume1
```

目标路径已存在时先确认原有内容，不直接覆盖。新会话中可提出：

> 使用 bnu-math-grade9-volume1，为菱形的性质与判定设计一节40分钟的课，包含问题链、板书和练习答案。

## 资料范围

仅保存结构化技能，不保存教材PDF、原文提取结果或整页截图。教材技能包含综合提炼与明确标注的教学建议；具体图形题仍可能需要读取原教材。

本仓库按私有资料库维护。私有可见性不替代源资料使用与分享权限；新增资料按其来源权限处理。
