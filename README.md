# 复制爆款

> 想快速复制爆款起号？这个库收集逆向拆解和复刻爆款视频的方法，每条都写清楚能帮你解决什么、怎么用它搞钱。
>
> A curated collection of viral-video replication prompts & skills for viral short videos, gathered from practitioners sharing on X.
> 
> Each entry answers: what problem it solves (and who it's for), how to use it step by step, and how to make money with it.
> 
> Star counts verified via GitHub API on 2026-10-12. Continuously updated.

## 条目

### awesome-opus5-5-videos

**核心提炼**
- 解决什么问题：不知道 AI 视频能做成什么样、没灵感——523 个 X 爆款视频 + 背后 prompt，每个附 Skillry 上的实时复刻对比。
- 核心用法（3 步）：1) 按分类（动效/科普/3D/游戏）挑一个喜欢的 → 2) 打开 prompts/ 下对应 prompt 文件复制 → 3) 粘给 Claude Opus 5.5（或自己的 agent）渲染成单 HTML 文件，录屏即成视频。
- 什么时候用 / 常见坑：找选题灵感、学爆款 prompt 写法时用；部分条目只公开了部分 prompt，文件里会注明，复刻出来可能有差距。

**适用场景**：想用 AI 做爆款视频的内容创作者、prompt 研究者。

**怎么用它搞钱**：拆解爆款做同款，快速涨粉。

**来源**：[yihui-dev/awesome-opus5-5-videos](https://github.com/yihui-dev/awesome-opus5-5-videos) · ⭐4370 · 更新于 2026-10-12

### viral-video-replicator

**核心提炼**
- 解决什么问题：看到竞品爆款想复刻但不知道怎么拆——逆向提取参考视频全部参数，生成 Seedance 2.0 可直接用的复刻 prompt。
- 核心用法（5 步）：1) 装 skill（Claude Code）+ 备好 FFmpeg 和火山方舟 API → 2) 丢参考视频说"复刻这个" → 3) 自动帧提取→ASR 转录→视觉结构化分析 → 4) 选 4 种替换模式（纯复刻/换脸/换衣/全换）→ 5) 拿 prompt 去即梦按操作手册生成。
- 什么时候用 / 常见坑：服装带货、穿搭类目对标复刻最合适；依赖火山方舟视觉 API 和 Seed-ASR，服务挂了会降级（纯视觉分析会丢对话）；本地要有 FFmpeg。

**适用场景**：服装/带货类目、想对标爆款快速起号的账号运营者。

**怎么用它搞钱**：对标账号快速复制起号。

**来源**：[dingtom336-gif/viral-video-replicator](https://github.com/dingtom336-gif/viral-video-replicator) · ⭐43 · 更新于 2026-04-01

### hypit

**核心提炼**
- 解决什么问题：一条爆款想出 100 个变体，一个个剪太慢——给 agent 一套"视频语言"（SVML），投一个参考视频，agent 按完整工作流克隆：画面、字幕、B-roll、特效都对着文字锚点重建。
- 核心用法（4 步）：1) `npx skills add hypit-ai/hypit -g` 装 skill → 2) 丢参考视频给 agent（Claude Code/Codex）→ 3) agent 解析成 SVML 工作流 → 4) 换人脸/换文案/换 B-roll，一条命令批量出变体。
- 什么时候用 / 常见坑：做系列化同款（测评、榜单、口播）批量起量时用；生成模型可选，不调用就不产生模型费用；license 是带条件的 Apache 2.0，商用前看一眼 LICENSE。

**适用场景**：想批量复制爆款结构、跑矩阵号的团队和个人。

**怎么用它搞钱**：矩阵号批量复刻爆款起号，或给品牌做"同款爆款结构"代运营。

**来源**：[hypit-ai/hypit](https://github.com/hypit-ai/hypit) · ⭐21397 · 更新于 2026-10-09

### AI-Youtube-Shorts-Generator

**核心提炼**
- 解决什么问题：长视频/直播回放没人看完——自动找高光金句切成竖屏爆款短片，省掉 Opus Clip 每月 20–300 美元的订阅。
- 核心用法（4 步）：1) 装好（API 模式要 MuAPI key，本地模式要 ffmpeg + LLM key）→ 2) 丢 YouTube 长视频链接 → 3) Whisper 转录 + LLM 按爆款维度（钩子、情绪峰值、金句）打分选高光 → 4) 自动竖屏裁剪导出 N 条 9:16 成片；支持 xargs 批量跑整个链接列表。
- 什么时候用 / 常见坑：有长视频存量（播客、直播、课程）想转短视频引流时用；高光算法开源可调；本地模式可全离线，但要自己配模型。

**适用场景**：有长视频内容、想低成本做短视频矩阵的博主和机构。

**怎么用它搞钱**：给长视频博主/机构做切片代运营（按条收费），或自己切矩阵号涨粉带货。

**来源**：[Anil-matcha/AI-Youtube-Shorts-Generator](https://github.com/Anil-matcha/AI-Youtube-Shorts-Generator) · ⭐5310 · 更新于 2026-10-11

### @brainextends《AI UGC 0 成本复刻五步法》

**核心提炼**
- 解决什么问题：预算为零也想复制 AI UGC 爆款——一条极简可复用的"拆格式→首帧→图生视频→批量变体"工作流，不花钱也能跑。
- 核心用法（5 步）：1) 在 TikTok/IG Reels 上找一个跑起来的爆款视频格式 → 2) 用 ChatGPT 对该格式做逆向拆解（reverse engineer），拆出结构骨架 → 3) 用免费额度的图生图模型（帖中用 GPT Images 免费计划，每天 2–3 张）生成首帧图 → 4) 把首帧图喂给 Seedance 做图生视频 → 5) 用 Seedance 的多图参考（multi-image reference）功能批量做出无限个变体。
- 什么时候用 / 常见坑：低成本跑量、一次测多个变体时用；逆向拆解抄的是"格式骨架"不是照搬内容，首帧图质量决定成片下限。

**适用场景**：预算为零、想低成本复制 AI UGC 爆款格式的个人创作者。

**怎么用它搞钱**：用免费额度加 Seedance 批量产出 UGC 风格带货/引流视频，低成本起矩阵号，或接"爆款格式复刻"代做单。

**来源**：[@brainextends](https://x.com/brainextends/status/2110441122766127486)（2026-10-14）

### @wonfull888《video-to-prompt：视频反推提示词 skill》

**核心提炼**
- 解决什么问题：看到爆款视频想复刻但写不出 prompt——给个视频直接输出中英双语的完整提示词，微调就能拿去生成。
- 核心用法（5 步）：1) 克隆 [wonfull888/ai-video-prompt](https://github.com/wonfull888/ai-video-prompt)，备好 OpenRouter 和 DeepSeek key → 2) 在 Cursor/Codex 里对 agent 说 `video-to-prompt /path/to/video.mp4` → 3) Gemini 3.8 Flash 原生读完整视频（不只是截图）：切分镜、追踪人物动作、运镜、表情 → 4) DeepSeek 二次复核：逐帧核查高难度动作段，删掉画面证据不足的内容，统一人物命名防串人 → 5) 产出中英双语 prompt.md（含证据帧和分镜拆解），直接适配 Seedance 2.5/2.0、Veo、Sora、Kling、Wan。
- 什么时候用 / 常见坑：竞品爆款翻拍、爆款结构批量复用时用；"看"和"核查"分两个模型做（视觉便宜模型看、文本模型验）是成本控制的关键；需自备 API key。

**适用场景**：用 Cursor/Codex 做 AI 视频、想把参考爆款逆向成可复用 prompt 的开发者和工作室。

**怎么用它搞钱**：把竞品爆款批量反推成 prompt 翻拍起号，或提供"爆款视频反推拆解"代拆服务按条收费。

**来源**：[wonfull888/ai-video-prompt](https://github.com/wonfull888/ai-video-prompt)（2026-10-15 经 API 核验真实开源；方法由 [@wonfull888](https://x.com/wonfull888/status/2109791506420969616) 于 2026-10-12 在 X 分享）

### @jonnyscales《UGC 带货视频逆向三要素：抄格式不抄逐字稿》

**核心提炼**
- 解决什么问题：复制 UGC 带货爆款容易抄成"山寨感"——逐字照抄是最大错误，正确做法是逆向拆解这个格式"为什么有效"。
- 核心用法（3 要素）：1) 钩子（hook）——视频开头用什么抓住了注意力 → 2) 叙事线（narrative）——用什么故事线把人留住 → 3) 产品切入时机——产品在视频的哪个时间点、以什么方式出现。三要素拆出来，换自己的产品和话术重拍一条。
- 什么时候用 / 常见坑：做 UGC 广告/带货短视频、想复制爆款又怕同质化被平台降权时用；目标是"看起来自然、自发、真实"，逐字稿一字不落全抄反而最假。

**适用场景**：做 UGC 广告/带货短视频、需要复制爆款结构又要避开同质化的创作者和商家。

**怎么用它搞钱**：用三要素框架批量"合法翻拍"带货爆款，提高转化率；或给商家做 UGC 脚本代写/代拍，按转化效果收费。

**来源**：[@jonnyscales](https://x.com/jonnyscales/status/2110038127674871966)（2026-10-13）

### @double_burger_2《素材库对标复制法：新手不缺灵感》

**核心提炼**
- 解决什么问题：内容新手灵感枯竭、写不出对标爆款的内容——先建库再开写，灵感变成"从库里挑"。
- 核心用法（3 步）：1) 建素材库：把对标博主的视频转成逐字稿，把爆款长文存下来 → 2) 备料到量：至少 10 篇能拆的长文、5 个能模仿的结构、3 个长期对标的账号，备料标准先定死 → 3) 每日用法：打开素材库挑一个观点，换成自己的话讲一遍。
- 什么时候用 / 常见坑：稳定日更、做账号起号冷启动时用；对标账号要长期跟踪同一批（看他们的选题演变），不要今天换一批明天换一批。

**适用场景**：刚起步的内容新手、需要稳定产出对标爆款内容的账号运营者。

**怎么用它搞钱**：对标账号拆解+稳定产出，快速起号接商单；或把"对标素材库搭建"做成代运营服务卖给商家。

**来源**：[@double_burger_2](https://x.com/double_burger_2/status/2110654159053873185)（2026-10-15）

### @xiyue0803《词锚点脚本：剪辑模板化批量复刻》

**核心提炼**
- 解决什么问题：剪商业故事短视频最折磨人的是卡点和大字动画——每次换故事都要逐帧对轨道，苦力活重复做。
- 核心用法（4 步）：1) 拿一条现成的爆款视频喂给 Claude，让 AI 拆解分镜结构、大字出现时机、字幕层级 → 2) 生成"带词锚点的脚本"：锚点绑定具体单词而不是写死时间戳 → 3) 换新文案和新配音，画面和动效按词锚点自动对齐 → 4) 搭好一套模板，不同故事直接套，批量复刻。
- 什么时候用 / 常见坑：剪商业故事/口播类短视频、想一套模板复用多个故事时用；词锚点的关键是"绑定单词不绑定时间"，文案节奏变了对齐才不会崩。

**适用场景**：剪商业故事/口播类短视频、想一套模板批量复用多个故事的剪辑师和工作室。

**怎么用它搞钱**：把高频故事类型做成词锚点模板，接批量代剪单；或自己搭模板矩阵号日更故事号涨粉带货。

**来源**：[@xiyue0803](https://x.com/xiyue0803/status/2110618364179886544)（2026-10-15）

### @superfang119《观默代码动效复刻法：长文转 16 秒预告》

**核心提炼**
- 解决什么问题：想复刻热门代码动效视频但无从下手——复刻观默"长文章转 16 秒预告"的完整实战。
- 核心用法（5 步）：1) 核对原片真实参数：下载原片查得 16.619 秒/1920×1080/995 帧，不轻信帖子自述的"15 秒"，按文件建时间轴；原帖"收藏过 2000"指的是长文而非样片，不混为模型对比依据；2) 核心取舍：预告只保留"一个判断"，不搬全部小标题，一个持续运动的主角（橙色小球）演完全程，背景与主角连续、文字轮流接管；3) 五段式时间轴：0–2.5 秒文章页收起交出主角 → 2.5–5.5 秒演示蓄力/接触/回弹 → 5.5–9 秒走过五个制作节点 → 9–12 秒演示拍点 → 12–16 秒收成文章入口；4) 动画与音频共用一份计划文件：两次落地定在 3.5/4.5 秒（30fps 下第 105/135 帧），五个节点在 5.6/6.2/6.8/7.4/8.0 秒，120BPM 即每拍 0.5 秒=15 帧，拍点事件落在明确帧号；5) 声音全部代码合成（四组和弦琶音+低频鼓点+节点音+落地音效，48kHz 双声道 16 秒共 768000 采样帧），不采样原片配乐。
- 什么时候用 / 常见坑：复刻知识类/教程类动效预告片时用；帖子附完整制作简报模板可直接交给代码 Agent（含交付规格/主角连续性规则/关键时间点/验收项）；声明手工运动曲线不宣称物理仿真、结构检查不代替播放听审。

**适用场景**：想复刻代码动效类爆款视频的创作者、做知识类视频预告的内容号。

**怎么用它搞钱**：把长文/课程批量转成动效预告片引流，或接"知识类视频预告代做单"。

**来源**：[@superfang119](https://x.com/superfang119/status/2110899170861256711)（2026-10-15）

### @superfang119《动效卡库复刻法：637 张卡里挑 3 张跑通》

**核心提炼**
- 解决什么问题：开源动效库 awesome-ai-motion 有 637 张卡片，不知哪张真能用——实测只挑 3 张跑通。
- 核心用法（5 步）：1) 先核对仓库真相：637 条目中仅 128 个标 done 且有对应 MP4，另 509 个为 planned 只有卡片；"改字就导出"只适用于前者，后者需额外开发验收；2) 复刻五步：选卡 → 保留原始时序 → 替换中文内容 → 渲染 → 抽帧查画面，只改文字字体，不动时间线与缓动参数；3) 三张卡实测参数：mask-reveal（文字 yPercent 110→0，0.3 秒起、每行 1.05 秒、第二行晚 0.35 秒、power3.out）、kinetic-type-sweep（1.95 秒匀速 + 0.30 秒 power4.out 急停，中心词变朱红、其余行透明度降至 0.13）、product-demo 配方（光标 2.71 秒点击、回答 2.83 秒逐段出现、放大 4.41 秒开始）；4) 中文适配两坑：换汉字后居中终点须重算（等字体就绪再用 offsetLeft/offsetWidth），打字机间隔数组固定长度、长文案会超时，需同步调整打字安排与点击时间；5) 验收靠抽帧而非只看成片：mask-reveal 查 0.23/0.73/1.23/2.9 秒，kinetic-type-sweep 查 0.9/2.0/2.4/3.3 秒。
- 什么时候用 / 常见坑：想用代码做动效视频/预告片时用；帖子附 Agent 任务提示词模板（读 SKILL.md + 两张卡 + 配方，保留原时序输出 MP4）；最小起步只需 `node scripts/render.mjs effects/mask-reveal --embed --text "…"`（Node 20+/FFmpeg/Playwright/Chromium）。

**适用场景**：想用代码做动效视频的创作者、知识类账号和课程运营者。

**怎么用它搞钱**：批量生产代码动效视频（教程预告/课程宣传）做矩阵号引流，或接代做单。

**来源**：[@superfang119](https://x.com/superfang119/status/2110883959425176056)（2026-10-15）

### @brainextends《Saveo 爆款格式拆解：600 万播放的火柴人营销模板》

**核心提炼**
- 解决什么问题：小预算品牌/账号想做出病毒传播的视频——拆解理财预算类 App「Saveo」靠一条纯 AI 生成短视频一天拿下约 600 万播放、5.6 万新增粉丝的案例，提炼成可套用的格式模板。
- 核心用法（6 条）：1) 钩子公式：第一句就是制造压迫感的悬念开场（大意是"你刚偷了 1000 万美元"），先用一句话把观众钉在屏幕前；2) 低成本画风复用：火柴人（stickman）风格动画，观众一眼有熟悉感，制作门槛低、适合批量复制；3) 连载式剧情留人：围绕"火柴人主角如何把 1000 万现金洗白"展开，观众为了知道后续发展而关注，把单次观看转化成持续追更；4) 游戏化变现设计：剧情做成可互动的游戏玩法，提供 10 美元抢先体验付费入口，按 10% 粉丝转化估算一天可变现约 5.6 万美元；5) 成功六要素：剧本和钩子写得好、Reels 做成互动游戏、用悬念让观众"为了知道结局而关注"、观众对主角剧情产生情感投入、火柴人风格辨识度极高、用好色彩心理学营造情绪；6) 结论：强钩子开场 + 连载悬念 + 低成本高辨识度动画 + 游戏化变现的简单组合，低成本、可规模化复制。
- 什么时候用 / 常见坑：小预算品牌做病毒传播、想做系列连载账号时用；学的是"悬念开场+连载+游戏化"的组合结构，不是照搬剧情题材，换成自己的赛道重写。

**适用场景**：小预算品牌、想做连载型短视频账号的内容创作者和 App 获客方。

**怎么用它搞钱**：用"悬念钩子+连载剧情+游戏化变现"模板做系列号吸粉，用小额付费入口做转化；或给品牌做同款病毒营销代运营。

**来源**：[@brainextends](https://x.com/brainextends/status/2110814597653664113)（2026-10-15；午档窗口内漏收，晚档补录）

## 收录标准

- 来源：X 博主实战分享（原帖 / 评论区 / 引用链）及 GitHub 高星项目
- 每条格式：核心提炼（解决什么问题 / 核心用法 / 什么时候用）+ 适用场景 + 「怎么用它搞钱」+ 来源链接
- Star 数为 2026-10-12 经 GitHub API 核验；持续收录中
- 去重：同一项目只收录一次，不堆 raw 链接

## 相关分类

- 总索引：[x-viral-video-skills](https://github.com/kkone1238899/x-viral-video-skills) —— 13 个分类导航
- [x-viral-video-scripts](https://github.com/kkone1238899/x-viral-video-scripts) —— 编剧 / 脚本
- [x-viral-video-hooks](https://github.com/kkone1238899/x-viral-video-hooks) —— 标题 / 5 秒钩子
- [x-viral-video-creative-direction](https://github.com/kkone1238899/x-viral-video-creative-direction) —— 创意总监
- [x-viral-video-directing](https://github.com/kkone1238899/x-viral-video-directing) —— 导演
- [x-viral-video-breakdown](https://github.com/kkone1238899/x-viral-video-breakdown) —— 拉片
- [x-viral-video-pipeline](https://github.com/kkone1238899/x-viral-video-pipeline) —— 流水线 / 生产管线
- [x-viral-video-de-ai](https://github.com/kkone1238899/x-viral-video-de-ai) —— 去 AI 味
- [x-viral-video-characters](https://github.com/kkone1238899/x-viral-video-characters) —— 人物构建
- [x-viral-video-editing](https://github.com/kkone1238899/x-viral-video-editing) —— 视听剪辑技巧
- [x-viral-video-prompt-opt](https://github.com/kkone1238899/x-viral-video-prompt-opt) —— 提示词优化
- [x-viral-video-copywriting](https://github.com/kkone1238899/x-viral-video-copywriting) —— 文案
- [x-viral-video-showcase](https://github.com/kkone1238899/x-viral-video-showcase) —— X 病毒视频合集

## 投稿

发现好的复制爆款 prompt / skill，欢迎提 Issue 或 PR（格式见 CONTRIBUTING.md）。

## 更新日志

- 2026-10-15 晚档：新增 3 个 X 来源条目（@superfang119 观默代码动效复刻法、@superfang119 动效卡库复刻法、@brainextends Saveo 爆款格式拆解（午档窗口内漏收、晚档补录）），条目总数 12
- 2026-10-15：新增 5 个 X 来源条目（@brainextends AI UGC 五步复刻、@wonfull888 video-to-prompt 反推 skill、@jonnyscales UGC 逆向三要素、@double_burger_2 素材库对标法、@xiyue0803 词锚点批量复刻），条目总数 9
- 2026-10-12：条目升级为小节式（核心提炼/适用场景/怎么用它搞钱），新增 2 个项目，Star 全部重新核验
- 2026-10-11：首版，2 个项目，持续收录中
