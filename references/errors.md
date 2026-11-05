# 故障百科索引

适用场景：智能体人设 Prompt 上线后行为、格式、知识、工具、语音、载体各类故障的现象速查。共 221 条，按现象查编号，进对应分册看原因和解法。

---

## 分册

| 编号 | 分册 | 条数 | 覆盖现象 |
| --- | --- | --- | --- |
| 1–42 | [人设结构与迭代](errors/01-structure.md) | 42 | 骨架块缺失、块边界错位、简化砍错层、客户否定的迭代失控 |
| 43–59 | [输出格式](errors/02-format.md) | 17 | Markdown 符号外泄、数字列表被误断句、字数与首句失效 |
| 60–75 | [模型行为](errors/03-behavior.md) | 16 | 反复反问、话术复读、暴露配置、拒答泛滥、跨场景污染 |
| 76–99 | [知识库配合](errors/04-knowledge.md) | 24 | 召不回来、知识内嵌超限、名称外泄、图片链接错配 |
| 100–108 | [幻觉压制](errors/05-hallucination.md) | 9 | 杜撰科室医生电话、不确定就编、兜底话术不触发 |
| 109–121 | [多轮与场景](errors/06-multiturn.md) | 13 | 流程回不去、话题跳转丢失、场景污染、记忆边界失控 |
| 122–139 | [工具调用](errors/07-tool.md) | 18 | 该调不调、乱调、调用代码上屏、结果原样吐给用户 |
| 140–149 | [语音与多语言](errors/08-voice.md) | 10 | ASR 同音误识别、专有名词听错、播报标点错、语种切换失败 |
| 150–166 | [跨载体改写](errors/09-carrier.md) | 17 | 载体不匹配、字数与载体冲突、动作指令污染、能力承诺越界 |
| 167–201 | [行业场景](errors/10-scene-b2b.md) | 35 | 金融医疗政务文旅零售能源红线、行业话术错配、知识口径不一 |
| 202–221 | [机器人角色](errors/11-scene-robot.md) | 20 | 形象角色人设崩坏、动作指令不生效、移动能力乱承诺、亲和度失衡 |

## 按现象速查

| 你看到的现象 | 编号 | 分册 |
| --- | --- | --- |
| 回复仍偏正式，字数限制形同虚设 | 1 | [人设结构与迭代](errors/01-structure.md) |
| 一次性抛出全部问题，多轮访谈无法推进 | 2 | [人设结构与迭代](errors/01-structure.md) |
| 宽泛问题触发知识库全量召回，回复极其啰嗦 | 3 | [人设结构与迭代](errors/01-structure.md) |
| Few-Shot 示例与回复规范自相矛盾 | 4 | [人设结构与迭代](errors/01-structure.md) |
| Prompt 内的动作指令导致回复夹杂括号动作描写 | 5 | [人设结构与迭代](errors/01-structure.md) |
| 模型模仿 Prompt 里的井号，回复里吐出 # 号 | 6 | [人设结构与迭代](errors/01-structure.md) |
| 同一技能名高频重复，形成注意力黑洞 | 7 | [人设结构与迭代](errors/01-structure.md) |
| 交互策略示例与知识库唯一性冲突 | 8 | [人设结构与迭代](errors/01-structure.md) |
| 禁止项分散在多块，约束权重被稀释 | 9 | [人设结构与迭代](errors/01-structure.md) |
| 块内序号重号，降低指令执行精度 | 10 | [人设结构与迭代](errors/01-structure.md) |
| 角色名称在正文与限制段混用 | 11 | [人设结构与迭代](errors/01-structure.md) |
| 把比喻当成身份写进核心定位 | 12 | [人设结构与迭代](errors/01-structure.md) |
| 知识库全文塞进技能块，一次背完全部流程 | 13 | [人设结构与迭代](errors/01-structure.md) |
| 简化版未删干净原场景限定，残留逻辑持续触发 | 14 | [人设结构与迭代](errors/01-structure.md) |
| 大屏数字人吐出系统标签与引用角标 | 15 | [人设结构与迭代](errors/01-structure.md) |
| 政务类人设自行输出网址链接 | 16 | [人设结构与迭代](errors/01-structure.md) |
| 人设性别与形象发生漂移 | 17 | [人设结构与迭代](errors/01-structure.md) |
| 闲聊态与业务态共用同一字数上限 | 18 | [人设结构与迭代](errors/01-structure.md) |
| 把"简化一下"理解成推倒重写 | 19 | [人设结构与迭代](errors/01-structure.md) |
| 一次改多层，客户无法判断哪里生效 | 20 | [人设结构与迭代](errors/01-structure.md) |
| 字数限制写了但不生效 | 21 | [人设结构与迭代](errors/01-structure.md) |
| 抽象人设标签撑不起真人感 | 22 | [人设结构与迭代](errors/01-structure.md) |
| 人设里的性别被默认解读 | 23 | [人设结构与迭代](errors/01-structure.md) |
| 角色名在示例里串名 | 24 | [人设结构与迭代](errors/01-structure.md) |
| 业务场景迁移后旧客户痕迹残留 | 25 | [人设结构与迭代](errors/01-structure.md) |
| 换城市换展会时漏改兜底入口 | 26 | [人设结构与迭代](errors/01-structure.md) |
| 技能关键词密度过高，导致全局乱触发 | 27 | [人设结构与迭代](errors/01-structure.md) |
| 模型吐出 Markdown 符号 | 28 | [人设结构与迭代](errors/01-structure.md) |
| 模型输出括号动作描写 | 29 | [人设结构与迭代](errors/01-structure.md) |
| 模型自行吐出网址 | 30 | [人设结构与迭代](errors/01-structure.md) |
| 后台系统标签穿帮 | 31 | [人设结构与迭代](errors/01-structure.md) |
| 一次性把所有情况全吐出来 | 32 | [人设结构与迭代](errors/01-structure.md) |
| 流程型人设不按提纲一步步问 | 33 | [人设结构与迭代](errors/01-structure.md) |
| 多场景人设切岗后现场冷场 | 34 | [人设结构与迭代](errors/01-structure.md) |
| 闲聊态啰嗦，业务态被误压短 | 35 | [人设结构与迭代](errors/01-structure.md) |
| 白名单被 ASR 同音字击穿 | 36 | [人设结构与迭代](errors/01-structure.md) |
| 调工作流时大屏静默或过渡词复读 | 37 | [人设结构与迭代](errors/01-structure.md) |
| 新增需求与既有红线正面冲突 | 38 | [人设结构与迭代](errors/01-structure.md) |
| 只改 Prompt 不改 RAG，二维码弹不出来 | 39 | [人设结构与迭代](errors/01-structure.md) |
| Prompt 内部数量与序号自相矛盾 | 40 | [人设结构与迭代](errors/01-structure.md) |
| 把参考脚本原样抄成 Few-Shot | 41 | [人设结构与迭代](errors/01-structure.md) |
| 压平的 Prompt 直接动手改 | 42 | [人设结构与迭代](errors/01-structure.md) |
| 禁列表符号与要求数字列表并存，`1.` 被删除后误断句 | 43 | [输出格式](errors/02-format.md) |
| 大屏需要保留 `1. 2. 3.`，但 `**` 和 `#` 必须禁掉 | 44 | [输出格式](errors/02-format.md) |
| 回复内容带 `**`，普通格式禁令拦不住 | 45 | [输出格式](errors/02-format.md) |
| 播报里带冒号，听起来机械 | 46 | [输出格式](errors/02-format.md) |
| 括号里的动作神态被念出来 | 47 | [输出格式](errors/02-format.md) |
| 字数限制完全不生效 | 48 | [输出格式](errors/02-format.md) |
| 字数限制的理由写成"大屏展示"，但载体是实体机器人 | 49 | [输出格式](errors/02-format.md) |
| 知识库括号内的补充说明被读出来 | 50 | [输出格式](errors/02-format.md) |
| 网址和图片链接被念出来 | 51 | [输出格式](errors/02-format.md) |
| 公司名读音被括号标注，每次对话重复读 | 52 | [输出格式](errors/02-format.md) |
| 模型把 Markdown 符号念成"星号星号""井号" | 53 | [输出格式](errors/02-format.md) |
| 去列表化禁令下达后，模型仍吐数字序号 | 54 | [输出格式](errors/02-format.md) |
| Few-Shot 示例是长段落，字数禁令形同虚设 | 55 | [输出格式](errors/02-format.md) |
| 首句没有标点，与后文黏成一句长播报 | 56 | [输出格式](errors/02-format.md) |
| 断句按书面标点走，听起来不像说话 | 57 | [输出格式](errors/02-format.md) |
| 越界问题没有固定话术，模型开始编造 | 58 | [输出格式](errors/02-format.md) |
| 素材未覆盖的故障类型 | 59 | [输出格式](errors/02-format.md) |
| 每轮反问，把用户问句原样反抛回去 | 60 | [模型行为](errors/03-behavior.md) |
| 每轮结尾都征求许可，问「要不要了解细节」 | 61 | [模型行为](errors/03-behavior.md) |
| 写死的话术被逐字照搬，同一意图永远同一个回复结构 | 62 | [模型行为](errors/03-behavior.md) |
| 回复里暴露出 Prompt 配置与设定条款 | 63 | [模型行为](errors/03-behavior.md) |
| 回复里说出「启动数据库」「正在扫描」这类后台动作词 | 64 | [模型行为](errors/03-behavior.md) |
| 兜底拒答话术泛滥，正常问题也被拒 | 65 | [模型行为](errors/03-behavior.md) |
| 为不存在的外部知识库写「检索不到就兜底」 | 66 | [模型行为](errors/03-behavior.md) |
| 安全提醒话术机械刷屏 | 67 | [模型行为](errors/03-behavior.md) |
| 字数压太死，复杂事项讲不透彻 | 68 | [模型行为](errors/03-behavior.md) |
| 拒答之后把无关技能当兜底推销（乌云舞） | 69 | [模型行为](errors/03-behavior.md) |
| 同一台词反复出现，例句删不掉又要止住复读 | 70 | [模型行为](errors/03-behavior.md) |
| 过渡词重复播报两遍 | 71 | [模型行为](errors/03-behavior.md) |
| 把上一个客户的设定带进新场景 | 72 | [模型行为](errors/03-behavior.md) |
| 跨轮失忆，用户早前说的硬性信息被丢掉 | 73 | [模型行为](errors/03-behavior.md) |
| 业务能力写成物理动作，模型输出做不到的台词 | 74 | [模型行为](errors/03-behavior.md) |
| 人设残留旧场景称谓，暴露给甲方 | 75 | [模型行为](errors/03-behavior.md) |
| 模型答出知识库里没有的内容 | 76 | [知识库配合](errors/04-knowledge.md) |
| 「尽量只用知识库」约束过弱 | 77 | [知识库配合](errors/04-knowledge.md) |
| 模型把知识库文件名念出来 | 78 | [知识库配合](errors/04-knowledge.md) |
| 引用角标 [1] [2] 出现在回复中 | 79 | [知识库配合](errors/04-knowledge.md) |
| 知识库原文的数字列表被照搬 | 80 | [知识库配合](errors/04-knowledge.md) |
| 知识库里的图片 CDN 链接被朗读 | 81 | [知识库配合](errors/04-knowledge.md) |
| 知识库里有二维码就自动推二维码 | 82 | [知识库配合](errors/04-knowledge.md) |
| 专家名单被摘要成两三个 | 83 | [知识库配合](errors/04-knowledge.md) |
| 「我要挂号」被误判成无关问题拒回 | 84 | [知识库配合](errors/04-knowledge.md) |
| 知识库只有历史年份，问「今天」就乱答 | 85 | [知识库配合](errors/04-knowledge.md) |
| 机器人端不能挂知识库，模型说自己不会跳舞 | 86 | [知识库配合](errors/04-knowledge.md) |
| 想在 FAQ 里穷举所有问法 | 87 | [知识库配合](errors/04-knowledge.md) |
| 内嵌知识库时直接粘长文档 | 88 | [知识库配合](errors/04-knowledge.md) |
| 提炼过度被客户打回「知识太少」 | 89 | [知识库配合](errors/04-knowledge.md) |
| 把二维码的调用逻辑写进了知识库 | 90 | [知识库配合](errors/04-knowledge.md) |
| 知识库名称与后台不一致导致不弹图 | 91 | [知识库配合](errors/04-knowledge.md) |
| 挂号从二维码改成链接后仍给二维码 | 92 | [知识库配合](errors/04-knowledge.md) |
| 科室层够用却推荐了具体医生 | 93 | [知识库配合](errors/04-knowledge.md) |
| 多轮理解配置污染当前轮判断 | 94 | [知识库配合](errors/04-knowledge.md) |
| 模型对商务敏感问题给出承诺 | 95 | [知识库配合](errors/04-knowledge.md) |
| 固定口径太像线上客服，不会现场引流 | 96 | [知识库配合](errors/04-knowledge.md) |
| 知识库检索范围与展会定位错配 | 97 | [知识库配合](errors/04-knowledge.md) |
| 知识按产品线补充后模型不做分流推荐 | 98 | [知识库配合](errors/04-knowledge.md) |
| 素材未覆盖 | 99 | [知识库配合](errors/04-knowledge.md) |
| 知识库中不存在的医生被凭空编造出来 | 100 | [幻觉压制](errors/05-hallucination.md) |
| 召回内容正确，输出却把 A 科室的医生归进 B 科室 | 101 | [幻觉压制](errors/05-hallucination.md) |
| 认错被当成服务态度问题而被禁止，模型改为继续圆谎 | 102 | [幻觉压制](errors/05-hallucination.md) |
| 省略句追问被判为「查不到」，模型输出暂无数据 | 103 | [幻觉压制](errors/05-hallucination.md) |
| Excel 知识库中的合并单元格导致科室与医生错配 | 104 | [幻觉压制](errors/05-hallucination.md) |
| 「回复要简短」与「名单要列全」互相内耗，模型靠瞎编或过度缩写过关 | 105 | [幻觉压制](errors/05-hallucination.md) |
| 免责话术把患者推向泛化的「正规医疗机构」，本院转化归零 | 106 | [幻觉压制](errors/05-hallucination.md) |
| 回复里暴露知识库文件名 | 107 | [幻觉压制](errors/05-hallucination.md) |
| 兜底话术只有道歉、没有下一步动作，模型在下次追问时转向编造 | 108 | [幻觉压制](errors/05-hallucination.md) |
| 多轮对话后人设退化成冷冰冰的普通客服 | 109 | [多轮与场景](errors/06-multiturn.md) |
| 业务解答完，下一轮闲聊仍残留上一轮的严肃语气 | 110 | [多轮与场景](errors/06-multiturn.md) |
| 智能体只能干一个岗位，体验者问「你能做什么」时暴露不了多场景能力 | 111 | [多轮与场景](errors/06-multiturn.md) |
| 场景切换后不宣告岗位、不主动抛题，体验者不知道切换是否生效 | 112 | [多轮与场景](errors/06-multiturn.md) |
| 面试官无限套娃，不给结论也不结束 | 113 | [多轮与场景](errors/06-multiturn.md) |
| 面试开场直接抛场景题，没有自我介绍 | 114 | [多轮与场景](errors/06-multiturn.md) |
| 深挖阶段跑去问新话题，候选人经历没被追问 | 115 | [多轮与场景](errors/06-multiturn.md) |
| 销售对练中陪练抢话、主动推销、主导话题 | 116 | [多轮与场景](errors/06-multiturn.md) |
| 对练第一轮就把预算、痛点全交代，学员无从挖掘 | 117 | [多轮与场景](errors/06-multiturn.md) |
| 收口轮被字数上限卡住，评价或总结输出残缺 | 118 | [多轮与场景](errors/06-multiturn.md) |
| 同一 Prompt 内残留两个字数上限版本 | 119 | [多轮与场景](errors/06-multiturn.md) |
| Few-Shot 里带括号动作描写，与禁令冲突后被模型模仿 | 120 | [多轮与场景](errors/06-multiturn.md) |
| 结束语由模型自由生成，二维码与留存动作丢失 | 121 | [多轮与场景](errors/06-multiturn.md) |
| 挂了插件但只有明确命令才联网 | 122 | [工具调用](errors/07-tool.md) |
| 固定场景不调工作流，改用文字或知识库直接答 | 123 | [工具调用](errors/07-tool.md) |
| 工作流名与平台配置名不一致导致不命中 | 124 | [工具调用](errors/07-tool.md) |
| 知识库拦截了工作流 | 125 | [工具调用](errors/07-tool.md) |
| 过渡话术没生效，数字人静默卡住两三秒 | 126 | [工具调用](errors/07-tool.md) |
| 过渡话术被念了两遍 | 127 | [工具调用](errors/07-tool.md) |
| 调用结束后答非所问，重新寒暄或复述等待语 | 128 | [工具调用](errors/07-tool.md) |
| 屏幕上打出 function= 和 parameters= 代码 | 129 | [工具调用](errors/07-tool.md) |
| 工作流返回永远是空，JSONPath 键名对不上 | 130 | [工具调用](errors/07-tool.md) |
| 返回体被二次转义成字符串，路径检索失效 | 131 | [工具调用](errors/07-tool.md) |
| 工作流测试总报查无数据，其实是样本不在库内 | 132 | [工具调用](errors/07-tool.md) |
| 插件失败时模型编造过期日期或虚假天气 | 133 | [工具调用](errors/07-tool.md) |
| 缺参直接调工作流，提交空参数报错 | 134 | [工具调用](errors/07-tool.md) |
| 模糊提问时模型自己猜着调 | 135 | [工具调用](errors/07-tool.md) |
| 轻量模型下工具调用格式不稳定 | 136 | [工具调用](errors/07-tool.md) |
| 数字人文本里出现括号动作神态描写 | 137 | [工具调用](errors/07-tool.md) |
| 工作流与知识库覆盖同一话题时业务冲突 | 138 | [工具调用](errors/07-tool.md) |
| 大屏前静默三秒，游客以为设备坏了 | 139 | [工具调用](errors/07-tool.md) |
| ASR 同音错字触发模型自我纠错，先来一句"您可能是想了解" | 140 | [语音与多语言](errors/08-voice.md) |
| 专有名词被识别成谐音，检索命中不了知识库 FAQ | 141 | [语音与多语言](errors/08-voice.md) |
| 加了"可切换英文"的技能，用户英文提问仍回中文 | 142 | [语音与多语言](errors/08-voice.md) |
| 语言教学类人设被用户的中文带跑，全程变成中文对话 | 143 | [语音与多语言](errors/08-voice.md) |
| 英文回复沿用中文的字数上限，播报过短或过长 | 144 | [语音与多语言](errors/08-voice.md) |
| 同一 Prompt 里既禁语气词又要求加填充词 | 145 | [语音与多语言](errors/08-voice.md) |
| 播报文本里混入动作神态描写与屏幕 UI 描述 | 146 | [语音与多语言](errors/08-voice.md) |
| 英文 Prompt 里残留跨人设的复制粘贴内容 | 147 | [语音与多语言](errors/08-voice.md) |
| 数字型专有名词只写数字部分，纠偏词表漏掉读法变体 | 148 | [语音与多语言](errors/08-voice.md) |
| 语言规则写成了"允许"而不是"禁止" | 149 | [语音与多语言](errors/08-voice.md) |
| 用空间位置做阶段触发条件 | 150 | [跨载体改写](errors/09-carrier.md) |
| 主宾姓名写死在台词里 | 151 | [跨载体改写](errors/09-carrier.md) |
| 硬件动作括号被当成台词念出来 | 152 | [跨载体改写](errors/09-carrier.md) |
| 中控脚本与人设 Prompt 抢动作 | 153 | [跨载体改写](errors/09-carrier.md) |
| 大屏被要求带路 | 154 | [跨载体改写](errors/09-carrier.md) |
| AGV 承诺带路到未入库地点 | 155 | [跨载体改写](errors/09-carrier.md) |
| 载体人设保留大幅动作技能 | 156 | [跨载体改写](errors/09-carrier.md) |
| 字数上限一刀切 | 157 | [跨载体改写](errors/09-carrier.md) |
| 插件调用时现场冷场 | 158 | [跨载体改写](errors/09-carrier.md) |
| 开场白念技术黑话 | 159 | [跨载体改写](errors/09-carrier.md) |
| 展示型产物被塞进主 Prompt | 160 | [跨载体改写](errors/09-carrier.md) |
| 同一人设换载体只改名不改能力 | 161 | [跨载体改写](errors/09-carrier.md) |
| 自助设备口头承诺价格 | 162 | [跨载体改写](errors/09-carrier.md) |
| 国企/央企载体保留网络语调 | 163 | [跨载体改写](errors/09-carrier.md) |
| 换载体后 Few-Shot 没跟着改 | 164 | [跨载体改写](errors/09-carrier.md) |
| 把语音唤醒写进触发条件 | 165 | [跨载体改写](errors/09-carrier.md) |
| 未覆盖载体的错误类比 | 166 | [跨载体改写](errors/09-carrier.md) |
| 医疗类人设把知识约束写成"尽量"，模型上网抓偏方 | 167 | [行业场景](errors/10-scene-b2b.md) |
| 医疗类人设写"不对问题进行衍生"，科普完不指引科室，业务闭环断掉 | 168 | [行业场景](errors/10-scene-b2b.md) |
| 医疗漏斗方向写反，家长问辅食就被推销挂号，冒犯感极强 | 169 | [行业场景](errors/10-scene-b2b.md) |
| 医疗人设开场白出现语病，家长第一句就被冒犯 | 170 | [行业场景](errors/10-scene-b2b.md) |
| 医疗人设把知识库文件名和引用角标念给患者听 | 171 | [行业场景](errors/10-scene-b2b.md) |
| 政务人设用预训练知识回答区级政策，答成了全国通用流程 | 172 | [行业场景](errors/10-scene-b2b.md) |
| 政务人设遇到宽泛问题一次性堆砌所有情形，群众看不下去 | 173 | [行业场景](errors/10-scene-b2b.md) |
| 涉诈警情先背法条流程，错失止损黄金时间 | 174 | [行业场景](errors/10-scene-b2b.md) |
| 政务人设承诺了办结时限，越权且无法兑现 | 175 | [行业场景](errors/10-scene-b2b.md) |
| 政务人设被问办案进展，直接透露了调查细节 | 176 | [行业场景](errors/10-scene-b2b.md) |
| 景区讲解一次背完所有站点，游客听两句就走 | 177 | [行业场景](errors/10-scene-b2b.md) |
| 联网查天气不设过渡词，数字人在屏幕前哑巴两三秒 | 178 | [行业场景](errors/10-scene-b2b.md) |
| 过渡词在拿到结果后重复播报，一句话说两遍 | 179 | [行业场景](errors/10-scene-b2b.md) |
| 景区讲解只说"很高很漂亮"，全是正确的废话 | 180 | [行业场景](errors/10-scene-b2b.md) |
| 景区人设承诺"今天一定能看清外滩"，被天气打脸 | 181 | [行业场景](errors/10-scene-b2b.md) |
| 把"话题独立性"写成绝对禁令，模型把核心硬约束也一起清空 | 182 | [行业场景](errors/10-scene-b2b.md) |
| Few-Shot 只演示单轮回应，反而强化了模型的失忆 | 183 | [行业场景](errors/10-scene-b2b.md) |
| 把"主动招揽路人"写进业务能力，模型输出硬件做不到的台词 | 184 | [行业场景](errors/10-scene-b2b.md) |
| 后台数据拼接标签被念给现场观众听 | 185 | [行业场景](errors/10-scene-b2b.md) |
| 保健酒被讲成"降三高"，直接踩食品药品监管红线 | 186 | [行业场景](errors/10-scene-b2b.md) |
| 酒类人设漏了健康饮酒警示，合规缺项 | 187 | [行业场景](errors/10-scene-b2b.md) |
| 官网助手承诺了具体售价，商务侧无法兑现 | 188 | [行业场景](errors/10-scene-b2b.md) |
| 官网助手用旧记忆回答"今天几号" | 189 | [行业场景](errors/10-scene-b2b.md) |
| 央企展台沿用消费级"有梗"语调，客户当场否决 | 190 | [行业场景](errors/10-scene-b2b.md) |
| 央企 Prompt 内又写了一遍知识库正文，与外部 RAG 打架 | 191 | [行业场景](errors/10-scene-b2b.md) |
| 把具体人名和物理路线硬编码，换个展台就完全不可复用 | 192 | [行业场景](errors/10-scene-b2b.md) |
| 具身机器人不分阶段，一开口把谢幕词也念了 | 193 | [行业场景](errors/10-scene-b2b.md) |
| 大屏数字人把括号动作描写念出来 | 194 | [行业场景](errors/10-scene-b2b.md) |
| 只写"禁止井号"，模型仍然输出 Markdown 标题 | 195 | [行业场景](errors/10-scene-b2b.md) |
| 前台角色名前后不一致，同一份 Prompt 里出现两个名字 | 196 | [行业场景](errors/10-scene-b2b.md) |
| 展台版 Prompt 直接搬到公司大堂，业务动作全部错位 | 197 | [行业场景](errors/10-scene-b2b.md) |
| 模板串行业污染，上一个客户的话术规则残留在新行业 Prompt 里 | 198 | [行业场景](errors/10-scene-b2b.md) |
| 大屏智能体只做咨询不留资，流量用完即走 | 199 | [行业场景](errors/10-scene-b2b.md) |
| 首句不锁长度，数字人开口就是三十字长句 | 200 | [行业场景](errors/10-scene-b2b.md) |
| 双语能力只写"可以英文回答"，英文回复长度失控 | 201 | [行业场景](errors/10-scene-b2b.md) |
| 超写实人像仍在 Prompt 里自称「机器人」 | 202 | [机器人角色](errors/11-scene-robot.md) |
| 身份写成「银行或电信营业厅」，一个「或」字废掉整套人设 | 203 | [机器人角色](errors/11-scene-robot.md) |
| 场景停在抽象层，连续四轮被退回 | 204 | [机器人角色](errors/11-scene-robot.md) |
| 写了「禁止话题关联」，模型四五轮后把用户硬约束也忘了 | 205 | [机器人角色](errors/11-scene-robot.md) |
| 开场白套黄金模板，温婉学姐被写成工具人 | 206 | [机器人角色](errors/11-scene-robot.md) |
| 括号动作描写被 TTS 念出来，或整段表现力被删光 | 207 | [机器人角色](errors/11-scene-robot.md) |
| 字数限制的理由写成「大屏展示」，但角色是语音播报 | 208 | [机器人角色](errors/11-scene-robot.md) |
| 英文输出用中文字数限制，约束直接失效 | 209 | [机器人角色](errors/11-scene-robot.md) |
| 没有联网却设成体育新闻主持人，被问比分必然胡编 | 210 | [机器人角色](errors/11-scene-robot.md) |
| 客户要求「不要取名字」，Few-Shot 示例里还留着名字 | 211 | [机器人角色](errors/11-scene-robot.md) |
| 客户补充知识库后，旧口径没同步更新 | 212 | [机器人角色](errors/11-scene-robot.md) |
| 把「欢迎手势」「双手平摊」写进 Prompt | 213 | [机器人角色](errors/11-scene-robot.md) |
| 业务能力写成态度词，模型只能说空话 | 214 | [机器人角色](errors/11-scene-robot.md) |
| 模板残留其他行业的术语，出现在不相干的人设里 | 215 | [机器人角色](errors/11-scene-robot.md) |
| 视觉与品类错配，穿泳装的角色开口讲车机 | 216 | [机器人角色](errors/11-scene-robot.md) |
| 新角色与已有角色撞场景，做了第二遍口语陪练 | 217 | [机器人角色](errors/11-scene-robot.md) |
| 角色承诺录取、承诺包过 | 218 | [机器人角色](errors/11-scene-robot.md) |
| 回复里带冒号与数字列表，播报像在念表格 | 219 | [机器人角色](errors/11-scene-robot.md) |
| 形象与功能都对了，但客户不认这是「服务机器人」 | 220 | [机器人角色](errors/11-scene-robot.md) |
| 全英文人设里混进中文提示，语言红线失效 | 221 | [机器人角色](errors/11-scene-robot.md) |
