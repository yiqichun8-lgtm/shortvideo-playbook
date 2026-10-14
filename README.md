# 实体生意短视频实操方法论 · Skill 包

把一套面向实体生意经营者的短视频方法论，体系化成 **8 个可直接安装调用的 skill 入口**，覆盖「定位 → 选题 → 脚本 → 自检」全链路。

> **声明**：本仓库为**自用方法论体系**，是长期实践与体系化整理的成果，归纳自大量真实案例。
> 原始素材（含未公开的访谈与案例记录）**未纳入本仓库**，此处仅保留方法论骨架。

---

## 核心主张

> 做短视频不靠创意，靠工程。

先锁死「进店理由」（商业定位），再用**四类脚本的固定结构 × 八大爆款元素**批量出选题，以原生、高频、多维的内容，把「相信并进店的理由」持续晒给精准本地用户。

---

## 8 个入口

| 当你…… | 用这个 |
|---|---|
| 不知道有什么可拍 / 有播放没客人 | `shortvideo-positioning` |
| 缺选题、标题不够勾人 | `shortvideo-topic-generator` |
| 想表态、借热点说话 | `shortvideo-opinion-script` |
| 拍进货、备餐、服务过程 | `shortvideo-process-script` |
| 做干货内容涨粉 | `shortvideo-knowledge-script` |
| 讲创业经历、夸员工、做店庆 | `shortvideo-story-script` |
| 判断这条能不能发 / 数据差在哪 | `shortvideo-script-selfcheck` |
| 不确定走哪个 / 想查术语 | `shortvideo-playbook`（路由） |

**`shortvideo-playbook` 是路由总入口**，内含 15 张能力卡的完整索引。另外 8 张补充卡（AI 出选题提示词公式、拍摄基础、剪辑工作流、自然流引导、拆片法、进阶大制作脚本、IP 问卷、矩阵团队）挂在路由下按需调用，不单独占触发位。

---

## 安装

这套 skill 用的是 **`SKILL.md` 开放标准**（[agentskills.io](https://agentskills.io)），
Codex CLI、Claude Code、Cursor、Gemini CLI 等 38+ 平台通用。只需放到对应工具的 skills 目录：

| 工具 | 安装命令（在 `dist/shortvideo-playbook/` 目录下执行） |
|---|---|
| **WorkBuddy** | `cp -R shortvideo-* ~/.workbuddy/skills/` |
| **Codex CLI** | `cp -R shortvideo-* ~/.codex/skills/` |
| **Claude Code** | `cp -R shortvideo-* ~/.claude/skills/` |
| **Cursor / 其他** | 放到该项目/工具的 skills 目录即可 |

项目级安装（团队共享）：把 `shortvideo-*` 放进仓库根的 `.codex/skills/` 并提交，
所有人克隆后自动生效。

```bash
git clone https://github.com/<YOUR_USERNAME>/shortvideo-playbook.git
cd shortvideo-playbook/dist/shortvideo-playbook
cp -R shortvideo-* ~/.workbuddy/skills/
```

重启对应工具生效。新会话中输入 `/skills` 可确认是否已加载。

---

## 用法示例

**不用记命令**，描述你的处境就行，它会靠 `description` 自动匹配：

```
我开了一家开了 8 年的社区面馆，人均 25，主要靠回头客，
但年轻人越来越少，帮我找进店理由。
```

想指定就用 `/` 或 `$` 前缀：

```
$shortvideo-positioning 我开了一家开了 8 年的社区面馆，人均 25，
主要靠回头客，帮我捋清楚到底靠什么让人专门跑一趟。
```

```
$shortvideo-topic-generator 我的核心优势是"现炒现做、拒绝预制菜"，
给我 10 个下周就能拍的选题，按钩子强度排个序。
```

```
$shortvideo-script-selfcheck 帮我看看这条脚本能不能发：[粘贴脚本]
```

---

## 目录结构

```
.
├── dist/shortvideo-playbook/        ← 编译产物，可直接安装
│   ├── shortvideo-playbook/         ← 路由入口（含 15 张卡索引）
│   ├── shortvideo-positioning/
│   ├── shortvideo-topic-generator/
│   ├── shortvideo-opinion-script/
│   ├── shortvideo-process-script/
│   ├── shortvideo-knowledge-script/
│   ├── shortvideo-story-script/
│   └── shortvideo-script-selfcheck/
│
├── books/shortvideo-playbook/       ← 方法论全貌（原始素材已排除）
│   ├── BOOK_OVERVIEW.md      体系总览
│   ├── DIGEST.md             精华长文，建议从这里读起
│   ├── GLOSSARY.md           术语词典
│   ├── verified.md           验证记录
│   ├── PIPELINE_STATE.md     整理过程
│   ├── tests/                触发评测用例
│   └── .cangjie/capabilities/ 15 张能力卡 + 清单（可重新编译）
│
└── README.md
```

---

## 已知边界（重要）

这套方法论有明确适用范围，用之前请知道：

1. **绑定自然流红利期**。付费流量占比上升后，「靠内容白嫖流量」的难度显著变大。
2. **不要承诺效果**。定位正确提高的是变现概率，不保证结果。
3. **幸存者偏差**。看到的成功案例都是筛选后的结果，做不起来的不会出现在案例里。
4. **工业化套路的同质化反噬**。同一套爆款元素被同行批量复用后，边际效果会下降。
5. **内容治不了产品**。如果复购和出品做不好，涨粉只会让差评传播得更快。
6. **平台风险**。「荷尔蒙」类擦边元素在当前治理下是高危项，代价是限流或封号。

术语「情绪波点」「置身事外」的确切含义尚未完全敲定，已在 `GLOSSARY.md` 中标注待确认并给出推测定义。
