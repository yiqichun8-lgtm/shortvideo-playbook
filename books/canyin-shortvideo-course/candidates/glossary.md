# glossary-extractor 候选输出（阶段 1）
# 书目：餐饮短视频实操课程体系
# 说明：本文件不独立成 skill，但作为所有 skill 的共享词典被引用。
# key_distinction 是最有价值的字段——它防止下游 skill 把这些词当成常识词义用。

- id: g01
  term: 进店理由 / 成交理由
  type: term
  source_chapter: "01:L41-67; 04:L173-216"
  author_definition: |
    "进店理由从三个维度寻找：产品、店铺、人。……进店理由—说 XXX 好就主要体现什么好。"
  key_distinction: |
    ≠「卖点/差异化」（那是给同行看的定位）
    ≠「广告语」（那是文案，不是理由）
    = 用户选择你而不选同行的具体、可被画面证明的原因；共 15 条封闭枚举，
      一条内容只主打一个，多条内容之间用不同组合。
  why_it_matters: |
    所有内容必须围绕某一个进店理由展开，否则内容"正确但不变现"。
    若 skill 把它理解成普通卖点，会建议用户"把卖点都罗列一遍"——这是最典型的错误用法。
  tags: [term, core, positioning]

- id: g02
  term: 水桶型漏斗
  type: term
  source_chapter: 03:L190-191
  author_definition: |
    "成交理由充足，并且都是真事儿、人家不会质疑，还老出现——OK，
    你的账号就是一个水桶型漏斗的账号了，你的流量一定会往下漏，一定会变现好。"
  key_distinction: |
    ≠「漏斗」（营销漏斗讲的是转化层级）
    = 一个判别式：成交理由充足 + 原生感 + 高频出现，三者同时成立即"定位正确"，
      流量会自然往下漏成成交。没成立之前谈技巧没有意义。
  why_it_matters: 下游 skill 判断"该不该加爆款元素"之前，先用这个判别式验收定位。
  tags: [term, positioning, diagnostics]

- id: g03
  term: 原生感 / 原生
  type: term
  source_chapter: "03:L180-186; 04:L166-170"
  author_definition: |
    "越自然越好：说人话，不夹，不装，不开美颜，不用花哨的分镜头，少用画外音。"
  key_distinction: |
    ≠「画质好」「制作精良」
    = 观众相信视频里的这个人就是生活中的这个人；
      假 = 穿不属于自己的衣服、用相机、端着说话、用不属于自己的语气。
      注意：不是粗糙，而是"人格一致"。
  why_it_matters: |
    多数拍摄/剪辑建议会本能提升制作精度，与本条冲突；
    没有这条澄清，skill 会给出"建议上稳定器和相机"这类适得其反的建议。
  tags: [term, authenticity, production]

- id: g04
  term: 三有原则
  type: term
  source_chapter: "01:L36-39; 04:L148-150"
  author_definition: |
    "内容被喜爱的三有原则：有用处、有兴趣、有共鸣。"
    有用处→教程类/推荐类；有兴趣→美好类/炫技类/恶搞类；有共鸣→情感类/励志类/吐槽类。
  key_distinction: |
    ≠「好内容」的泛泛标准
    = 选题时的三选一过滤器：一条内容必须明确命中其中至少一项，否则不进入脚本环节。
  why_it_matters: 它是选题阶段的准入闸门，不是发布后的评价标准。
  tags: [term, filter]

- id: g05
  term: 八大爆款元素
  type: term
  source_chapter: "03:L197-251; 01:L108-117"
  author_definition: |
    "成本的、人群的、奇葩的、最差的、反差的、怀旧的、荷尔蒙的、头牌的。
    一个选题加上一个爆款元素，就是爆款选题。"
  key_distinction: |
    ≠ 内容类型（它们不是赛道、不是脚本类型）
    ≠ 选题本身（它们是叠加在选题上的"调料"）
    = 八个人类共通的观看动机；行业无关，因为"火这件事跟行业没关系"。
      讲师自述：反差与对比本该是两个，为便于售卖合并成"八大"。
  why_it_matters: |
    若当成内容分类用，会出现"我做餐饮属于八大里的哪一个"的误用；
    正确用法是"每条普通选题试挂一个元素，看能否变成通顺的选题"。
  tags: [term, viral-elements, core]

- id: g06
  term: 爆款词根
  type: term
  source_chapter: 03:L204-206, L220, L238
  author_definition: |
    "（小伙伴们把这八个爆款元素拆成 30 多个词根），把这个'花小钱办大事儿'这个人类爱看的
    爆款词根往 AI 里一输就搞定了。"
  key_distinction: |
    ≠ 爆款元素（元素是八个大类）
    = 元素的具体词汇化表达，可直接套进标题：
      "花小钱办大事/最省时间/最省力气/最省钱"（成本）、
      "买完必后悔/用了必后悔/9块9/最惨的"（最差）、
      "千万不要/建议不要"（否定句式）、"20年前的/当年/经典的/古代"（怀旧）、
      "同款/名校/名企/最贵的/最有面子的"（头牌）。
  why_it_matters: |
    这是元素落到可执行层的抓手；AI 提示词、标题改写、跨行业迁移都在这个颗粒度上工作。
    注意其有效性会被耗尽（会"用烂"），需要持续更新词根库。
  tags: [term, viral-elements, heading]

- id: g07
  term: 火车节模型
  type: term
  source_chapter: "01:L233-250; 04:L337-339; 03:L633-647"
  author_definition: |
    "起因（必须加钩子）→ 关键步骤 → 转场 → 经过 → 转场 → 关键步骤 → 继续经过与转场 → 结果。
    想在火车上让人从第一节走到第五节？告诉他第五节有抽奖还有美女，他就自己抬腿跑过去了——
    这叫钩子。"
  key_distinction: |
    ≠ 一般叙事结构（起因经过结果）
    = 晒过程专用：每一节车厢之间都要有钩子驱动，关键步骤里埋入要展示的专业点，
      结果处才是客资转化点。经过控制在 1-3 个，多个经过要服务同一个钩子。
  why_it_matters: 晒过程 skill 的核心结构；缺了它，晒过程会退化成流水账 Vlog。
  tags: [term, script-structure, share-process]

- id: g08
  term: 钩子
  type: term
  source_chapter: "04:L346-359; 03:L633-647"
  author_definition: |
    "广告别生打，中间加钩子。……（钩子）第五节车厢不但有抽奖还有美女。"
  key_distinction: |
    ≠「悬念标题」
    = 让观众再走一节车厢的具体理由，可以是金钱/对抗/送温暖/验证揭秘/盲盒/荷尔蒙六类；
      出现在起因（必加）、也出现在段落之间（少而精）。
  why_it_matters: 用户常把钩子只理解为标题党，导致视频只有开头有钩子、中间塌掉。
  tags: [term, hook, share-process]

- id: g09
  term: 期待感
  type: term
  source_chapter: "01:L252-290; 03:L647"
  author_definition: |
    "（钩子）在我们的课上有三个字去总结：期待感。让观众永远充满着期待感，我就愿意看下去。"
  key_distinction: |
    ≠「氛围感」
    = 可勾选的六类钩子清单（金钱/对抗/送温暖/验证揭秘/盲盒/荷尔蒙）；
      晒过程的核心指标就是让观众从头到尾对未来有预期。
  why_it_matters: 它是"为什么这条视频能留人"的唯一解释框架，也是自检的可操作项。
  tags: [term, hook, retention]

- id: g10
  term: 桥段
  type: term
  source_chapter: "01:L396-424; 04:L401-412"
  author_definition: |
    "经典桥段：一轮困境（盲目自信/家门不幸/天灾人祸）、一轮转机（通关密码/至亲寄托/贵人相助/
    天赋异禀/意外之喜）、二轮困境（恶霸欺压/过河拆桥/至亲背叛/强权干涉）、
    二轮转机（因祸得福/贵人相助/破釜沉舟）。……创新都来自元素的重新排列组合。"
  key_distinction: |
    ≠「剧情桥段」的泛称
    = 固定的、可枚举的叙事单元库；创作动作是"识别 → 重新排列组合"，
      不是"发明新故事"。成功案例型中"贵人"必须是讲述者本人。
  why_it_matters: 没有这个概念，讲故事 skill 会建议用户"去想一个感人的故事"，无法执行。
  tags: [term, storytelling, library]

- id: g11
  term: 情绪曲线 / 难点升级
  type: term
  source_chapter: "04:L401-412; 01:L396-410"
  author_definition: |
    "2、一轮困境（背景简单带入，快进主题）；4、二轮困境（二轮痛点要高于一轮）；
    5、二轮转机（二轮爽点要高于一轮）。"
  key_distinction: |
    ≠「要有情绪起伏」
    = 可量化规则：第二轮的痛点和爽点必须高于第一轮，否则情绪曲线走平。
  why_it_matters: 给"故事好不好看"提供了唯一可验证的判据。
  tags: [term, storytelling, rule]

- id: g12
  term: 六论据
  type: term
  source_chapter: "01:L192-199; 03:L404-446"
  author_definition: |
    "权衡利弊（不这么做会失去什么，这么做会得到什么）、无奈之举（该懂的该做的都尽力了，
    但我没有办法）、不同视角（当事人怎么想、旁观者怎么想）、维度升级（从历史时间线或
    未来社会影响看问题）、人身攻击（对当事人的外貌、品行或智力评头论足）、
    倒打一耙（不讨论实际事实，只抒发心情）。"
  key_distinction: |
    ≠「论据」（一般意义上的证明材料）
    = 六种固定的说服路径（零件库），一个视频通常只用一个，长文案可用两个；
      常用组合是权衡利弊 + 维度升级。底层心法：给观众"想做但不好意思做的事"找理由，
      给"不想做或没做成的事"找借口。
  why_it_matters: |
    观点类 skill 的核心零件表；澄清"倒打一耙"的确切含义可解决知识体系文档里的「待确认」项。
  tags: [term, argument, opinion]

- id: g13
  term: 质检员还是销售员
  type: term
  source_chapter: "01:L301-305; 04:L350"
  author_definition: |
    "讲述者是'质检员'还是'销售员'？（自检问题）"
  key_distinction: |
    ≠ 一个职位
    = 晒过程时的讲述姿态自检：你是在中立地展示/检验这个过程（质检员），
      还是在推销（销售员）。前者留人且不引起防备，后者观众立刻关闭。
  why_it_matters: 用角色隐喻做语气自检，非常低成本且高频有效。
  tags: [term, self-check, share-process]

- id: g14
  term: 获得感
  type: term
  source_chapter: "01:L338-343; 04:L309-312"
  author_definition: |
    "推荐内容的获得感标准：效果好、料够猛、信息多。"
  key_distinction: |
    ≠「有价值」的笼统评价
    = 三条可对照的自检项：解法见效快/反馈周期短/行动成本低，
      内容密度高（一次给到 5-8 条）。
  why_it_matters: 教知识类内容的准入门槛；不满足就重新做信息密度。
  tags: [term, teach-knowledge, quality]

- id: g15
  term: 情绪波点
  type: term
  source_chapter: "01:L120-125; 04:L237"
  author_definition: |
    "四种内容与四类心智动作对应：讲故事→回忆，晒过程→行动，教知识→分析，
    聊观点→情绪波动（另有'情绪波点'的写法）。"
  key_distinction: |
    ⚠ 该术语在来源文档中标注「待确认」。在逐字稿语境中它指的不是 generic 的"情绪起伏"，
    而是**观点类内容天然自带跳转到另一个人的立场/情绪上去的能力**
    ——这就是为什么写观点前必须先决定"替谁说话"。
    建议下游 skill 保留原词但在卡片中给出上述工作定义，并标注不确定性。
  why_it_matters: 不澄清会导致"四类心智动作"框架在观点项上出现语义空洞。
  tags: [term, uncertain, to-confirm]

- id: g16
  term: 置身事外
  type: term
  source_chapter: "01:L243-250（火车节模型操作步骤最后一步）"
  author_definition: |
    "（火车节模型操作）：确认要晒什么 → 预描场景，联想画面 → 聚焦关键环节 →
    展示专业点 → 补充关键步骤中可能出现的事件细节 → 提炼'火车节' → 置身事外（具体操作含义待确认）。"
  key_distinction: |
    ⚠ 文档已标注「待确认」。结合课程整体逻辑，最可能的所指是：
    从"我在做事"切换到"我在讲述/审视这件事"的视角——即留出解说者位，
    以便给各个环节加钩子。但该解释未被原文证实，**skill 中应标注为推测**。
  why_it_matters: 该步骤缺具体操作定义，误用会让用户卡在最后一步。
  tags: [term, uncertain, to-confirm]

- id: g17
  term: 均播时长 / 完播时长
  type: term
  source_chapter: 03:L628-630
  author_definition: |
    "我们怎么判断一个视频好不好呢？大家记住这个事儿：完播时长，并不是点赞数。
    在你们的后台可以看到一个均播的时长，均播时长拉的越高……进入你的直播间看你的视频更有耐心听成交。"
  key_distinction: |
    ≠ 完播率百分比（很多教程把它当成核心指标）
    = 后台的"平均播放时长"绝对值；它决定粉丝对你的耐心额度，决定直播间成交能力。
  why_it_matters: |
    这一条直接推翻常见的"短视频要短"建议，是中长视频策略的判据来源。
  tags: [term, distribution, metric]

- id: g18
  term: 矩阵
  type: term
  source_chapter: "02:L21-40"
  author_definition: |
    "矩阵的意义呢，其实是从粉丝经济到品牌经济一个过渡……可不是多赚点儿钱的事儿。"
  key_distinction: |
    ≠「多开几个号多份收益」
    = 让多个 IP 的学员/观众反复看到同一个品牌名，形成品牌资产沉淀。
  why_it_matters: 误解会造成"为了多赚点钱盲目开号"，反而在品牌层面失效。
  tags: [term, team, lower-priority]

- id: g19
  term: 拆片
  type: term
  source_chapter: "04:L552-581; 02:L284-287"
  author_definition: |
    "（拆片万能表）内容类型/脚本结构/拍摄角度/出镜人物/呈现形式/出场方式/剪辑方式。"
  key_distinction: |
    ≠「拉片」（逐秒描述画面，课程中明确否定了这种做法：
      "他把一个片子拆成第一秒是什么、第二秒是什么……那我用它干嘛呀？"）
    = 输出"这条为什么火 + 我怎么借鉴"的结构化分析。
  why_it_matters: 明确区分可避免 AI 拆片/人工拆片产出无效流水账。
  tags: [term, analysis, definition-matters]

- id: g20
  term: 散弹枪原理
  type: term
  source_chapter: 04:L267-269
  author_definition: |
    "散弹枪原理：扩大流量。普通选题 + 明星/名企/名人/名校 = 爆款选题。"
  key_distinction: |
    ≠ 泛泛地"蹭热点"
    = 借一个更大的已知载体来突破本行业流量池的具体加法操作，是"头牌"元素的别名用法。
  why_it_matters: 提供了"怎么把普通选题变大"的最简单公式。
  tags: [term, viral-elements, method]

- id: g21
  term: 自然流
  type: term
  source_chapter: "04:L510-535"
  author_definition: |
    "（第三周课程）前期破冰/中期引导/后期鼓励……让IP拍摄更自然的好处：老板喜欢+流量大。"
  key_distinction: |
    ≠「自然流量」（区别于付费流量的那个"自然流量"）
    = 一种拍摄方式：不背稿、现场提问引导、当场出情绪，成片显得没被设计过。
    这是本课程体系里最容易被混淆的术语之一。
  why_it_matters: |
    混淆两个含义会导致 skill 在"要不要投流"的问题上错误触发这套拍摄方法。
  tags: [term, production, confusion-prone]

- id: g22
  term: 英雄时刻
  type: term
  source_chapter: "01:L439-447; 04:L417-419"
  author_definition: |
    "平凡英雄的英雄时刻：自己解决问题、敢作敢当、随手帮助、坚守原则、仗义扶弱、
    积极面对、及时回怼。"
  key_distinction: |
    ≠「高光时刻」（那是结果）
    = 七种可被识别的高光行为类型，用于在素材里标记"这里是不是英雄时刻"。
  why_it_matters: 平凡英雄型脚本的唯一难点是"从平淡素材里认出英雄时刻"，需要枚举库。
  tags: [term, storytelling, library]
