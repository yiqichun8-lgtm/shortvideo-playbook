# 餐饮短视频课程体系 · 蒸馏 Skill 包

把一套餐饮/实体店短视频线下课与进阶课（含 34 万字口播逐字稿）蒸馏成 **8 个可直接安装调用的 skill 入口**，覆盖"定位 → 选题 → 脚本 → 自检"全链路。

> **声明**：本仓库为**自用蒸馏产物**，是对课程内容的理解、重构与二次表达，非课程官方材料。原始逐字稿与源文档因版权原因**未纳入本仓库**。知识归属原课程体系，本仓库仅保留方法论骨架与个人批注。

---

## 核心主张

> 实体店老板做短视频不靠创意，靠工程。

先锁死「进店理由」（商业定位），再用**四类脚本的固定结构 × 八大爆款元素**批量出选题，以原生、高频、多维的内容，把「相信并进店的理由」持续晒给精准本地用户。

---

## 8 个入口

| 当你…… | 用这个 |
|---|---|
| 不知道有什么可拍 / 有播放没客人 | `canyin-positioning` |
| 缺选题、标题不够勾人 | `canyin-topic-generator` |
| 想表态、借热点说话 | `canyin-opinion-script` |
| 拍进货、备餐、服务过程 | `canyin-process-script` |
| 做干货内容涨粉 | `canyin-knowledge-script` |
| 讲创业经历、夸员工、做店庆 | `canyin-story-script` |
| 判断这条能不能发 / 数据差在哪 | `canyin-script-selfcheck` |
| 不确定走哪个 / 想查术语原文 | `canyin-shortvideo-course`（路由） |

**`canyin-shortvideo-course` 是路由总入口**，内含 15 张能力卡的完整索引。另外 8 张补充卡（AI 出选题提示词公式、拍摄基础、剪辑工作流、自然流引导、拆片法、进阶大制作脚本、IP 问卷、矩阵团队）挂在路由下按需调用，不单独占触发位。

---

## 安装

这套 skill 用的是 **`SKILL.md` 开放标准**（[agentskills.io](https://agentskills.io)），
Codex CLI、Claude Code、Cursor、Gemini CLI 等 38+ 平台通用。只需放到对应工具的 skills 目录：

| 工具 | 安装命令（在 `dist/canyin-shortvideo-course/` 目录下执行） |
|---|---|
| **WorkBuddy** | `cp -R canyin-* ~/.workbuddy/skills/` |
| **Codex CLI** | `cp -R canyin-* ~/.codex/skills/` |
| **Claude Code** | `cp -R canyin-* ~/.claude/skills/` |
| **Cursor / 其他** | 放到该项目/工具的 skills 目录即可 |

项目级安装（团队共享）：把 `canyin-*` 放进仓库根的 `.codex/skills/` 并提交，
所有人克隆后自动生效。

```bash
git clone https://github.com/<YOUR_USERNAME>/canyin-shortvideo-skills.git
cd canyin-shortvideo-skills/dist/canyin-shortvideo-course
cp -R canyin-* ~/.workbuddy/skills/
```

重启对应工具生效。新会话中输入 `/skills` 可确认是否已加载。

---

## 用法示例

```
用 canyin-positioning，我开了一家开了 8 年的社区川菜馆，
人均 45，主要靠回头客，但年轻人越来越少，帮我找进店理由。
```

```
用 canyin-topic-generator，基于"现炒现做、不用预制菜"这个进店理由，
给我 10 个下周能拍的选题。
```

```
用 canyin-script-selfcheck，帮我看看这条脚本能不能发。
```

---

## 目录结构

```
.
├── dist/canyin-shortvideo-course/   ← 编译产物，可直接安装
│   ├── canyin-shortvideo-course/    ← 路由入口（含 15 张卡索引）
│   ├── canyin-positioning/
│   ├── canyin-topic-generator/
│   ├── canyin-opinion-script/
│   ├── canyin-process-script/
│   ├── canyin-knowledge-script/
│   ├── canyin-story-script/
│   └── canyin-script-selfcheck/
│
├── books/canyin-shortvideo-course/  ← 蒸馏全过程（源文件已排除）
│   ├── BOOK_OVERVIEW.md      整书理解（Adler 四步）
│   ├── DIGEST.md             精华长文，建议从这里读起
│   ├── GLOSSARY.md           22 条术语词典（定义取自讲师原话）
│   ├── verified.md           三重验证记录
│   ├── PIPELINE_STATE.md     流水线状态
│   ├── candidates/           187 条候选方法论
│   ├── rejected/             未晋级项与驳回理由
│   ├── tests/                触发评测用例
│   └── .cangjie/capabilities/ 15 张 RIA 能力卡 + verified.yaml
│
└── README.md
```

---

## 已知边界（重要）

这套方法论有明确适用范围，用之前请知道：

1. **绑定抖音自然流红利期**。付费流量占比上升后，"靠内容白嫖流量"的难度显著变大。
2. **讲者是卖课机构**，存在过度承诺倾向（典型如"天下没人做不成 IP"）。
3. **幸存者偏差**。课堂上展示的成功案例是筛选后的结果。
4. **工业化套路的同质化反噬**。同一套爆款元素被同行批量复用后，边际效果会下降。
5. **内容治不了产品**。如果复购和出品做不好，涨粉只会让差评传播得更快——这是原材料里刻意淡化的一面。

术语「情绪波点」「置身事外」的确切含义未能从逐字稿敲定，已在 `GLOSSARY.md` 中标注待确认并给出推测定义。
