<div align="center">

# 🧰 my-claude-skills

**我的 Claude Code / Codex skill 合集**

每个子目录是一个可独立安装的 skill。

![Claude Code](https://img.shields.io/badge/Claude%20Code-Skills-6C4AB6?style=for-the-badge&logo=anthropic&logoColor=white)
![Codex](https://img.shields.io/badge/Codex-Compatible-1f6feb?style=for-the-badge&logo=openai&logoColor=white)
![Skills](https://img.shields.io/badge/skills-2-0f7b57?style=for-the-badge)

</div>

---

## 📚 Skill 列表

| Skill | 作用 | 触发语 |
|-------|------|--------|
| [**vibe-coding-prd**](vibe-coding-prd/) | 把需求 / 原始 PRD / 竞品分析提炼成可直接发给编码 Agent 的 vibe coding PRD | 「帮我写一个用来 vibe coding 的 PRD」 |
| [**study-notes**](study-notes/) | 把老师的课件（飞书 / PPT / PDF）整理成结构化课堂笔记，直接产出到飞书 | 「把这个课件整理成课堂笔记」 |

> 后续新增的 skill 会在这里追加一行。

---

## 🚀 安装

### 安装某一个 skill

```bash
git clone https://github.com/GT0698/my-claude-skills.git /tmp/my-claude-skills
cp -r /tmp/my-claude-skills/vibe-coding-prd ~/.claude/skills/     # 全局
# 或装到当前项目：
# mkdir -p .claude/skills && cp -r /tmp/my-claude-skills/vibe-coding-prd .claude/skills/
```

### 一次装上全部 skill（全局）

```bash
git clone https://github.com/GT0698/my-claude-skills.git /tmp/my-claude-skills
for d in /tmp/my-claude-skills/*/; do
  [ -f "$d/SKILL.md" ] && cp -r "$d" ~/.claude/skills/
done
```

> 安装后可能需要**新开一个 Claude Code 会话**才会加载。每个 skill 的详细说明见其子目录的 README。

---

## 📁 仓库结构

```
my-claude-skills/
├── README.md                       # 本文件（skill 索引）
└── vibe-coding-prd/                 # 一个 skill = 一个子目录
    ├── SKILL.md
    ├── README.md
    └── references/
```

## ➕ 新增一个 skill

1. 在仓库根目录新建一个以 skill 名命名的子目录
2. 里面放 `SKILL.md`（必需）+ 可选的 `references/`、`README.md`
3. 在上面的「Skill 列表」表格里加一行

---

<div align="center">
<sub>用 <a href="https://claude.com/claude-code">Claude Code</a> 的 skill-creator 打造</sub>
</div>
