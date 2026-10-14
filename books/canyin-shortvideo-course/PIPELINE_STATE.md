# PIPELINE_STATE — canyin-shortvideo-course

- **slug**: canyin-shortvideo-course
- **源材料**: 6 个文件（2 份逐字稿 + 知识体系 docx + 编导思维导图 pdf + 2 个 xlsx 模板），文本已提取至 `source/`（共 34.2 万字符）
- **输出模式**: **pack**（用户显式选择）。1 个来源路由入口 + 7 个晋级 Skill = 8 个可发现入口
- **用户选型**: 老板视角、策划与脚本为主；自用蒸馏，不署名

## 阶段进度

| 阶段 | 状态 | 备注 |
|---|---|---|
| 0 整书理解 | ✅ 完成 | BOOK_OVERVIEW.md（用户已确认骨架） |
| 1 并行提取 | ✅ 完成 | 187 条候选：frameworks 53 / principles 62 / cases 28 / counter-examples 22 / glossary 22 |
| 1.5 三重验证 | ✅ 完成 | verified.md：15 个能力单元全部通过；rejected/rejected-summary.md |
| 1.6 晋级门 | ✅ 完成 | 7 promoted（U01–U07）+ 8 router（U08–U15），入口数 8 = 软预算上限 |
| 2 RIA++ 能力卡 | ✅ 完成 | cards/ 下 15 张卡（R/I/A1/A2/E/B 六段齐全） |
| 3 Zettelkasten 链接 | ✅ 完成 | verified.yaml 的 also_read + GLOSSARY.md（22 条术语） |
| 4 压力测试 | ✅ 完成 | tests/test-prompts.json（每晋级 Skill 3+2+1，darwin 兼容） |
| 5 编译与交付 | ✅ 完成 | 编译至 dist/canyin-shortvideo-course，validate 0 errors / 0 warnings；已安装到 ~/.workbuddy/skills/；DIGEST.md 约 1.4 万字符 |

## 执行过程中的偏离（审计留痕）

1. **阶段 1 降级为串行**：5 个并行 sub-agent 全部返回 429（使用量限额，23:15 UTC+8 重置）。
   - framework-extractor 与 principle-extractor 在被中断前已各自写出完整候选文件（53 + 62 条），予以采纳；
   - cases / counter-examples / glossary 三份由主编我自己按对应 extractor prompt 补齐。
   - 影响： case / counter-example / glossary 三类的覆盖率依赖检索式取块（Grep + 定向窗口读取），
     未做全量逐行扫描，存在少量证据遗漏的可能（如 02 逐字稿只做了部分采样）。
     若需补漏，可在配额恢复后重跑这三个 extractor 做增补（不改写既有 slot）。
2. **traceability 修正**：写卡过程中发现若干引文失真，已逐条回原文用行号核对并修正。
3. **范围裁剪**：编导求职面试框架（04:L751-831）不属于老板视角，未进入 Bundle（记录在 rejected-summary 第三节）。

## 后续可做

- 配额恢复后，串行重跑 case / counter-example / glossary extractor 增补遗漏；
- 用 darwin-skill 接入 tests/test-prompts.json 做触发进化；
- 若将来想换形态：`python3 scripts/cangjie.py replan-output --dry-run`。
