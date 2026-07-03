<div align="center">

# 📝 study-notes（课堂笔记整理）

**把老师的课件（飞书文档 / PPT / PDF）整理成结构化课堂笔记，直接产出到飞书。**

也能在你已有部分笔记时，保守地帮你修订。

![Feishu](https://img.shields.io/badge/输出-飞书文档-00D6B9?style=for-the-badge)
![Input](https://img.shields.io/badge/输入-飞书%20·%20PPT%20·%20PDF-1f6feb?style=for-the-badge)
![Confirm](https://img.shields.io/badge/修订-保守%20·%20不删原文-e0533d?style=for-the-badge)

</div>

---

## ✨ 它做什么

课件大多是"讲课顺序 + 满屏图片"，不适合日后速查。这个 skill 把课件**按主题重组**成一套固定结构的笔记，让你"忘了某个知识点时，看一眼就知道细节"。

## 🧱 固定三块结构

```
# {日期}{课程名}课堂笔记
# 课堂重点      ← skill 生成/修订：按主题重排，定义/流程/对照分层呈现
# 课程资料      ← 只留「标题三 + 序号」粘贴区，你实时补资料网址/课件
# 课后任务      ← 只留带标签的空待办，你实时补
```

## 📐 排版规则（都已内置）

- **层级 ≤ 5 层**；标题序号单位优先（`一/二/三`、`1/2/3`），最多 `1.1`，绝不 `1.1.1`
- **并列**用无序列表、**递进/次序**用数字（每个结构内重新起号）
- **纲领/结论句** → 飞书**高亮块**（callout）；段内关键处**加粗**
- **能层级化的不上表格**，只有多维对照复杂才用表格
- **图片**：从零转笔记不留图、全文字化；修订模式单图转文字后可留图并标"（图1）"

## 🗂️ 产出位置（自动判断）

| 情况 | 建到哪 |
|------|--------|
| 素材是某知识库里的在线文档 | 同一个知识库、同目录（不问） |
| 你指定了知识库/目录 | 按你说的 |
| 素材来自文档库/零散云文档 | 生成前弹框让你选 |
| 兜底（没说/跳过/本地 PPT·PDF） | **默认文档库**，绝不落云盘 |

## 🚀 安装

```bash
git clone https://github.com/GT0698/my-claude-skills.git /tmp/my-claude-skills
cp -r /tmp/my-claude-skills/study-notes ~/.claude/skills/     # 全局
# 或装到当前项目：
# mkdir -p .claude/skills && cp -r /tmp/my-claude-skills/study-notes .claude/skills/
```

## 💬 怎么用

```
把这个课件整理成课堂笔记
<粘贴课件：飞书链接 / .pptx / .pdf>
```

默认直接产出到飞书；需要 markdown 草稿时，单独说一声即可。
