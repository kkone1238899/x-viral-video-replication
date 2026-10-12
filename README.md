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

- 2026-10-12：条目升级为小节式（核心提炼/适用场景/怎么用它搞钱），新增 2 个项目，Star 全部重新核验
- 2026-10-11：首版，2 个项目，持续收录中
