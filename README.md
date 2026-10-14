# 实体生意短视频实操方法论 · Skill 包

把一套面向实体生意经营者的短视频方法论，体系化成 **8 个可直接安装调用的 skill 入口**，覆盖「定位 → 选题 → 脚本 → 自检」全链路。

> **方法论归属**：本仓库由易拿冠持续实践、整理与维护，面向有实体生意的经营者公开使用。
> 本仓库仅包含可执行的方法论、案例与 Skill 产物，不包含未公开的访谈和内部记录。

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

### WorkBuddy 可直接导入版

下载 [shortvideo-playbook-workbuddy.zip](https://gitee.com/yngyng666888/shortvideo-playbook/raw/main/releases/shortvideo-playbook-workbuddy.zip)，在 WorkBuddy 电脑端进入「专家 · Skills · Connectors → Skills → 添加 Skill」，直接上传该 ZIP。

> ZIP 根目录已直接放置 `SKILL.md`，并内含 15 张能力卡。不要解压后重新压缩。手机端如果没有「添加 Skill / 上传 ZIP」入口，需先在电脑端安装；单纯把 GitHub/Gitee 仓库链接发给对话窗口，不会自动安装。

### 完整 8 入口版

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
│   ├── tests/                触发评测用例
│   └── .cangjie/capabilities/ 15 张能力卡 + 清单（可重新编译）
│
└── README.md
```

---

## 让它真正为实体生意工作

这不是一套只追求播放量的内容模板，而是一套把经营优势转成短视频证据的工作方法：

1. **经营目标优先**：用有效咨询、到店、成交与复购验收，不被单一播放量带偏。
2. **真实证据优先**：产品、服务、流程、案例和客户反馈是内容的核心素材。
3. **自有表达优先**：结构可以复用，但人物、语气、细节和证据必须来自自己的生意。
4. **连续迭代优先**：根据品类、客单价、地域与客户阶段复盘，沉淀自己的有效选题和表达。

每张能力卡都保留必要的使用边界，用于保护账号、品牌、客户隐私和交付质量。
