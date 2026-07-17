# Ian Mychouchou Illustrations

> 把中文文章里的判断、流程、状态和隐喻，变成一张张白底、手绘、怪诞但清爽的正文配图。
>
> 16:9 横版 | 臭臭布偶猫 IP | 纯白手绘 | 少量红橙蓝中文批注 | Codex Skill

---

## 这个仓库是什么

Ian Mychouchou Illustrations 是一个独立的 Codex Skill 仓库，用来指导 AI Agent 为中文文章、帖子、博客、Notion 文档和方法论内容生成正文配图。

这个版本沿用原始 Ian 配图 skill 的工作流逻辑、构图逻辑和风格 DNA，但固定视觉 IP 已切换为 **臭臭 / mychouchou** —— 一只健硕、软糯、带一点小狮子威风感的布偶猫。

一句话：**让 AI 不只是“配一张图”，而是让臭臭把文章里的一个关键认知动作亲自做出来。**

---

## 当前确认的 IP 方向

- 名字：`mychouchou / 臭臭`
- 一个词识别点：`狮偶`
- 气质：健硕、乖、无辜、软糯，但上工时很靠谱
- 品种：布偶猫
- 特征：圆脸、大圆蓝眼、奶灰白双色、中长毛躯干、蓬松尾巴
- 体型：平衡结实，不胖、不短腿、不细长

参考母版图：`assets/mychouchou-reference-sheet-01.png`

---

## 安装

复制 skill 到 Codex skills 目录：

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./ian-mychouchou-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

安装后，在 Codex 里使用：

```text
Use $ian-mychouchou-illustrations 为这篇中文文章设计并生成 4 张臭臭怪诞正文配图。
```

---

## 仓库结构

```text
.
├── README.md
├── LICENSE
├── NOTICE.md
├── assets/
│   └── mychouchou-reference-sheet-01.png
└── ian-mychouchou-illustrations/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        ├── mychouchou-ip.md
        ├── composition-patterns.md
        ├── prompt-template.md
        ├── qa-checklist.md
        └── style-dna.md
```
