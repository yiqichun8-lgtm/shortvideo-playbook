# counter-example-extractor 候选输出（阶段 1）
# 书目：餐饮短视频实操课程体系
# 说明：本类产出是阶段 2 的 Boundary (B) 段核心素材——没有反例，skill 就没有边界。

- id: ce01
  title: 专业团队 + 200 万投资 + 无明确产品 → 赔光
  type: counter-example
  source_chapter: 03:L5-11
  source_quote: |
    "a 那个老板他在想的问题是：我请的运营也挺专业的，我请的主播也不是外行，
    怎么 200 万就赔光了呢？……200 万人民币在短视频行业里根本就不叫钱。"
  failure_mode: |
    先搭团队、备货盘、投钱，再想"我们做什么内容"——把顺序倒过来，
    结果是有播放、无人格、无产品、无成交。
  mechanism: |
    短视频变现的第一驱动是"这个人可信且他的东西有用"，不是制作资源。
    钱能买到设备和运营，买不到已经存在的信任关系和成交理由。
  warning_signs:
    - 先把团队/直播间搭起来才讨论卖什么
    - 拿"我要规划一个商业盘"当开场白
    - 半年之内必然赚不到钱，尤其在大城市被各类"商业盘"提案消耗
  bound_to:
    - "商业定位前置"
    - "小而专优先"
    - "四种变现方式筛选"
  tags: [counter-example, positioning, money]

- id: ce02
  title: 外包孵化/代运营：花大钱找人做号
  type: counter-example
  source_chapter: 03:L10-11
  source_quote: |
    "他在某人那儿交了200万的孵化费，给他做了1300个粉丝……他把钱退回来，真退回100万。"
  failure_mode: |
    把"做IP"当成可外包的服务采购，账号起来了也黏在代运营身上，自己不会也不会获得客资。
  mechanism: |
    代运营只对"交付内容条数"负责，不对"是否成交"负责；IP 的人格不可能由第三人代理。
  warning_signs:
    - 对方承诺代运营全程托管
    - 合同指标是"发布条数/涨粉数"而不是咨询量/成交
    - 收费高到超出单条内容试错成本几十倍
  bound_to:
    - "商业定位前置"
    - "原生感（自己出镜）"
  tags: [counter-example, outsourcing, money]

- id: ce03
  title: 被包装成"假人"：西装 + 相机 + 端庄 = 有流量不变现
  type: counter-example
  source_chapter: 03:L182-186
  source_quote: |
    "我见过最多的被代运营公司坑的就是这个点：穿西服、上相机、端庄一点，拍出来的视频是个假人儿……
    好所以为什么有的老师出镜很端庄、变现还好？因为人家生活中就端庄。你一个干粗活的，你装什么呀？"
  failure_mode: |
    用不属于自己的人设和器材去"提升质感"，观众说不出哪里假但本能不信，最终账号不变现。
  mechanism: |
    观众的识别系统对"人格一致性"极敏感；一旦识别为表演，内容中的成交理由自动失效。
  warning_signs:
    - 买了相机/补光灯才敢开拍
    - 出镜前换上平时不穿的衣服
    - 开美颜、端着说话、用不属于自己的口音
  bound_to:
    - "原生感原则"
    - "不用相机/不用美颜"
  tags: [counter-example, authenticity, conversion]

- id: ce04
  title: "硬装"有技巧有流量但骗不过观众
  type: counter-example
  source_chapter: 03:L186
  source_quote: |
    "大家别硬装，你一硬装吧，有可能有技巧有流量，但是大家能看出来你是假的，你的账号变现就不好。"
  failure_mode: 把人格当成道具，短期数据好看，长期转化归零。
  mechanism: 内容与本人错位，成交所需的信任无法累积。
  warning_signs:
    - 视频里的人"朋友认不出来"
    - 线下见到本人与视频判若两人
  bound_to:
    - "原生感原则"
  tags: [counter-example, authenticity]

- id: ce05
  title: 本地号一开头就报地名，把流量锁死在本地
  type: counter-example
  source_chapter: 03:L380-382
  source_quote: |
    "我看过很多连麦的人，他们今天教一个知识或者表达一个观点，非要在这个视频开头加一个在哪儿哪儿的人……
    你加上地区，你流量就跑不出去。"
  failure_mode: |
    每条视频开头加"沈阳的注意了"，把本来全网可用的选题限制在本地流量池，播放量天花板骤降。
  mechanism: |
    人群选题（不要跟公婆住）本可跑百万流量，本地人自然也在其中；
    加了地域词就先放弃了 95% 的池子。
  warning_signs:
    - 每条视频开头必报城市
    - 认为"泛流量没用，我要精准"
  bound_to:
    - "人群选题 vs 行业选题的双轨策略"
    - "本地餐饮账号尤其危险"
  tags: [counter-example, traffic, local-business]

- id: ce06
  title: 生打广告没人看
  type: counter-example
  source_chapter: 03:L642-647
  source_quote: |
    "（那条视频）广告打了好多……但如果这样的广告我们生拍就没人看。我们不愿看这样的广告。
    广告别生打，中间加钩子。"
  failure_mode: |
    把产品/卖点直接铺陈出来当拍摄对象，用户秒划走。
  mechanism: |
    用户来满足的是期待感，不是购买需求；没有钩子就没有停留，没有停留就到不了广告点。
  warning_signs:
    - 脚本里全是"我们的产品/我们的服务"
    - 前三秒没有任何悬念或冲突
  bound_to:
    - "火车节模型"
    - "期待感六技巧"
    - "广告-钩子交替节奏"
  tags: [counter-example, hook, share-process]

- id: ce07
  title: 迷信"短视频必须 7 秒/15 秒"
  type: counter-example
  source_chapter: 03:L627-630
  source_quote: |
    "大家肯定听说过什么七秒、15秒、视频不能特别长……千万不要做15秒七秒，
    你能帮平台留住的客户时间就那么点儿。"
  failure_mode: |
    为了短而删掉过程中最能建立信任的细节，导致均播时长低、粉丝耐心低、进直播间不下单。
  mechanism: |
    平台按"帮它留住用户时间"分配流量，判断标准是均播时长而不是点赞数。
  warning_signs:
    - 用"完播率"而不是"均播时长"判断好坏
    - 为了时长把关键步骤剪掉
  bound_to:
    - "留存优先的中长视频策略"
    - "晒过程要拍长"
  tags: [counter-example, distribution, editing]

- id: ce08
  title: 讲原理没流量，只该讲操作步骤
  type: counter-example
  source_chapter: 03:L615-616
  source_quote: |
    "同样是干减肥的，他俩的播放量、点赞量差这么多——就是你不需要讲知识的原理，
    你只需要直接告诉大家怎么操作就可以了。"
  failure_mode: |
    从概念、原理、分类讲起，把观众当学生而不是"累了一天想休息的人"。
  mechanism: |
    刷视频的用户心智是"把抖音所有粉丝当成小宝宝，简单耐心地告诉他怎么做"。
  warning_signs:
    - 开头是"什么是 XX""XX 的三种原理"
    - 观众需要记住前置概念才能听懂后面
  bound_to:
    - "教知识四型"
    - "获得感三标准"
  tags: [counter-example, teach-knowledge, copywriting]

- id: ce09
  title: 只搜一个平台就开拍 → 内容同质没流量
  type: counter-example
  source_chapter: 03:L548
  source_quote: |
    "今天有一个选题，搜了抖音或者视频号，搜完以后直接用——那这种他肯定没有流量。
    大家就是多搜几个，好的变成自己的。"
  failure_mode: 单平台取材，全网搬运同一套信息，自己的内容没有增量。
  mechanism: 观众已经刷过同样的信息；没有跨源整合就没有"信息多"的获得感。
  warning_signs:
    - 素材全部来自同一个搜索框
    - 内容能被任何同行一字不差复述
  bound_to:
    - "同行评论区 + 多平台素材库挖掘法"
    - "获得感三标准"
  tags: [counter-example, source-mining, knowledge]

- id: ce10
  title: 拍摄现场五不做（毁 IP 情绪）
  type: counter-example
  source_chapter: 04:L516-522
  source_quote: |
    "1、批评IP情绪状态不对；2、要求IP完全背稿；3、打断IP说话；4、和IP说刚才那段没录上；
    5、拍摄说悄悄话。"
  failure_mode: |
    用管理演员的方式管理老板/IP，导致 IP 越拍越僵、越来越不说人话，最终放弃出镜。
  mechanism: |
    非职业 IP 的表现力来自松弛感，批评和背稿直接摧毁松弛感；谎称没录上是欺骗，会摧毁信任。
  warning_signs:
    - 现场说"你刚才情绪不对，重来"
    - 递提词器要求照读
  bound_to:
    - "自然流现场引导法"
    - "拍完必夸奖"
  tags: [counter-example, directing, execution]

- id: ce11
  title: 提问四禁忌（见面就开大/人形读稿器/杠精式提问/想起来就问）
  type: counter-example
  source_chapter: 04:L532-535
  source_quote: |
    "提问禁忌：见面就开大、人形读稿器、杠精讨厌鬼、想起来就问。"
  failure_mode: |
    采访式拍摄时提问方式不对，IP 的回答变成干瘪的事实描述，出不来故事和情绪。
  mechanism: |
    缺乏场域搭建（了解 IP 本人/行业）就提问，问题不在 IP 的表达舒适区。
  warning_signs:
    - 第一个问题就问最痛的经历
    - 照着提纲逐条念
  bound_to:
    - "自然流现场引导法"
    - "IP 定位信息采集框架"
  tags: [counter-example, directing, execution]

- id: ce12
  title: 拍摄构图七禁忌
  type: counter-example
  source_chapter: 04:L124-127
  source_quote: |
    "拍摄禁忌：面壁思过/顶天立地/脑袋悬浮/断手断脚/移花接木/东倒西歪/喧宾夺主。"
  failure_mode: |
    画面问题让观众本能不舒服直接划走，与技术水平无关，纯粹是物理失误。
  mechanism: |
    人眼对头顶尖物、切断关节、背景杂乱、主体被陪体压制极其敏感。
  warning_signs:
    - 头顶出现横梁/柜角
    - 人物紧贴画面边缘留出大片空墙
    - 裁切在手腕/脚踝
  bound_to:
    - "拍摄呈现场域构建"
    - "拒绝素背景"
  tags: [counter-example, shooting, execution]

- id: ce13
  title: 剪辑五错：吞字 / 系统字 / 白字无阴影 / 花哨特效 / 多用贴纸
  type: counter-example
  source_chapter: 04:L31-78
  source_quote: |
    "不要吞字❗❗❗❗❗❗ 字体：不要用系统字。用白色字体时记得加阴影。……贴纸只有四种可用，
    其余不要乱加。……（精剪切勿花哨）"
  failure_mode: |
    字幕识别后直接裁切气口导致吞字；用系统字体、纯白无阴影字让画面廉价；
    特效贴纸堆砌让视频变成 PPT。
  mechanism: |
    观感成本：任何一个"廉价感细节"都会拉低整条视频的可信度，进而影响变现。
  warning_signs:
    - 剪完没试听一遍就导出
    - 用默认字体和默认花字模板
  bound_to:
    - "剪辑十步工作流"
    - "封面五规则"
  tags: [counter-example, editing, execution]

- id: ce14
  title: 荷尔蒙元素的账号安全风险
  type: counter-example
  source_chapter: 02:L628-629; 04:L365-367
  source_quote: |
    "发了账号封了……抖音它是个公域流量，他怕那些有那个坏人啊，真的会去找你啊。"
  failure_mode: |
    为了钩子使用擦边/性暗示元素，轻则限流重则封号；
    素材里列举的黑丝/大胸/搭讪/变装等在当下平台治理中已是高危项。
  mechanism: |
    平台对荷尔蒙类内容的判定不区分"你的动机"，只看画面与措辞是否触发模型。
  warning_signs:
    - 靠身材/穿着/暧昧关系做钩子
    - 封面靠露肤吸引点击
  bound_to:
    - "八大爆款元素·荷尔蒙"
    - "期待感六技巧"
  tags: [counter-example, platform-risk, viral-element]

- id: ce15
  title: 帮助弱者视频一看镜头就假
  type: counter-example
  source_chapter: 02:L1035-1037
  source_quote: |
    "你在真的帮这个人的时候，你不要去看镜头……讲他苦难的时候，你也正常跟人聊天，
    也不要看镜头，你只有最后有感悟了，你才可以出镜。"
  failure_mode: |
    一边做好事一边对着镜头解说，观众立刻判断为摆拍，善意内容反噬人设。
  mechanism: |
    助人场景的真实性靠"忘记镜头存在"来证明，这是唯一无法表演的部分。
  warning_signs:
    - 帮助过程中有旁白
    - 受访者在被帮助时明显对着镜头
  bound_to:
    - "帮助弱者型脚本"
    - "原生感原则"
  tags: [counter-example, authenticity, advanced-script]

- id: ce16
  title: 揭秘的越界：别把自己送进去
  type: counter-example
  source_chapter: 03:L560, L578-580
  source_quote: |
    "（揭秘）打开给大家看一看……你们揭秘就别影响自己生命就行了，
    别报完以后，你要么进去了，要么有人咋地你的就行。"
  failure_mode: |
    揭秘到自己参与过的灰色环节，或曝光具体到可被追溯的第三方利益链条。
  mechanism: |
    流量收益是一次性的，法律/人身风险是长期的；餐饮业尤其涉及供应链与同行关系。
  warning_signs:
    - 素材涉及自己参与的黑产/违规操作
    - 点名到具体厂商、配送商、同行姓名
  bound_to:
    - "教知识四型·揭秘型"
    - "揭秘的边界"
  tags: [counter-example, legal-risk, teach-knowledge]

- id: ce17
  title: 词根会被用烂——同质化反噬
  type: counter-example
  source_chapter: 03:L254
  source_quote: |
    "有的同学会说：'老师，如果有一天"如何贪小便宜"这个词根被用烂了'……"
  failure_mode: |
    全行业都在用同一批词根（买完必后悔/千万别/觉醒），用户对套路免疫，点击率下滑。
  mechanism: |
    爆款元素之所以有效是因为它稀缺，一旦成为行业默认语法，情绪唤起失效。
  warning_signs:
    - 打开同城同赛道，三家在用同一个句式
    - 自己看到这个词根已经不想点
  bound_to:
    - "八大爆款元素"
    - "爆款词根"
    - "快速出选题六技巧"
  tags: [counter-example, viral-element, saturation]

- id: ce18
  title: AI 开着推理功能 → 输出失控
  type: counter-example
  source_chapter: 03:L193-195
  source_quote: |
    "我们用 DeepSeek 会出问题，你们就把（推理）关了……用他的推理都会觉得他乱推理，
    答案非常的非、非常的不可控。"
  failure_mode: |
    用推理模型跑已经写清楚的指令，AI 脑补背景，产出似是而非的选题和不实的数据。
  mechanism: |
    指令足够具体时不需要推理；推理会在信息不足处自行补全，产生幻觉。
  warning_signs:
    - 提示词里身份/人群/预算写得很清楚却仍然开着深度推理
    - AI 给出的知识性内容无法验证
  bound_to:
    - "AI 出选题/写文案 prompt 公式"
    - "教知识的事实核查"
  tags: [counter-example, ai-workflow, quality]

- id: ce19
  title: 常犯的三个脚本错误：反馈过长、排列不好、对象模糊
  type: counter-example
  source_chapter: 04:L323-329
  source_quote: |
    "脚本自检：反馈过长，排列不好，对象模糊。"
  failure_mode: |
    教知识视频给出周期很长的方案（反馈过长）、信息没有排序（排列不好）、
    说不清这条拍给谁看（对象模糊），三者任一都会让用户放弃学习。
  mechanism: |
    短视频知识产品的价值 = 见效快 × 易学会 × 对"我"有用；三条都在破坏这个乘法。
  warning_signs:
    - "坚持三个月你就会看到变化"
    - 一条视频塞进五个平行知识点
    - 说不出"这条是拍给準備/已经在 XX 的人看的"
  bound_to:
    - "教知识四型"
    - "获得感三标准"
    - "对象明确"
  tags: [counter-example, teach-knowledge, self-check]

- id: ce20
  title: 出不来选题时不搭素材库，靠灵感硬憋
  type: counter-example
  source_chapter: 04:L182
  source_quote: |
    "（出选题）出不来选题！要搭建素材库！"
  failure_mode: |
    每次拍之前临时想选题，导致更新断更、内容质量波动，无法高频。
  mechanism: |
    高频的前提是选题的工业化供应；灵感驱动的产能不足以支撑"天天出现"。
  warning_signs:
    - 打开手机才想今天拍什么
    - 一周更新低于 3 条
  bound_to:
    - "高频原则"
    - "素材库检索法"
  tags: [counter-example, workflow, source-mining]

- id: ce21
  title: 过度培养主播/达人，90% 会跑
  type: counter-example
  source_chapter: 03:L234-237
  source_quote: |
    "老板应该培养主播，还是招一个？……培养起来的概率非常低，而且培养起来90%都是跑。"
  failure_mode: |
    投入资源从零培养素人主播，成材率低且成材后流失率高。
  mechanism: |
    行业内部攀比与信息透明，能力具备后收益预期立刻抬高，人情约束弱于市场报价。
  warning_signs:
    - 以"我培养了你"作为留人理由
    - 薪酬显著低于同水平同行
  bound_to:
    - "矩阵与团队搭建"
  tags: [counter-example, team, lower-priority]

- id: ce22
  title: 分钱机制照搬别的行业
  type: counter-example
  source_chapter: 02:L40-60
  source_quote: |
    "这个分钱机制呢，不能套到大家的行业里，每个行业的利润环节不一样，
    导致每个行业那个分钱机制都不一样。"
  failure_mode: |
    直接照搬讲师所在行业（培训/流量）的分钱比例，导致激励错位、团队崩盘。
  mechanism: |
    分成结构必须匹配本行业的毛利结构和利润归属环节。
  warning_signs:
    - 直接问"你们公司怎么分的"准备照抄
  bound_to:
    - "矩阵与团队搭建"
  tags: [counter-example, team, lower-priority]
