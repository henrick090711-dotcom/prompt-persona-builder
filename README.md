# prompt-persona-builder

给数字人、机器人、智能体写人设 Prompt，以及改别人写坏的人设 Prompt。

这套文档来自 202 轮真实项目对话的提炼，覆盖金融、医疗、政务、文旅、零售、能源、会展等行业的落地案例，最终收敛成一套可复用的结构、约束写法和故障百科。

## 装什么

人设 Prompt 的六块骨架、每块的边界、简化版怎么砍、Markdown 格式规范、开场白与推荐问题怎么写；输出格式的死锁写法；模型行为的调优手法；知识库与人设的配合；幻觉压制；多轮流程与场景切换；工具与工作流调用；语音场景的 ASR 纠错；同一人设跨载体改写；以及一批可直接改字段就用的行业模板。

## 什么时候用

- 要写一个数字人、机器人、智能体的人设
- 客户给了现成 Prompt，要求优化、简化、加功能、换场景
- 模型反复反问、话术像复读机、输出带 Markdown、字数控制不住
- 知识库召不回来、模型开始编造科室医生电话
- 语音场景里品牌名被听错
- 同一套人设要同时上大屏、机器人本体、线上智能体

## 目录结构

```
prompt-persona-builder/
├── SKILL.md                              入口索引与核心原则
├── README.md                             本文件
├── LICENSE                               MIT
├── references/
│   ├── persona-structure.md              人设 Prompt 的标准结构
│   ├── persona-tuning.md                 现成人设的改写与迭代
│   ├── format-control.md                 输出格式约束
│   ├── behavior-tuning.md                模型行为调优
│   ├── knowledge-prompt.md               Prompt 与知识库配合
│   ├── hallucination.md                  幻觉压制
│   ├── multi-turn.md                     多轮对话与场景切换
│   ├── tool-invocation.md                工具与工作流调用
│   ├── asr-multilingual.md               语音场景与多语言
│   ├── carrier-diff.md                   跨载体改写
│   ├── scene-b2b.md                      B 端行业场景模板
│   ├── scene-robot.md                    机器人/数字人角色模板
│   ├── errors.md                         故障百科索引（221 条）
│   └── errors/                           故障百科分册
│       ├── 01-structure.md               1–42    人设结构与迭代
│       ├── 02-format.md                  43–59   输出格式
│       ├── 03-behavior.md                60–75   模型行为
│       ├── 04-knowledge.md               76–99   知识库配合
│       ├── 05-hallucination.md           100–108 幻觉压制
│       ├── 06-multiturn.md               109–121 多轮与场景
│       ├── 07-tool.md                    122–139 工具调用
│       ├── 08-voice.md                   140–149 语音与多语言
│       ├── 09-carrier.md                 150–166 跨载体改写
│       ├── 10-scene-b2b.md               167–201 行业场景
│       └── 11-scene-robot.md             202–221 机器人角色
└── examples/
    └── minimal-persona.md                最小可用骨架与填法示例
```

## 怎么读

第一次接触这套东西，从 `examples/minimal-persona.md` 开始，先跑通六块骨架。骨架跑通后遇到具体问题，再按 `SKILL.md` 的路由表查对应主题篇。查报错直接进 `references/errors.md` 按现象找编号。

不要一次读完所有文档。这套文档按「遇到问题查一篇」设计，通读反而抓不住重点。

## 与 Dify 对话流的关系

这套文档只管 Prompt 层。要搭 Dify 对话流、设计状态机、配节点变量、接 HTTP 接口，用另一套 `dify-chatflow-builder`。

两者的交界：对话流的节点提示词怎么写、变量怎么嵌进 Prompt、多场景分诊的 Prompt 层怎么设计，两套文档都有覆盖，看哪边更贴近当前问题。

## 兼容性

统一使用标准命名 `SKILL.md`。若目标平台要求小写文件名，复制一份改名即可，注意 GitHub 不允许同一目录下存在两个仅大小写不同的文件。

## 许可

MIT License，见 `LICENSE`。
