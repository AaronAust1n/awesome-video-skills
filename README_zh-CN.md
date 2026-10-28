# Awesome Video Skills

[English](README.md) | **中文**

> 精选开源项目合集，主题：**用文本模型做视频**——LLM（Claude / Opus / Codex…）写代码，Remotion、HyperFrames、three.js、Blender、manim 等渲染引擎执行代码，输出视频。确定性、可编辑、Agent 原生。
>
> 范围说明：核心聚焦*代码渲染*视频。提示词驱动的视频生成模型工作流（Seedance 等）有[独立章节](#seedance-与视频生成模型工作流)，扩散模型 / Agentic 平台在末尾简述。

[![Awesome](https://cdn.jsdelivr.net/gh/sindresorhus/awesome@d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

**数据快照：2026-10-07** · Stars 数据来自当日 GitHub API（`54.3k` = 54,300 星）· **479 个 GitHub 仓库 + X 社区动态**

---

## 目录

- [展示：代码渲染作品](#展示代码渲染作品) (8)
- [渲染引擎（代码→视频）](#渲染引擎代码视频) (39)
- [AI 视频编辑 Agent](#ai-视频编辑-agent) (36)
- [Agentic 生产系统与短视频流水线](#agentic-生产系统与短视频流水线) (28)
- [MCP 与控制层](#mcp-与控制层) (13)
- [视频技能：产品影片、宣传片与解说视频](#视频技能产品影片宣传片与解说视频) (45)
- [视频技能：短剧、故事与 Recap](#视频技能短剧故事与-recap) (9)
- [manim 与数学教育视频](#manim-与数学教育视频) (19)
- [建模案例与技能](#建模案例与技能) (16)
- [Seedance 与视频生成模型工作流](#seedance-与视频生成模型工作流) (19)
- [开源视频生成模型](#开源视频生成模型) (36)
- [数字人、语音与工具链](#数字人语音与工具链) (45)
- [视频翻译与唇形同步](#视频翻译与唇形同步) (15)
- [视频字幕、转写与翻译工具](#视频字幕转写与翻译工具) (14)
- [视频增强、超分与修复](#视频增强超分与修复) (25)
- [ComfyUI 视频生态与自定义节点](#comfyui-视频生态与自定义节点) (20)
- [FFmpeg 与 CLI 视频工具链](#ffmpeg-与-cli-视频工具链) (8)
- [Blender 与 3D](#blender-与-3d) (7)
- [角色、动捕与游戏资产](#角色动捕与游戏资产) (7)
- [实时与交互式视频生成](#实时与交互式视频生成) (7)
- [视频生成 API 与编排](#视频生成-api-与编排) (4)
- [相关](#相关) (23)
- [相关：Unreal、WebGL 与 3D 资产生成](#相关-unrealwebgl-与-3d-资产生成) (6)
- [相关 Awesome Lists](#相关-awesome-lists) (31)
- [On X](#on-x)

## 展示：代码渲染作品

整条流水线都由「文本模型写代码」驱动的成片。直接 clone 下来读代码，就是最好的教程。

| | | |
|:---:|:---:|:---:|
| <a href="https://www.youtube.com/watch?v=5EoO5413dBY"><img src="https://img.youtube.com/vi/5EoO5413dBY/maxresdefault.jpg" width="300" alt="pdoom 音乐视频"></a> | <a href="https://youtu.be/gcVvRM_P3SM"><img src="https://raw.githubusercontent.com/Vincentwei1021/video-shotcraft/main/workbench/docs/overview.png" width="300" alt="video-shotcraft"></a> | <a href="https://github.com/op7418/guizang-product-video-skill"><img src="https://raw.githubusercontent.com/op7418/guizang-product-video-skill/main/assets/readme/hero.jpg" width="300" alt="归藏产品视频"></a> |
| **[pdoom-video](https://github.com/mexicat/pdoom-video)** · [▶ YouTube 4K](https://www.youtube.com/watch?v=5EoO5413dBY) | **[video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft)** · [▶ 演示](https://youtu.be/gcVvRM_P3SM) | **[归藏 product video skill](https://github.com/op7418/guizang-product-video-skill)** |
| <a href="https://github.com/achimala/dream-loop"><img src="https://raw.githubusercontent.com/achimala/dream-loop/main/assets/vesper-preview.gif" width="300" alt="dream loop 3D"></a> | <a href="https://github.com/xiejunjie524/handdraw-story-video"><img src="https://raw.githubusercontent.com/xiejunjie524/handdraw-story-video/main/examples/soy-milk-at-4am/preview.jpg" width="300" alt="手绘故事视频"></a> | <a href="https://github.com/Alisa0808/vox-director"><img src="https://raw.githubusercontent.com/Alisa0808/vox-director/main/assets/thumbs/football.jpg" width="300" alt="vox director"></a> |
| **[dream-loop](https://github.com/achimala/dream-loop)** | **[handdraw-story-video](https://github.com/xiejunjie524/handdraw-story-video)** | **[vox-director](https://github.com/Alisa0808/vox-director)** |
| <a href="https://www.youtube.com/watch?v=uEB5E67vcPA"><img src="https://img.youtube.com/vi/uEB5E67vcPA/maxresdefault.jpg" width="300" alt="PDoomVideo p5.js 音乐视频"></a> | <a href="https://github.com/gnipbao/story-to-handdrawn-video"><img src="https://raw.githubusercontent.com/gnipbao/story-to-handdrawn-video/main/references/style-examples/standard/colored-pencil-diary.png" width="300" alt="手绘日记视频风格"></a> | <a href="https://github.com/alexgreensh/anidoodle"><img src="https://raw.githubusercontent.com/alexgreensh/anidoodle/main/assets/banner.gif" width="300" alt="anidoodle 代码艺术"></a> |
| **[PDoomVideo](https://github.com/JohnHeibel/PDoomVideo)** · [▶ YouTube](https://www.youtube.com/watch?v=uEB5E67vcPA) | **[story-to-handdrawn-video](https://github.com/gnipbao/story-to-handdrawn-video)** | **[anidoodle](https://github.com/alexgreensh/anidoodle)** |

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [pdoom-video](https://github.com/mexicat/pdoom-video) | 2.4k | TypeScript | Active | 2026-09-28 | 用 **Claude Code 中的 Claude Opus 5.5** 做的生成式 MV：TypeScript + three.js 渲染器、词同步卡拉 OK 排版、确定性帧、真 4K60 导出。 | [▶](https://www.youtube.com/watch?v=5EoO5413dBY) |
| [functional-emotions-video](https://github.com/ledbetterljoshua/functional-emotions-video) | 63 | JavaScript | Active | 2026-09-23 | Claude Opus 5.5 的"绘画感" MV：自研 GPU 笔触渲染器，浏览器里实时播放。 | — |
| [frontier-friday-video](https://github.com/earlvanze/frontier-friday-video) | 1 | JavaScript | Active | 2026-09-28 | 代码渲染 MV：GPT 负责 2D 动态字体，Claude 负责 3D 渲染器。 | [▶](https://youtu.be/ZJCHKxBG43o) |
| [hyperframes-launches](https://github.com/heygen-com/hyperframes-launches) | 579 | HTML | Active | 2026-09-26 | HeyGen 产品发布视频背后的开源 HyperFrames 工程。 | — |
| [NullMotion](https://github.com/blixvip/NullMotion) | 814 | HTML | Active | 2026-09-29 | 发布片预览：成片动效广告与它脱胎而出的黑白 HyperFrames 草稿对照。 | — |
| [dream-loop](https://github.com/achimala/dream-loop) | 1.6k | — | — | — | 用 Claude Code 中的 Claude Opus 5.5 做的梦幻 3D 循环动画。 | — |
| [Battle-of-Austerlitz-Film](https://github.com/WinterArc21/Battle-of-Austerlitz-Film) | 22 | — | — | — | 4–5 分钟的奥斯特里茨战役电影，全部用代码构建：WebGL 渲染器、地形数据、Kokoro 旁白、合成音效。 | — |
| [PDoomVideo](https://github.com/JohnHeibel/PDoomVideo) | 1.9k | — | — | — | pdoom 同曲的另一版 p5.js 演绎（主条目为 mexicat/pdoom-video）——p5.brush 绘画风渲染、无头 Chrome 截帧、FFmpeg 合成。 | [▶](https://youtu.be/8j-hR4fJywU) |

## 渲染引擎（代码→视频）

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [Remotion](https://github.com/remotion-dev/remotion) | 61.2k | TypeScript | Active | 2026-09-30 | 用 React 编程式做视频，代码视频的事实标准。 | — |
| [HyperFrames](https://github.com/heygen-com/hyperframes) | 58.2k | TypeScript | Active | 2026-09-30 | 写 HTML，渲染视频，为 Agent 而生（HeyGen 出品）。 | — |
| [hyperframes-community-skills](https://github.com/heygen-com/hyperframes-community-skills) | 175 | JavaScript | Active | 2026-09-29 | 官方社区维护的 HyperFrames 专项工作流 skills 库。 | — |
| [html-anything](https://github.com/nexu-io/html-anything) | 9.0k | HTML | Active | 2026-09-15 | Agent 化 HTML 编辑器：本地 Agent 写 HTML 直接交付，75 个 skills × 9 种载体。 | — |
| [manim](https://github.com/3b1b/manim) | 94.4k | Python | Active | 2026-09-09 | 数学讲解视频动画引擎（3Blue1Brown 同款）。 | [▶](https://www.youtube.com/watch?v=rbu7Zu5X1zI) |
| [FFmpeg](https://github.com/FFmpeg/FFmpeg) | 64.7k | C | Active | 2026-09-30 | 所有视频流水线最终都会调用的通用音视频工具箱。 | — |
| [Shotcut](https://github.com/mltframework/shotcut) | 15.3k | C++ | Active | 2026-09-30 | 跨平台开源非线性视频编辑器。 | — |
| [html-video](https://github.com/nexu-io/html-video) | 4.6k | HTML | Active | 2026-06-21 | 面向编程 Agent 的本地出片：HTML/CSS/数据 → 真 MP4。 | — |
| [remotion-template-three](https://github.com/remotion-dev/template-three) | 110 | TypeScript | Active | 2026-09-29 | Remotion + React Three Fiber 模板：3D 场景渲染为视频帧。 | — |
| [Graphite](https://github.com/GraphiteEditor/Graphite) | 27.4k | Rust | Active | 2026-09-29 | 开源 2D 矢量/栅格编辑器，节点式程序动画，GPU 加速。 | — |
| [lottie-web](https://github.com/airbnb/lottie-web) | 32.1k | JavaScript | Active | 2025-09-01 | 原生渲染 After Effects 动画：JSON 驱动，Agent 可写格式。 | [▶](https://www.youtube.com/watch?v=5XMUJdjI0L8) |
| [react-three-fiber](https://github.com/pmndrs/react-three-fiber) | 32.6k | TypeScript | Active | 2026-09-30 | React 的 Three.js 渲染器：3D 场景即 React 组件，可与 Remotion 组合做 3D 视频。 | — |
| [p5.js](https://github.com/processing/p5.js) | 24.1k | JavaScript | Active | 2026-09-30 | 创意编程工具包：sketch → canvas 帧 → CCapture 录视频。pdoom-video 的底座。 | — |
| [Diffusion Studio editor](https://github.com/diffusionstudio/editor) | 3.2k | TypeScript | Active | 2026-09-29 | 为 Agent 打造的开源视频编辑器：剪辑变代码，代码变视频。 | [▶](https://youtu.be/HEfHFsfGXjs) |
| [animspark](https://github.com/animspark/animspark) | 32 | TypeScript | Active | 2026-09-26 | 编程 Agent 可以直接"写电影"的开源视频引擎：影片格式 + 帧级精确渲染。 | — |
| [presentation-ai](https://github.com/allweonedev/presentation-ai) | 3.0k | TypeScript | Active | 2026-06-05 | 开源 AI 演示文稿生成器（Gamma 替代）。代码驱动幻灯片→视频导出。 | [▶](https://www.youtube.com/watch?v=UUePLJeFqVQ) |
| [codex-slides](https://github.com/nexu-io/codex-slides) | 922 | TypeScript | Active | 2026-07-21 | Codex 内的开源 AI 幻灯片工作室：45 模板、73 风格、PPTX/PDF 导出。 | — |
| [presenton](https://github.com/presenton/presenton) | 10.9k | TypeScript | Active | 2026-09-30 | 开源 AI 演示文稿生成器：自托管、BYOK、MCP server、PPTX/PDF 导出。 | — |
| [Ultimate-AI-Media-Generator-Skill](https://github.com/ZeroLu/Ultimate-AI-Media-Generator-Skill) | 92 | MDX | Active | 2026-09-08 | 开源 AI 媒体 Skill：图像、视频、音频，通过 CyberBara API。支持 Seedance、Sora、Kling。 | — |
| [manim-mcp](https://github.com/paulnegz/manim-mcp) | 20 | Python | Active | 2026-02-25 | 文本→视频动画：描述→代码→渲染 MP4。CLI、Agent 模式、MCP server。 | — |
| [Motion-Canvas](https://github.com/motion-canvas/motion-canvas) | 19.2k | TypeScript | — | — | 代码驱动的动画框架（生成器函数、缓动），用于解说类视频。 | — |
| [editly](https://github.com/mifi/editly) | 5.5k | TypeScript | Moderate | 2025-05-12 | Node.js 编程式视频编辑器：JSON/JS 驱动多轨剪辑，图层、转场、叠加。 | [▶](https://youtu.be/LNeclLkxUEY) |
| [MotionAgent](https://github.com/leoisufa/MotionAgent) | 5 | Python | Active | 2025-10-22 | ICCV 2025：运动场 Agent + 光流的细粒度可控视频生成。 | [▶](https://www.youtube.com/watch?v=O9WW2UpXsAI) |
| [claude-code-video-toolkit](https://github.com/digitalsamba/claude-code-video-toolkit) | 2.2k | Python | Active | 2026-09-28 | Claude Code 的 AI 原生视频制作工作台：skills、命令、模板、品牌配置、转场、项目生命周期。 | — |
| [motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | 35 | JavaScript | Active | 2026-09-30 | 代码做出 showreel 级动效 + 每条视频的原创配乐。 | — |
| [paint-video-skill](https://github.com/nzl153/paint-video-skill) | 1 | JavaScript | Active | 2026-09-30 | 代码做手绘动画短片和音乐视频：水彩、水墨、蜡笔。 | — |
| [JIZURA](https://github.com/852wa/JIZURA) | 1.6k | HTML | Active | 2026-09-29 | 浏览器端文字 PV 自动生成器：歌词 + 音频 → 随机组合 860+ 部件 → 多风格视频。MP4/PNG 导出 + AE 插件。 | [▶](https://852wa.github.io/JIZURA/) |
| [golive-skill](https://github.com/mikehasa/golive-skill) | 1.2k | TypeScript | Active | 2026-09-29 | 代码生成应用一键部署：实时预览→视频采集管线。 | — |
| [opus-video-prompts](https://github.com/joeseesun/opus-video-prompts) | 189 | — | Active | 2026-09-27 | Opus 5.5 代码渲染视频 Prompt 合集：18 份 prompt + 54 案例。 | [▶](https://www.bilibili.com/video/BV1qihf6rE6f) |
| [Revideo](https://github.com/redotvideo/revideo) | — | TypeScript | — | — | Motion Canvas 分支转为库：渲染 API、模板和自动化管线，用于程序化视频。 | — |
| [Diffusion-Studio-Core](https://github.com/diffusionstudio/core) | 1.2k | TypeScript | — | — | 浏览器视频合成引擎，基于 WebCodecs（无 wasm/ffmpeg）；用代码编辑视频。 | — |
| [text-to-lottie](https://github.com/diffusionstudio/lottie) | 5.5k | TypeScript | — | — | 用 Claude Code/Codex 生成生产级 Lottie 动画。Text-to-Lottie 框架，带实时预览播放器。 | — |
| [AnimTOON](https://github.com/srk0102/AnimTOON) | 20 | Python | — | — | AI 模型将任意 SVG 动画化为 Lottie 动画。为 LLM 生成设计的紧凑纯文本动画格式。 | — |
| [handanim](https://github.com/subroy13/handanim) | 48 | Python | Moderate | 2025-06 | Python 白板风格手绘动画库，用素描风格笔触和手写文字创建教育视频。 | — |
| [pytoon-dev](https://github.com/nitinthewiz/pytoon-dev) | 150 | Python | Moderate | 2025-03 | Python 动画库，基于机器学习音频分析自动生成卡通角色口型和表情同步动画。 | [▶](https://www.youtube.com/watch?v=Sg2OBBNwF-k) |
| [ai-video-pipeline](https://github.com/shenyuhao1/ai-video-pipeline) | 1 | Python | Moderate | 2026-05 | AI 视频生成流水线：Dify 工作流 + Manim 动画 + TTS 旁白 + Whisper 字幕 + FFmpeg 合成，含 GUI。 | — |
| [ManimCommunity/manim](https://github.com/ManimCommunity/manim) | 41.1k | Python | Active | 2026-09-29 | 社区维护版 manim：API 更稳、文档更全、插件生态更广——大多数 skill 以它为目标。 | — |
| [Manim.js](https://github.com/JazonJiao/Manim.js) | 454 | JavaScript | Active | 2026-08-22 | 用 JavaScript（p5.js）复刻 3Blue1Brown 的 manim——浏览器里跑的数学动画。 | — |
| [anidoodle](https://github.com/alexgreensh/anidoodle) | 834 | — | Active | 2026-09-28 | 以代码书写的艺术与动画：插画、循环动效、交互式网页艺术、发布视频。 | — |

## AI 视频编辑 Agent

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [palmier-pro](https://github.com/palmier-io/palmier-pro) | 14.5k | — | — | — | 为 AI 而生的 macOS 视频编辑器。 | — |
| [jianying-editor-skill](https://github.com/luoluoluo22/jianying-editor-skill) | 3.8k | — | — | — | Agent 自动操作剪映完成剪辑。[▶ B站演示](https://www.bilibili.com/video/BV1hLzCBzEDS) | [▶](https://www.bilibili.com/video/BV1hLzCBzEDS) |
| [FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) | 3.5k | — | — | — | AI 视频剪辑 Agent：手动剪辑 → 意图驱动的智能导演。 | — |
| [chengfeng-videocut-skills](https://github.com/Agentchengfeng/chengfeng-videocut-skills) | 3.0k | — | — | — | 用 Claude Code Skills 做的视频剪辑 Agent。 | — |
| [OpenChatCut](https://github.com/0xsline/OpenChatCut) | 2.2k | — | — | — | 本地优先的对话式 AI 剪辑器：专业多轨时间线 + Agent Skills。 | — |
| [VideoAgent](https://github.com/HKUDS/VideoAgent) | 1.9k | — | — | — | [EMNLP 2026] 视频理解、剪辑与再创作一体的 Agent 框架。 | — |
| [open-edit](https://github.com/veedstudio/open-edit) | 1.6k | — | — | — | Agent 驱动的剪辑流水线：字幕、动效、幻灯片、剪辑与渲染。 | — |
| [CutClaw](https://github.com/GVCLab/CutClaw) | 980 | — | — | — | 音乐卡点驱动的 Agent 长视频剪辑。 | — |
| [ai-video-editor](https://github.com/MartinDelophy/ai-video-editor) | 881 | — | — | — | 本地优先：创作者与 AI Agent 编辑同一条真实时间线。 | [▶](https://youtu.be/bqKhpPPa-qo) |
| [clipify](https://github.com/louisedesadeleer/clipify) | 583 | — | — | — | Claude Code skill：长视频 → 社交切片，自动找高光、重构 9:16。 | — |
| [chatgpt-video-editing-skills](https://github.com/Jaycheng1103/chatgpt-video-editing-skills) | 574 | — | — | — | 用 ChatGPT／Codex 按八大步骤完成可验证的短影音剪辑。 | — |
| [velocut](https://github.com/open-ribbi/velocut) | 454 | — | — | — | 浏览器里的 AI 原生本地剪辑器：Rust/WASM + WebGPU。 | — |
| [ghost-editor](https://github.com/kurbaitaev/ghost-editor) | 66 | — | — | — | 口播 Reels 的 AI 剪辑器：7 种风格、人脸安全字幕、动效场景。 | — |
| [claude-video](https://github.com/bradautomates/claude-video) | 17.9k | — | — | — | Claude Code Skill：观看并分析视频文件，提取关键帧，生成摘要。 | — |
| [Youtube-clipper-skill](https://github.com/op7418/Youtube-clipper-skill) | 2.2k | — | — | — | 下载 YouTube、AI 语义章节、切片、双语字幕、烧录。 | — |
| [viral-x-posts](https://github.com/shannhk/viral-x-posts) | 13 | — | — | — | Claude Code skill：23 个爆款 X/Twitter 帖子公式，视频内容分发。 | — |
| [video-ai-analysis](https://github.com/yangchen0991/video-ai-analysis) | 16 | — | — | — | AI 辅助影视分析：逐镜头拆解、场景检测、视觉语法。 | — |
| [JoyAI-Video-Edit](https://github.com/jd-opensource/JoyAI-Video-Edit) | 1.9k | — | — | — | 实时指令驱动视频剪辑：720p 30.19 FPS，自回归扩散，风格迁移。 | — |
| [hermes-video-editing](https://github.com/argus-metis/hermes-video-editing) | 5 | — | — | — | 专业视频剪辑 Skill：AI 字幕、去静音、场景检测、稳定、智能裁切。 | — |
| [video-analytics-agent](https://github.com/AgenticAI-Ind/video-analytics-agent) | 0 | — | — | — | 企业级视频分析 Agent：自动转录、场景检测、目标追踪。 | — |
| [SceneDetect](https://github.com/Breakthrough/PySceneDetect) | 5.2k | — | — | — | 视频场景切换检测：内容感知与阈值，CLI + Python API。 | — |
| [Kinocut](https://github.com/KyaniteLabs/kinocut) | 193 | — | — | — | 带护栏的视频剪辑 MCP server。FFmpeg、HyperFrames、质量门控、Shorts/Reels 再利用。 | — |
| [mcp-video](https://github.com/ipythonist/mcp-video) | 4 | — | — | — | 视频智能 MCP server：关键帧提取、转录、分析，支持 1000+ 站点。 | — |
| [ai-video-editor-review](https://github.com/vidio-research/ai-video-editor-review) | 2 | — | — | — | AI 视频剪辑技术协作开放综述（2025-2026）。 | — |
| [chatcut](https://github.com/ArtCog/chatcut) | — | Python | — | — | 一条命令把原始口播素材变成成品视频——转录→剪切停顿和口误→字幕→动效→调色→渲染。 | — |
| [video-clip-agent](https://github.com/neopen/video-clip-agent) | 39 | Python | — | — | AI 视频剪辑智能体：分析画面、音频、情绪，自动裁剪、筛选片段、卡点、加字幕背景音乐。 | — |
| [Director](https://github.com/video-db/Director) | 1.5k | — | — | — | 视频 Agent 框架：搜索/编辑/编译/生成。仓库直称「Director」。 | [▶](https://www.youtube.com/watch?v=Dncn_0RWrro) |
| [Monet](https://github.com/Monet-AI-Editor/Monet) | 116 | — | — | — | 编程 Agent 原生视频编辑器：Timeline + Codex/Claude Code + MCP + Remotion。 | — |
| [opencut](https://github.com/floomhq/opencut) | 7 | TypeScript | Active | 2026-09-29 | 基于 Remotion 的开源视频编辑器——浏览器端、React 驱动的时间线。 | — |
| [auto-video-editor](https://github.com/benpiper/auto-video-editor) | 12 | Python | Active | 2026-08-25 | 自动检测并移除视频中的沉默、口头禅和静止帧——Web UI + REST API。 | — |
| [Clypra](https://github.com/AIEraDev/Clypra) | 3.3k | Rust | Active | 2026-09-30 | Rust + Tauri v2 + React 19 的硬件加速视频编辑器，帧交付低于 10ms。 | — |
| [vanta](https://github.com/itsjwill/vanta) | 132 | TypeScript | Active | 2026-07-26 | 基于 Remotion 的开源 AI 视频引擎：声音克隆、AI 数字人、动态字幕。 | — |
| [dissect](https://github.com/0xpratzyy/dissect) | 24 | — | Active | 2026-10-01 | 把任意视频（YouTube/TikTok/Reels/X）逆向拆解成可复用的创作蓝图。 | — |
| [remocn-studio](https://github.com/Remocn/remocn-studio) | 149 | TypeScript | Active | 2026-10-01 | Agent 原生视频编辑器：一句话进，成片出。 | — |
| [short-video-maker (mushigaite)](https://github.com/mushigaite/short-video-maker) | 68 | Python | Active | 2026-10-05 | 免费开源：把 YouTube 长视频转成爆款短视频。 | — |
| [OpenCardboard](https://github.com/rakesh0x/OpenCardboard) | 57 | TypeScript | Active | 2026-10-04 | 本地优先的对话式 AI 剪辑器——素材不出本机。 | — |

## Agentic 生产系统与短视频流水线

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | 127.1k | — | — | — | 主题/关键词 → 高清短视频，LLM + 自动化工作流，品类之王。 | — |
| [OpenMontage](https://github.com/calesthio/OpenMontage) | 64.8k | — | — | — | 开源 Agent 化制片系统：12 条流水线、100+ 工具、700+ agent skills。 | — |
| [MoneyPrinterV2](https://github.com/FujiwaraChoki/MoneyPrinterV2) | 32.0k | — | — | — | 自动化网上赚钱流程。 | [▶](https://youtu.be/wAZ_ZSuIqfk) |
| [Pixelle-Video](https://github.com/ATH-MaaS/Pixelle-Video) | 28.5k | — | — | — | AI 全自动短视频引擎。 | [▶](https://www.bilibili.com/video/BV1WzyGBnEVp) |
| [hypit](https://github.com/hypit-ai/hypit) | 19.9k | — | — | — | 用 AI Agent 克隆任意爆款视频：换脸、换文案、换 B-roll，整套流程。 | — |
| [Toonflow](https://github.com/HBAI-Ltd/Toonflow-app) | 16.6k | — | — | — | 无限画布 + AI Agent + 可视化工作流：图像/视频生成、智能分镜、短剧创作。 | — |
| [huobao-drama](https://github.com/chatfire-AI/huobao-drama) | 15.6k | — | — | — | 火宝短剧：一句话生成完整短剧，剧本到成片全自动化。 | — |
| [waoowaoo](https://github.com/waooAI/waoowaoo) | 14.3k | — | — | — | 工业级全流程 AI 影视生产平台。 | — |
| [ViMax](https://github.com/HKUDS/ViMax) | 12.5k | — | — | — | Agent 化视频生成：导演、编剧、制片、生成器 All-in-One。 | — |
| [OpenCreator](https://github.com/krillinai/OpenCreator) | 12.5k | — | — | — | 原 KrillinAI：Codex 驱动的创作者 AI 工作台。 | — |
| [ShortGPT](https://github.com/RayVentura/ShortGPT) | 8.0k | — | — | — | YouTube Shorts / TikTok 频道自动化 AI 框架。 | [▶](https://youtu.be/hpoSHq-ER8U) |
| [MoneyPrinterPlus](https://github.com/ddean2009/MoneyPrinterPlus) | 7.2k | — | — | — | 批量生成短视频并自动发布到抖音/快手/小红书/视频号。 | [▶](https://www.bilibili.com/video/BV16VVGefEp1) |
| [dramaclaw](https://github.com/dramaclaw/dramaclaw) | 6.6k | — | — | — | 通用 AIGC 视频引擎：一条流水线，剧本到成片。 | [▶](https://www.bilibili.com/video/BV1iQV26cE4S) |
| [Jellyfish](https://github.com/Forget-C/Jellyfish) | 6.5k | — | — | — | AI 短剧端到端工作台：剧本 → 结构化分镜 → 成片。 | — |
| [ArcReel](https://github.com/ArcReel/ArcReel) | 5.3k | — | — | — | 小说/剧本 → 资产、分镜、视频与剪映草稿，跨镜头一致性 + 费用追踪。 | — |
| [youtube-automation-agent](https://github.com/darkzOGx/youtube-automation-agent) | 4.1k | — | — | — | AI Agent 7×24 运营 YouTube 频道：创作、优化、发布。 | — |
| [ai-podcast-generator](https://github.com/gordonho/ai-podcast-generator) | 0 | — | — | — | AI 播客视频生成器：脚本→TTS→数字人动画→视频输出。 | — |
| [AiToEarn](https://github.com/yikart/AiToEarn) | 26.6k | — | — | — | 全栈 AI 内容增长与变现：视频创作+分发+分析。 | [▶](https://www.youtube.com/watch?v=5041jEKaiU8) |
| [screenplay-agent](https://github.com/596600892/screenplay-agent) | 0 | — | — | — | AI 剧本写作与视频场景生成：一句话到好莱坞格式剧本 + MoneyPrinterTurbo 桥接。 | — |
| [script-to-storyboard](https://github.com/lookme2012/script-to-storyboard) | 14 | — | — | — | AI 辅助剧本+分镜：8 步工作流、多 LLM、Electron 桌面应用。 | — |
| [ClipForge-CLI](https://github.com/gitstq/ClipForge-CLI) | 0 | — | — | — | 轻量终端 AI 短视频脚本生成器：7 种风格、分镜、多格式导出、TUI 面板。 | — |
| [ai-video-generation-pipeline](https://github.com/SainathPattipati/ai-video-generation-pipeline) | 8 | — | — | — | 端到端 AI 视频：概念→脚本→分镜→一致角色→视频。 | — |
| [awesome-generative-ai-apps](https://github.com/Anil-matcha/awesome-generative-ai-apps) | 3.4k | — | — | — | 50+ 开源 AI SaaS 模板：视频工具、头像生成、一键部署。 | [▶](https://www.youtube.com/watch?v=X_kbyQyhgmI) |
| [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) | 140.3k | — | — | — | 100+ AI Agent 与 Skills：梗图生成器、音乐、播客、视频分析 Agent。 | — |
| [Free-AI-Social-Media-Scheduler](https://github.com/Korexer/Free-AI-Social-Media-Scheduler) | — | — | — | — | 免费 AI 社媒定时器：最优时间自动发布视频。 | — |
| [vox-ai-motion-graphics-generator](https://github.com/Anil-matcha/vox-ai-motion-graphics-generator) | 242 | Python | High | 2025-09 | 将任意主题转化为 Vox 风格纸拼贴解说视频，自动生成脚本、动画、旁白和字幕 | [▶](https://www.youtube.com/watch?v=chK_pnV1wqQ) |
| [aimv-studio](https://github.com/shaozheng0503/aimv-studio) | 20 | Python | Active | 2026-09-10 | 多 Agent MV 生成系统：AI 作曲、写词、生成画面、剪辑成片。 | — |
| [bang-story](https://github.com/bangtutorial/bang-story) | 71 | TypeScript | Active | 2026-10-02 | 桌面应用（印尼语）：故事点子 → AI 生成完整 YouTube 视频（bang-motion 作者出品）。 | — |

## MCP 与控制层

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [mcp-for-blender](https://github.com/ahujasid/mcp-for-blender) | 29.7k | — | — | — | 用任意 LLM 控制 Blender 3D 的社区插件。[▶ 演示](https://www.youtube.com/watch?v=I29rn92gkC4) | [▶](https://www.youtube.com/watch?v=I29rn92gkC4) |
| [scenario-labs/skills](https://github.com/scenario-labs/skills) | 898 | — | — | — | 让任意 AI Agent 产出可用的图像、视频、音频与 3D。 | — |
| [blend-ai](https://github.com/HoldMyBeer-gg/blend-ai) | 151 | — | — | — | Blender MCP server：186 个建模、材质、渲染等工具，由 Claude / Cursor 驱动。 | — |
| [blender-mcp-bridge](https://github.com/seehiong/blender-mcp-bridge) | 65 | — | — | — | 通过 MCP 自动化 Blender 建模：93 个工具，含雕刻、建筑/MEP、材质。 | — |
| [blender-mcp-pro](https://github.com/youichi-uda/blender-mcp-pro) | 31 | — | — | — | 100+ 工具的 MCP server：灯光、修改器、动画、着色器节点、几何节点。 | — |
| [Blender-Extension](https://github.com/suryansh00001/Blender-Extension) | 25 | — | — | — | Blender 内置 LLM 助手：自然语言直接生成 3D。 | — |
| [mcp-blender](https://github.com/RFingAdam/mcp-blender) | 19 | — | — | — | 218 个工具：3D 建模、AI 生成与 MSFS 内容创作。 | — |
| [video-generation-mcp](https://github.com/ricleedo/video-generation-mcp) | 0 | — | — | — | 视频生成 MCP server：文生视频、图生视频，通过 Kling/MiniMax/fal.ai API。 | — |
| [xai-mcp-server](https://github.com/joemccann/xai-mcp-server) | 1 | — | — | — | xAI Grok API 的 MCP 服务器，含视频生成能力。 | — |
| [browser-automation](https://github.com/howar31/browser-automation) | 0 | — | — | — | 驱动真实无头浏览器的 Claude Code Skill（Puppeteer + Playwright）——截图、网络拦截、CDP 调试。 | — |
| [video-audio-mcp](https://github.com/misbahsy/video-audio-mcp) | 87 | Python | Medium | 2025-07 | 基于 FFmpeg 的视频/音频编辑 MCP 服务器，支持格式转换、裁剪、叠加和转场 | — |
| [ffmpeg-skill](https://github.com/MastroMimmo/ffmpeg-skill) | 21 | Python | Medium | 2025-08 | Claude Code 自然语言视频编辑技能，18 个命令覆盖裁剪/合并/压缩/字幕/GIF/水印 | — |
| [short-video-maker](https://github.com/gyoridavid/short-video-maker) | 1.4k | TypeScript | Active | 2026-09-20 | 短视频生成器：脚本 → TTS 配音 → 自动字幕 → 背景素材 → MP4。 | — |

## 视频技能：产品影片、宣传片与解说视频

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | 10.5k | TypeScript | Active | 2026-09-28 | Claude Code & Codex 的电影感产品视频：基于 Remotion，152 张镜头配方卡、209 个动效预设。[▶ 演示 1](https://youtu.be/gcVvRM_P3SM) · [▶ 演示 2](https... | [▶](https://youtu.be/gcVvRM_P3SM) |
| [pixel2motion](https://github.com/nolangz/pixel2motion) | 2.4k | Python | Active | 2026-08-21 | 位图 Logo → 流畅 SVG 动画、HTML 动效 Demo、GIF/视频预览。 | — |
| [anything2explainer](https://github.com/Vincentwei1021/anything2explainer) | 2.3k | TypeScript | Active | 2026-09-18 | 输入任意主题，输出带旁黑的黑板风解说视频。 | — |
| [lanshu-create-ai-presenter-video](https://github.com/cclank/lanshu-create-ai-presenter-video) | 2.4k | Python | Active | 2026-09-27 | 不绑供应商的 Codex skill：脚本 → 可验收的 AI 数字人口播视频。 | — |
| [video-talkcraft](https://github.com/Vincentwei1021/video-talkcraft) | 1.4k | HTML | Active | 2026-09-22 | 把 Claude Code / Codex 变成旁白驱动解说视频的动效设计工作室。 | — |
| [hyperframes-student-kit](https://github.com/nateherkai/hyperframes-student-kit) | 1.2k | HTML | Active | 2026-09-28 | 用 Codex / Claude Code 剪视频、Reels 和 Shorts：14 个 skills、逐字稿驱动剪辑、406 个动效预设。 | — |
| [video-spec-builder](https://github.com/feicaiclub/video-spec-builder) | 1.0k | JavaScript | Active | 2026-05-18 | 把"我想做个视频"逼成精确到秒的分镜脚本 `video-spec.md`，再交给 HyperFrames 渲染，一条命令安装。 | — |
| [onetake](https://github.com/feitangyuan/onetake) | 1.8k | Python | Active | 2026-09-29 | 一镜到底动效片：每个节拍从上一个节拍生长出来，全程不切镜头。 | — |
| [capcut-cli](https://github.com/renezander030/capcut-cli) | 833 | JavaScript | Active | 2026-09-28 | 任意 LLM Agent 可驱动的剪映/CapCut CLI：零依赖，JSON 输入输出。 | [▶](https://www.youtube.com/watch?v=cl8SP3PjspQ) |
| [pyJianYingDraft](https://github.com/GuanYixuan/pyJianYingDraft) | 4.5k | Python | Active | 2026-09-26 | 轻量 Python 库生成和导出剪映草稿，适配自动化剪辑管线。 | — |
| [pyCapCut](https://github.com/GuanYixuan/pyCapCut) | 687 | Python | Active | 2026-09-30 | pyJianYingDraft 的 CapCut 版：Python 生成导出 CapCut 草稿。 | — |
| [bang-motion](https://github.com/bangtutorial/bang-motion) | 568 | HTML | Active | 2026-09-15 | 浏览器动效：片头、宣传片、bumper、动态字体、5 种解说风格。 | — |
| [Orkas-VideoStudio](https://github.com/Orkas-AI/Orkas-VideoStudio) | 497 | TypeScript | Active | 2026-09-22 | 把编程 Agent 变成视频工作室：自然语言描述，Agent 写时间线并渲染。 | — |
| [motion-video-kit](https://github.com/echris6/motion-video-kit) | 1.1k | Python | Active | 2026-09-28 | 带独立评审循环（critic loop）的高端商务视频 Claude Code 技能包。 | — |
| [llm-video-maker](https://github.com/GoldLegendW80/llm-video-maker) | 26 | JavaScript | Active | 2026-06-17 | 一句 prompt → 成片 MP4，适配 Claude Code / Cursor / Codex / Windsurf。 | — |
| [brand-motion-design-skill](https://github.com/ouerf-man/brand-motion-design-skill) | 30 | JavaScript | Active | 2026-09-27 | 用 HyperFrames 以代码做出 showreel 级品牌动效（发布片、宣传片、预告）。 | — |
| [claude-promo-video](https://github.com/smit-vanani/claude-promo-video) | 15 | JavaScript | Active | 2026-07-16 | 网址 → 高级感、卡点的产品宣传片（Remotion）。 | — |
| [motion-skills](https://github.com/iart-ai/motion-skills) | 729 | HTML | Active | 2026-09-23 | 50 个开源 skills，教会你的编程 Agent 做动效、动画与视频。 | — |
| [hyperframes-motion-director](https://github.com/geekjourneyx/hyperframes-motion-director) | 450 | JavaScript | Active | 2026-07-26 | 中文优先的 HyperFrames 动效视频产线：文章、产品、网站一键成片。 | — |
| [remotion-video-skill](https://github.com/wshuyi/remotion-video-skill) | 384 | Python | Active | 2026-01-25 | 用 Remotion 框架编程式做视频的 Claude Code skill。 | — |
| [super-video-maker-skill](https://github.com/Bomx/super-video-maker-skill) | 305 | Python | Active | 2026-08-09 | 一个 skill 调度多引擎：HeyGen 数字人、Seedance B-roll、OpenAI 图像、Remotion 与 HyperFrames。 | — |
| [marketing-studio](https://github.com/ucsandman/marketing-studio) | 248 | JavaScript | Active | 2026-09-06 | 用 Remotion 做产品发布物料，带受控 dry-run 的审核与分发流程。 | — |
| [erduo-broll-loop-engineering](https://github.com/erduo1998-cell/erduo-broll-loop-engineering) | 205 | TypeScript | Active | 2026-09-21 | SRT 驱动的双后端 B-roll Agent Skill：自动路由 HyperFrames / Remotion，内置 152 张 Shotcraft 镜头卡。 | — |
| [film-studio-skills](https://github.com/machina-exm/film-studio-skills) | 143 | — | Active | 2026-08-14 | 7 个可安装 skills，复刻 200 万美元级 AI 视频项目的产线：剧本到定剪。 | — |
| [claude-motion-design](https://github.com/howseen-ai/claude-motion-design) | 282 | — | — | — | 纯代码做动效设计视频：HTML + Playwright + ffmpeg，不用 After Effects。 | — |
| [Claude-Code-Video-Toolkit](https://github.com/wilwaldon/Claude-Code-Video-Toolkit) | 88 | — | — | — | Claude Code 做视频的 skills、MCP server 与工具集（Remotion 等）。 | — |
| [super-prototyping](https://github.com/ReScienceLab/super-prototyping) | 87 | — | — | — | 两小时从点子到 Logo、产品、品牌与发布片，面向 AI Agent 的产品验证系统。 | — |
| [vox-director](https://github.com/Alisa0808/vox-director) | 2.2k | — | — | — | 一个主题 → 完整的 Vox 风格纸拼贴解说/广告视频，端到端。 | — |
| [guizang-product-video-skill](https://github.com/op7418/guizang-product-video-skill) | 697 | — | — | — | 归藏的 Skill：复用真实产品组件和设计语言，代码做软件更新宣传片——分镜、原创配乐、音效、渲染。 | — |
| [motion-graphics-skill](https://github.com/AidenChenCode/motion-graphics-skill) | 0 | — | — | — | Claude Code Skill：把品牌简报（可选参考视频）变成成品动效 MP4。 | — |
| [video-production-skills](https://github.com/Pluviobyte/video-production-skills) | 666 | — | Active | 2026-07-14 | 可复用的 AI 视频制作 skills 库：创作、复刻、动效设计、片头。 | — |
| [reelbench-skills](https://github.com/eternityspring/reelbench-skills) | 850 | — | Active | 2026-09-21 | AI 视频相关的学习笔记与工具 skill。 | — |
| [simon-skills](https://github.com/trustfuture/simon-skills) | 324 | — | Active | 2026-09-24 | 不露脸做视频账号的 skill 合集：调查长片 + 手绘白板讲解视频，一句选题出片。 | — |
| [editor-pro-max](https://github.com/Hainrixz/editor-pro-max) | 257 | TypeScript | Active | 2026-03-26 | Remotion + Claude Code 构建的 AI 视频编辑器：用描述出片。 | — |
| [one-prompt-video-skills](https://github.com/huangbai-AI/one-prompt-video-skills) | 86 | — | Active | 2026-09-29 | 一句话生成完整口播视频：写稿、口播数字人、B-roll、HyperFrames 合成、抽帧检查（Claude Code Skills）。 | — |
| [adu-motion-video](https://github.com/adunext/adu-motion-video) | 168 | — | Active | 2026-09-28 | 阿杜与 Opus 5.5 的动画动效模板 Skill：选模板和风格，把口播与素材剪成视频，内置 11,028 个精选 Lottie 动画。 | — |
| [whiteboard-video](https://github.com/Cuongyd196/whiteboard-video) | 27 | — | Active | 2026-09-30 | 主题、剧本或 SRT → 完整白板手绘视频：Agent 写稿、绘制、配音。 | — |
| [nd-video-studio](https://github.com/vakovalskii/nd-video-studio) | 20 | — | Active | 2026-09-29 | HTML 出解说视频（HyperFrames → MP4）：AI 旁白、配乐与混音，Claude Code skill。 | — |
| [xilo-opus-video](https://github.com/Kianzzz/xilo-opus-video) | 26 | — | Active | 2026-09-28 | 用 Claude Opus 5.5 写代码做视频：先给三个方案和预览，确认后逐帧渲染成片（Canvas/WebGL/Three.js/Remotion/HyperFrames）。 | — |
| [livecanvas](https://github.com/pengchujin/livecanvas) | 417 | Swift | Active | 2026-09-30 | 一句话做成有封面、有动画的 Live 图（实况照片/动态封面）。 | — |
| [motion-video-skill](https://github.com/unclejobs-ai/motion-video-skill) | 102 | Python | Active | 2026-10-02 | Claude Code skill（韩语）：30–90 秒动效视频的制作流程与逐步检查 harness。 | — |
| [motionmaxxing](https://github.com/Tejashmakwana/motionmaxxing) | 75 | JavaScript | Active | 2026-10-06 | 给动效"医美"：把 AI 糙视频打磨成有真正动效设计的成片的 Agent skill。 | — |
| [kar-plain](https://github.com/Burntgogi/kar-plain) | 42 | HTML | Active | 2026-10-05 | 紧凑的 Codex/Claude skill（韩/英）：用文章、图解、网页、视频四种格式讲解主题，Karpathy 推文启发。 | — |
| [ecommerce-video-skills](https://github.com/xianyu110/ecommerce-video-skills) | 35 | Python | Active | 2026-10-04 | 12 个电商短视频 Agent Skills：3秒钩子、卖点分镜、图生视频提示词、edge-tts 配音、字幕花字、ffmpeg 自动成片，导出抖音/TikTok Shop/视频号格式。 | — |
| [mortiflix-oss](https://github.com/GTKottman/mortiflix-oss) | 242 | JavaScript | Active | 2026-10-05 | 本机的动效设计工作室：Claude 逐步制作视频，每个阶段由你审批。 | — |

## 视频技能：短剧、故事与 Recap

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [drama-skills](https://github.com/zenstory-ai/drama-skills) | 2.6k | — | — | — | AI 短剧/漫剧创作合集：剧本、角色资产、分镜 storyboard、图片/视频提示词、审查，适配 Claude Code 与 Codex。 | — |
| [video-recap-skills](https://github.com/zenstory-ai/video-recap-skills) | 554 | — | — | — | 视频 → 中文影视解说：场景检测、ASR、VLM、文案、渲染一条龙。 | — |
| [handdraw-story-video](https://github.com/xiejunjie524/handdraw-story-video) | 775 | — | — | — | 手绘故事视频 Skill：把任意故事变成带旁白的手绘动画短片。 | — |
| [Open-AI-Micro-Drama-Generator](https://github.com/Anil-matcha/Open-AI-Micro-Drama-Generator) | 518 | Python | — | — | AI 短剧/微剧视频生成器：多 Agent 流水线（编剧→分镜→帧→视频）把任何创意变成完整短剧。 | — |
| [story-to-handdrawn-video](https://github.com/gnipbao/story-to-handdrawn-video) | 2.2k | — | Active | 2026-09-22 | Agent skill：中文故事文案或有序图片 → 手绘日记漫动画视频。 | — |
| [html-anime](https://github.com/blixvip/html-anime) | 16 | — | Active | 2026-09-27 | HTML 动画番生成器：一句场景出分镜表，交给 Claude/Codex/Cursor 渲染（NullMotion 作者出品）。 | — |
| [cinematic-film](https://github.com/minosdevs/cinematic-film) | 21 | TypeScript | Active | 2026-09-30 | Claude Code skill：任意主题 → Remotion + three.js 电影感动画影片。 | — |
| [vocaloid-style-mv-pipeline](https://github.com/EGSECDA/vocaloid-style-mv-pipeline) | 52 | JavaScript | Active | 2026-10-04 | Vocaloid 风手绘歌词 MV 的产线与 Claude Code skill。 | — |
| [Muse-animated-short-film](https://github.com/sonlovinbot/Muse-animated-short-film) | 31 | — | Active | 2026-10-03 | 越南语 skill：在 Muse AI 上做动画短片——从点子到 MP4：角色、剧本、关键帧。 | — |

## manim 与数学教育视频

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [manim-skill](https://github.com/Yusuke710/manim-skill) | 165 | — | — | — | manim 的 SKILL.md：编程 Agent 自主规划场景并编写动画代码。 | — |
| [Math-To-Manim](https://github.com/HarleyCoops/Math-To-Manim) | 2.7k | — | — | — | 多管线 Manim 生成（Claude/Gemini/Kimi K2.5），55+ 示例覆盖物理、数学、CS。 | — |
| [3brown1blue](https://github.com/AmitSubhash/3brown1blue) | 36 | — | — | — | Claude Code 的第一性原理 manim skill：从零做数学动画，论文讲解风。 | — |
| [math-concept-film](https://github.com/liangdabiao/math-concept-film) | 30 | — | — | — | 你说一个数学概念，AI 还你一部带旁白的数学动画短片（Claude Code / Codex）。 | [▶](https://www.bilibili.com/video/BV1ws4R6fEHh) |
| [recursive-math-animator](https://github.com/Science-Prof-Robot/recursive-math-animator) | 13 | — | — | — | Cursor / Claude Code skill：manim + manim-voiceover，git 管理场景版本。 | — |
| [animus](https://github.com/KacemMathlouthi/animus) | 15 | — | — | — | 产出带旁白、有研究依据的解说视频，视觉全部代码驱动。 | — |
| [Chalkboard](https://github.com/nicglazkov/Chalkboard) | 9 | — | — | — | 多 Agent 流水线：任意主题 → 带旁白的 manim 动画。 | — |
| [manim-skill (awesome-skills)](https://github.com/awesome-skills/manim-skill) | 7 | — | — | — | 面向技术博客与教学的 manim 动画 skill。 | — |
| [manim-skill (vumichien)](https://github.com/vumichien/manim-skill) | 6 | — | — | — | 点子/论文/数学 → manim 动画，4 角色 Claude Code Agent 流水线。 | — |
| [paper2video](https://github.com/edwardyen724-g/paper2video) | 6 | — | — | — | 任意技术文章 → 2–5 分钟 3Blue1Brown 风格讲解视频，端到端开源。 | — |
| [notes-to-video](https://github.com/cymcymcymcym/notes-to-video) | 5 | — | — | — | 笔记 → 3Blue1Brown 风格的动画讲解视频（Claude Code skill）。 | — |
| [ManimML](https://github.com/helblazer811/ManimML) | 3.5k | — | — | — | Manim Community Library 构建的常见机器学习概念动画与可视化。 | — |
| [manim_graphic](https://github.com/theaashaychahande/manim_graphic) | 0 | — | — | — | 纯 Python + Manim CE 构建的高级动效动画：粒子系统、3D 弹出、镜头运动、光轨。 | — |
| [manim-plugintemplate](https://github.com/ManimCommunity/manim-plugintemplate) | 78 | — | — | — | 开发自定义 Manim 插件的官方脚手架，含项目结构和测试模板。 | — |
| [Code2Video](https://github.com/showlab/Code2Video) | 2.1k | Python | — | — | 以代码为中心的 Agent 框架，通过可执行 Manim 代码从知识点生成教学视频。三智能体：规划器、编码器、评论器。 | — |
| [TheoremExplainAgent](https://github.com/TIGER-AI-Lab/TheoremExplainAgent) | 1.5k | Python | — | — | 双智能体系统（规划器+编码器）自动生成最长 10 分钟的定理讲解视频（ACL 2025）。 | — |
| [ManimCat](https://github.com/Wing900/ManimCat) | 464 | Python | Active | 2026-09-26 | 自然语言生成数学动画，高质量 manim 渲染。 | — |
| [KimiK3Manim](https://github.com/HarleyCoops/KimiK3Manim) | 143 | Python | Active | 2026-07-29 | 用 Kimi K3 生成数学/物理讲解动画。 | — |
| [manim-notebook](https://github.com/Manim-Notebook/manim-notebook) | 49 | Python | Active | 2026-08-05 | 在 VSCode 中交互式预览的 ManimGL 笔记本。 | [▶](https://youtu.be/rbu7Zu5X1zI) |

## 建模案例与技能

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [holo-card-studio](https://github.com/EverettFish/holo-card-studio) | 1.9k | — | — | — | Python+Blender+Three.js 全息卡片生成器：视差、全息、星光特效。 | — |
| [camera-to-blender](https://github.com/ahujasid/camera-to-blender) | 842 | — | — | — | 拍一张真实物体的照片，直接"贴"进 Blender。 | — |
| [GameFactory-3A](https://github.com/OpenDCAI/GameFactory-3A) | 839 | — | — | — | 开源 3A 游戏生成 skill 与资产框架。 | — |
| [CozyClay](https://github.com/NomaDamas/CozyClay) | 761 | — | — | — | 浏览器里的开源预演（previs）工具：摆场景、摆角色 pose、设计运镜。 | — |
| [3dviz-pro-max](https://github.com/viettranx/3dviz-pro-max) | 680 | — | — | — | 创意 3D 可视化 Agent skill：点子 → 可探索的 Three.js/Blender 场景。 | — |
| [RuiC-card-skill](https://github.com/HRuiCcc/RuiC-card-skill) | 501 | — | — | — | 一句话生成可拖转、会流光、带景深层次的 3D 闪卡网页，附可编辑 Blender 工程。 | — |
| [awesome-astra-prompts](https://github.com/TripoGrowthLab/awesome-astra-prompts) | 327 | — | — | — | 200+ GPT-6 Astra 精选提示词与 3D 案例：游戏、Blender 场景、可交互世界。 | — |
| [autoremesher-blender-bridge](https://github.com/adriflex/autoremesher-blender-bridge) | 301 | — | — | — | AutoRemesher 的 Blender 桥接：在 Agent 流水线里做四边面重拓扑。 | — |
| [blender-skills](https://github.com/arjun988/blender-skills) | 272 | — | — | — | 94 个专业 Blender skill，适配 Cursor / Claude Code / Kiro / Codex，MCP 驱动产线。 | — |
| [blender-skills (kevinbadi)](https://github.com/kevinbadi/blender-skills) | 140 | — | — | — | Claude Code 的 Blender skills：3D 产品生成与镜头动画工作流。 | — |
| [cc-blender-skill](https://github.com/RobLe3/cc-blender-skill) | 84 | — | — | — | 自然语言驱动 Blender 5.x，像资深 3D 艺术家一样干活：10 个可链式加载的 skill。 | — |
| [BlenderXAlpha-3DGenSkill](https://github.com/ig-shadow-walker/BlenderXAlpha-3DGenSkill) | 29 | — | — | — | 大白话场景描述 → 在 Blender 里实时搭出 AI 生成的 3D 模型。 | — |
| [blender-kiln](https://github.com/elithril/blender-kiln) | 29 | — | — | — | Claude Code 的 Blender skill + 插件：文字 brief → 生产级 GLB 资产流水线。 | — |
| [awesome-3d-prompts](https://github.com/TripoGrowthLab/awesome-3d-prompts) | 16 | — | — | — | 面向 Astra / Claude / Kimi 的 3D 提示词：游戏、场景、资产、动画与可交互世界。 | — |
| [RemakeBench/skills](https://github.com/RemakeBench/skills) | 11 | — | — | — | 证据驱动的 Claude Code skills：构建并验证可玩的 3D 世界。 | — |
| [claude-code-handbook](https://github.com/ThamJiaHe/claude-code-handbook) | 206 | — | — | — | Claude Code + Remotion 制作程序化视频的实战指南：安装、核心概念、提示词模板、代码示例、排错。 | — |

## Seedance 与视频生成模型工作流

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [seedance2-skill](https://github.com/dexhunter/seedance2-skill) | 4.2k | — | — | — | 为 Seedance 2.0 生成最佳视频提示词的 skill。 | — |
| [seedance-prompt-skill](https://github.com/songguoxs/seedance-prompt-skill) | 2.9k | — | — | — | Seedance 2.0 视频提示词生成 skill。 | — |
| [awesome-seedance](https://github.com/ZeroLu/awesome-seedance) | 2.6k | — | — | — | Seedance 2.0 高保真提示词与资源大全。 | — |
| [Seedance2-Storyboard-Generator](https://github.com/liangdabiao/Seedance2-Storyboard-Generator) | 2.5k | — | — | — | 小说/故事 → 结构化 Seedance 2.0 分镜剧本，开源剧情 skill。 | — |
| [awesome-seedance (LearnPrompt)](https://github.com/LearnPrompt/awesome-seedance) | 1.8k | — | — | — | 证据导向的 Seedance 2.5/2.0 提示词库：463 个案例均可溯源原帖。 | — |
| [manju-laoli-skill](https://github.com/lixiaoxiao9888-create/manju-laoli-skill) | 1.1k | — | — | — | 漫剧老李 AIGC 全流程技能包：模型三选一锁（Seedance 等）+ 工业化短剧产线。 | — |
| [higgsfield-seedance2-jineng](https://github.com/beshuaxian/higgsfield-seedance2-jineng) | 874 | — | — | — | Seedance 2.0 × Higgsfield：15 个 Claude 提示词 skill——电影感、3D CGI、动漫、电商。 | — |
| [seedance2.0-prompt-skill](https://github.com/MapleShaw/seedance2.0-prompt-skill) | 803 | — | — | — | Seedance 2.0 提示词 skill。 | — |
| [make-prompt-seedance2](https://github.com/liangdabiao/make-prompt-seedance2) | 685 | — | — | — | Seedance 2.0 结构化提示词与通用 skill。 | [▶](https://www.bilibili.com/video/BV17qb26vEED) |
| [higgsfield-ai-prompt-skill](https://github.com/OSideMedia/higgsfield-ai-prompt-skill) | 698 | — | — | — | 32 个子 skill，覆盖 Seedance 2.5（omni-reference、video-to-video……）。 | — |
| [ai-shortfilm-prompts](https://github.com/jnMetaCode/ai-shortfilm-prompts) | 458 | — | — | — | 点子 → 电影级、模型可直接用的提示词：Sora · Kling · Veo · Seedance。 | — |
| [cinematic-video-prompt-skill](https://github.com/Rylaispirit/cinematic-video-prompt-skill) | 146 | — | — | — | AI 视频提示词速查表 + Claude Skill：机位、运镜、布光、构图。 | — |
| [awesome-seedance-2.5-prompts-skills](https://github.com/AtlasCloudAI/awesome-seedance-2.5-prompts-skills) | 222 | — | — | — | 100+ Seedance 2.5 提示词（带真实视频预览）+ 可安装的 Agent Skill。 | — |
| [Happy-Horse-1.1](https://github.com/CalvintheBear/Happy-Horse-1-1-Released) | 0 | — | — | — | 阿里 15B 模型：T2V/I2V/R2V + 原生音频 + 7 语言唇形同步，Video Arena #1。 | — |
| [visual-skills](https://github.com/smixs/visual-skills) | 481 | — | Active | — | AI 电影导演 Skills：Murch 剪辑、走位、蒙太奇、摄影、Seedance 2.5 语法。纯 Skill 路线。 | — |
| [Seedance-ShotDesign-Skills](https://github.com/woodfantasy/Seedance-ShotDesign-Skills) | 119 | — | — | — | Seedance 2.5 镜头设计/导演 Skill：4–180 秒、延长、多参考、局部编辑、视角重建、导演风格。 | — |
| [seedance-tvc-director](https://github.com/nutllwhy/seedance-tvc-director) | 293 | — | — | — | Seedance 2.5 TVC 导演：15 秒/30 秒/自定义 TVC、镜头规划、旁白路由、循证返工。 | — |
| [Seedance-CLI](https://github.com/L1angjy/Seedance-CLI) | 1 | — | — | — | 即梦 CLI：面向 Agent 的视频生成任务发布+下载工具。支持 OpenClaw、Hermes、Claude、Codex。 | — |
| [ai-media-generator](https://github.com/Hao0321/ai-media-generator) | 254 | — | — | — | AI 媒体 Agent Skill：自动创建高级导演级提示词、镜头、参考，跨平台生成。 | — |

## 开源视频生成模型

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [Wan2.2](https://github.com/Wan-Video/Wan2.2) | 17.7k | — | — | — | 开放的大规模视频生成模型。 | — |
| [CogVideo](https://github.com/zai-org/CogVideo) | 13.0k | — | — | — | CogVideoX（2024）与 CogVideo（ICLR 2023）。 | [▶](https://www.youtube.com/watch?v=5UCkMzP2VLE) |
| [HunyuanVideo](https://github.com/Tencent-Hunyuan/HunyuanVideo) | 12.6k | — | — | — | 腾讯：大型视频生成模型的系统性框架。 | — |
| [LTX-Video](https://github.com/Lightricks/LTX-Video) | 11.0k | — | — | — | LTX-Video 官方仓库。 | — |
| [LTX-2](https://github.com/Lightricks/LTX-2) | 9.6k | — | — | — | LTX-2 音视频联合生成模型：推理与 LoRA 训练包。 | — |
| [VideoCrafter](https://github.com/AILab-CVC/VideoCrafter) | 5.1k | — | — | — | 突破数据限制的高质量视频扩散模型。 | [▶](https://www.youtube.com/watch?v=0NfmIsNAg-g) |
| [HunyuanVideo-1.5](https://github.com/Tencent-Hunyuan/HunyuanVideo-1.5) | 4.6k | — | — | — | 领先的轻量级视频生成模型。 | — |
| [FastVideo](https://github.com/hao-ai-lab/FastVideo) | 4.5k | — | — | — | 视频生成加速的统一推理与后训练框架。 | — |
| [SkyReels-V2](https://github.com/SkyworkAI/SkyReels-V2) | 7.6k | — | — | — | 无限长度视频生成模型：自回归扩散，可生成电影级长片。 | — |
| [VACE](https://github.com/ali-vilab/VACE) | 4.0k | — | — | — | [ICCV 2025] 视频创作与编辑一体化。 | — |
| [Self-Forcing](https://github.com/guandeh17/Self-Forcing) | 3.5k | — | — | — | 弥合自回归视频扩散中训练与推理的鸿沟。 | — |
| [Open-Sora-V1.2](https://github.com/hpcaitech/Open-Sora) | 29.9k | — | — | — | Open-Sora 2.0：11B 参数，VBench 排名。文/图生视频、无限长度生成。 | [▶](https://www.bilibili.com/video/BV1ow4m1e7PX) |
| [Vchitect-2.0](https://github.com/Vchitect/Vchitect-2.0) | 921 | — | — | — | 稀疏到密集视频生成：渐进训练高质量 T2V。 | — |
| [Stable-Video-Diffusion](https://github.com/Stability-AI/generative-models) | 27.3k | — | — | — | Stability AI SVD：图生视频扩散，相机控制，6fps 25 帧。 | [▶](https://www.youtube.com/watch?v=dtqj-s50ynU) |
| [AnimateDiff](https://github.com/guoyww/AnimateDiff) | 12.3k | — | — | — | 个性化文生图模型做视频无需调优：运动模块注入。 | — |
| [ModelScope-T2V](https://github.com/modelscope/modelscope) | 9.2k | — | — | — | 阿里 ModelScope 文生视频：1.7B 模型，多阶段训练，开放权重。 | — |
| [I2VGen-XL](https://github.com/ali-vilab/I2VGen-XL) | 9 | — | — | — | 阿里图生视频：高质量、与输入图一致、可风格化。 | — |
| [Show-1](https://github.com/showlab/Show-1) | 1.1k | — | — | — | NUS Show Lab：像素级 T2V，逐帧与段落级交错生成。 | — |
| [Open-Sora-Plan](https://github.com/PKU-YuanGroup/Open-Sora-Plan) | 12.2k | — | — | — | 北大开源 Sora 复现计划，DiT 架构。 | [▶](https://youtu.be/IiWTdx2EHCY) |
| [Prompt-A-Video](https://github.com/jiyt17/Prompt-A-Video) | 25 | — | — | — | ICCV 2025：LLM 提示词增强文生视频，奖励进化 + DPO。 | — |
| [Allegro](https://github.com/rhymes-ai/Allegro) | 1.1k | — | — | — | Rhymes AI：高质量文生视频，15s 1080p，DiT 架构。 | — |
| [Sana](https://github.com/NVlabs/Sana) | 9.2k | — | — | — | NVIDIA：高分辨率图像与视频生成，线性 DiT，4K 输出。 | [▶](https://www.youtube.com/watch?v=ztdkfIMkdJ4) |
| [OpenVid](https://github.com/NJU-PCALab/OpenVid-1M) | 471 | — | — | — | 开放视频生成基准：1M 文本-视频对，评估工具包。 | — |
| [Wan2.1](https://github.com/Wan-Video/Wan2.1) | 17.1k | Python | Active | — | 阿里 Wan 2.1/2.2：MoE 架构，1.3B–14B 变体。首个开源 MoE 视频生成模型。1.3B 变体仅需 8GB 显存。 | — |
| [Mochi](https://github.com/genmoai/mochi) | 3.7k | Python | — | — | Genmo Mochi 1：约 100 亿参数，开源视频模型中写实感最强。官方 LoRA 训练器，最佳微调基座。 | — |
| [VideoTuna](https://github.com/VideoVerses/VideoTuna) | 554 | Python | — | — | 一体化视频生成代码库：推理和微调 T2V/I2V/T2I/V2V 模型。支持 Wan2.1、HunyuanVideo、CogVideoX、Mochi。 | — |
| [ConsisID](https://github.com/PKU-YuanGroup/ConsisID) | 862 | Python | — | — | 基于频率分解的身份保持文生视频（CVPR 2025 Highlight）。免微调 DiT 架构。 | [▶](https://www.youtube.com/watch?v=PhlgC-bI5SQ) |
| [MagicTime](https://github.com/PKU-YuanGroup/MagicTime) | 1.3k | Python | — | — | 延时视频生成模型作为蜕变模拟器（TPAMI 2025）。ChronoMagic 数据集 460K 对。 | [▶](https://www.bilibili.com/video/BV1wx421U7Gn) |
| [Latte](https://github.com/Vchitect/Latte) | 1.9k | Python | Active | 2025-03 | 用于视频生成的潜在扩散 Transformer，TMLR 2025，支持文生视频和文生图。 | — |
| [FasterCache](https://github.com/Vchitect/FasterCache) | 268 | Python | Active | 2024-11 | 免训练视频扩散模型加速，ICLR 2025，支持 Open-Sora、CogVideoX、Latte、Mochi 等。 | — |
| [UniAnimate](https://github.com/ali-vilab/UniAnimate) | 1.2k | Python | Active | 2025-04 | 统一视频扩散实现一致性人体图像动画，SCIS 2025，支持首帧条件长视频生成。 | — |
| [SCEPTER](https://github.com/modelscope/scepter) | 550 | Python | Active | 2025-01 | 生成式训练、微调和推理开源框架，支持 FLUX、SD3、CogVideoX、ACE++ 等。 | — |
| [CausVid](https://github.com/tianweiy/CausVid) | 1.4k | Python | Medium | 2025-06 | CVPR 2025 — 4 步自回归视频生成，9.4 FPS，基于因果注意力机制 | — |
| [Helios](https://github.com/PKU-YuanGroup/Helios) | 2.2k | Python | Medium | 2025-05 | 通过渐进式训练实现分钟级视频生成，19.5 FPS | [▶](https://www.youtube.com/watch?v=vd_AgHtOUFQ) |
| [LightX2V](https://github.com/ModelTC/LightX2V) | 2.9k | Python | High | 2025-08 | 轻量级视频生成推理框架，支持多种模型 | — |
| [StreamingVLM](https://github.com/mit-han-lab/streaming-vlm) | 1.1k | Python | Medium | 2025-03 | 用于实时视频理解的流式视觉语言模型 | — |

## 数字人、语音与工具链

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [Deep-Live-Cam](https://github.com/hacksider/Deep-Live-Cam) | 96.9k | — | — | — | 单图实时换脸，请负责任地使用。 | [▶](https://www.youtube.com/watch?v=OlNWCpFdVMA) |
| [VoiceStudio](https://github.com/debpalash/VoiceStudio) | 54.4k | — | — | — | 全本地的 ElevenLabs 替代：声音克隆、声音设计、视频配音。 | — |
| [LivePortrait](https://github.com/KlingAIResearch/LivePortrait) | 19.1k | — | — | — | 让肖像活起来（可灵团队）。 | — |
| [Duix-Avatar](https://github.com/duixcom/Duix-Avatar) | 15.6k | — | — | — | 开源数字人工具包：离线视频生成与数字人克隆。 | — |
| [video-subtitle-remover](https://github.com/YaoFANGUK/video-subtitle-remover) | 13.1k | — | — | — | AI 硬字幕/水印去除，全本地实现。 | [▶](https://b23.tv/guEbl9C) |
| [video-subtitle-extractor](https://github.com/YaoFANGUK/video-subtitle-extractor) | 9.5k | — | — | — | 视频硬字幕提取为 SRT，本地 OCR，带 GUI。 | [▶](https://www.bilibili.com/video/bv11L4y1Y7Tj) |
| [EchoMimicV2](https://github.com/antgroup/echomimic_v2) | 4.7k | — | — | — | [CVPR 2025] 半身人体动画。 | [▶](https://www.youtube.com/watch?v=2ab6U1-nVTQ) |
| [PersonaLive](https://github.com/GVCLab/PersonaLive) | 3.9k | — | — | — | [CVPR 2026] 面向直播的富表现力肖像动画。 | — |
| [MiniMax CLI](https://github.com/MiniMax-AI/cli) | 2.2k | — | — | — | 命令行生成文本、图像、视频、语音与音乐。 | — |
| [douyin-mcp-server](https://github.com/yzfly/douyin-mcp-server) | 1.3k | — | — | — | MCP server / skill：抖音无水印链接 + 文案提取。 | — |
| [comfyui-mcp](https://github.com/artokun/comfyui-mcp) | 793 | — | — | — | ComfyUI 的 Agent 原生控制面板：MCP server + 侧边栏 Agent。 | — |
| [Lumi-Digital-Human](https://github.com/QwenchC/Lumi-Digital-Human) | 2 | — | — | — | 本地流式数字人：实时唇形同步、多 TTS 引擎、浏览器端。 | — |
| [Talking-Head](https://github.com/Bomou-AI/Talking-Head) | 38 | — | — | — | 100+ 语言、350+ 声音模型。开源说话头视频生成。 | — |
| [Talking-Avatar](https://github.com/Bomou-AI/Talking-Avatar) | 14 | — | — | — | 说话头→数字人动画：面部表情+身体手势同步。 | — |
| [ip-human-agent](https://github.com/fa1314/ip-human-agent) | 53 | — | — | — | 超级 IP Agent 4.0：数字人口播全链路自动化。 | — |
| [dlp3d.ai](https://github.com/dlp3d-ai/dlp3d.ai) | 363 | — | — | — | SIGGRAPH Asia 2025：开源自主 3D 角色（LLM + 3D 数字人）。 | [▶](https://www.youtube.com/watch?v=cNEMW6IHKl8) |
| [Motion-Agent](https://github.com/szqwu/Motion-Agent) | 123 | — | — | — | ICLR 2025：LLM 对话框架驱动人体运动生成。 | — |
| [awesome-motion-style-transfer](https://github.com/GuangtaoLyu/awesome-motion-style-transfer) | 1 | — | — | — | 自动更新的人体运动风格迁移论文列表。 | — |
| [MuseTalk](https://github.com/TMElyralab/MuseTalk) | 6.7k | — | — | — | 腾讯实时音频唇形同步，非扩散，推理快。 | — |
| [MuseV](https://github.com/TMElyralab/MuseV) | 2.8k | — | — | — | 腾讯音乐：无限长度数字人视频，扩散生成，身份一致。 | [▶](https://www.bilibili.com/video/BV1ux4y1v7pF) |
| [ER-NeRF](https://github.com/Fictionarry/ER-NeRF) | 1.3k | — | — | — | 高效区域感知 NeRF 说话头：实时、高保真。 | [▶](https://youtu.be/Gc2d3Z8MMuI) |
| [GeneFace++](https://github.com/yerfor/GeneFacePlusPlus) | 1.8k | — | — | — | ICLR 2024：通用化 NeRF 说话脸，音频到运动域适配。 | — |
| [AniPortrait](https://github.com/Zejun-Yang/AniPortrait) | 5.0k | — | — | — | 腾讯：音频+参考肖像→富表现力动画，扩散生成。 | [▶](https://www.bilibili.com/video/BV1H4421F7dE) |
| [Hallo](https://github.com/fudan-generative-vision/hallo) | 8.7k | — | — | — | 复旦：分层音频驱动肖像动画，高保真唇形同步。 | — |
| [Awesome-AIGC-Image-Video-Detection](https://github.com/ant-research/Awesome-AIGC-Image-Video-Detection) | 460 | — | — | — | AI 生成图像与视频检测：数据集、基准、论文、工具。 | [▶](https://www.bilibili.com/video/BV1teuc63E6D) |
| [Open-AI-UGC](https://github.com/Anil-matcha/Open-AI-UGC) | 349 | JavaScript | — | — | Arcads 和 MakeUGC 的免费开源替代。用 Veo 3.1、Seedance 2、Grok Video、Happy Horse 1 生成 AI UGC 视频广告。 | — |
| [Wav2Lip](https://github.com/Rudrabha/Wav2Lip) | 13.2k | Python | — | — | 任意视频中任意人脸的唇形同步：从音频生成精确唇部运动。 | [▶](https://youtu.be/0fXaDCZNOJc) |
| [facefusion](https://github.com/facefusion/facefusion) | 30.1k | Python | — | — | 下一代换脸和增强工具。人脸视频编辑最成熟的仓库。 | — |
| [ChatTTS](https://github.com/2noise/ChatTTS) | 39.9k | Python | — | — | 开源高质量中文 TTS。自然韵律，含笑声和停顿建模。 | [▶](https://www.bilibili.com/video/BV1zn4y1o7iV) |
| [CosyVoice](https://github.com/FunAudioLLM/CosyVoice) | — | Python | — | — | 阿里多语言大语音生成模型：TTS、声音克隆、跨语言合成。 | — |
| [GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS) | 62.3k | Python | — | — | 少样本声音克隆 & TTS：1 分钟参考音频→声音克隆。零样本和少样本模式。 | [▶](https://www.bilibili.com/video/BV12g4y1m7Uw) |
| [EchoMimicV3](https://github.com/antgroup/echomimic_v3) | 1.1k | Python | — | — | 13 亿参数统一多模态多任务人体动画。音频驱动说话人脸和身体动画。 | [▶](https://www.bilibili.com/video/BV1W8tdzEEVN) |
| [MimicTalk](https://github.com/yerfor/MimicTalk) | 830 | Python | — | — | 基于 NeRF 的说话人脸：15 分钟训练个性化 3D 说话头像。音频驱动，高度逼真。 | — |
| [OpenAvatarChat](https://github.com/HumanAIGC-Engineering/OpenAvatarChat) | 3.8k | Python | — | — | 创建逼真数字人的开源平台。实时交互、逼真表情、低延迟、多平台。 | [▶](https://www.bilibili.com/video/BV1sv8QzLEC2) |
| [Wan-Animate](https://github.com/wan-animate/wananimate) | 6 | Python | — | — | 阿里统一 AI 角色动画与替换框架。用参考视频动作驱动静态照片动画。14B 模型。 | — |
| [Fay](https://github.com/xszyou/Fay) | 13.6k | Python | — | — | 实时对话数字人系统，整合 ASR、TTS、LLM。虚拟主播、语音助理场景。 | — |
| [KodaCut](https://github.com/wade56754/KodaCut) | 4 | Python | Active | 2026-07 | 开源 AI 口播剪辑代理：粗剪、紧凑字幕、证据型 B-roll、HUD 信息卡、1.25x 交付。 | — |
| [TEN-framework](https://github.com/TEN-framework/ten-framework) | 11.1k | Go | Active | 2026-08 | 实时多模态对话 AI 开源框架：语音助手、唇形同步数字人、SIP 通话、ESP32 集成。 | — |
| [awesome-heygen-ai-alternatives](https://github.com/furudo-erika/awesome-heygen-ai-alternatives) | 18 | — | Moderate | 2025-08 | HeyGen 开源替代方案精选列表，涵盖 AI 口播和数字人视频生成。 | — |
| [Duix-Mobile](https://github.com/duixcom/Duix-Mobile) | 8.3k | Kotlin | High | 2025-09 | 实时交互 AI 数字人，支持本地部署，延迟 <1.5s，面向移动端 | — |
| [Linly-Talker](https://github.com/Kedreamix/Linly-Talker) | 3.5k | Python | Active | 2026-02-10 | 数字人对话系统：LLM + 说话人头 + 语音的交互式数字人。 | [▶](https://www.bilibili.com/video/BV1rN4y1a76x) |
| [Qwen3-TTS](https://github.com/QwenLM/Qwen3-TTS) | 13.6k | Python | Active | 2026-03-17 | 通义千问团队开源 TTS 模型系列：多语言、零样本声音克隆。 | — |
| [Qwen3-Audiobook-Converter](https://github.com/WhiskeyCoder/Qwen3-Audiobook-Converter) | 1.1k | Python | Active | 2026-04-07 | PDF/EPUB/DOCX/TXT → 高质量有声书（Qwen3-TTS）。 | — |
| [yovoice](https://github.com/leemysw/yovoice) | 367 | — | Active | 2026-09-29 | macOS/Windows 开源声音创作：本地 TTS、声音克隆、情绪控制。 | — |
| [speech-studio](https://github.com/soniqo/speech-studio) | 68 | — | Active | 2026-08-30 | 面向创作者的桌面声音克隆工作室：克隆音色、带情绪写台词。 | [▶](https://www.youtube.com/watch?v=EuIU8tOWyzg) |

## 视频翻译与唇形同步

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [LatentSync](https://github.com/bytedance/LatentSync) | 6.1k | — | — | — | 字节跳动：Latent Diffusion 唇形同步，消费级 GPU。 | — |
| [SadTalker](https://github.com/OpenTalker/SadTalker) | 14.1k | — | — | — | 3DMM 说话头，GTX 1060+ 即可。MIT 许可。 | [▶](https://www.bilibili.com/video/BV1Dc411W7V6) |
| [YouDub](https://github.com/liuzhao1225/YouDub) | 615 | Python | — | — | YouTube 视频自动汉化：下载→分离音轨→识别→翻译→声音克隆→压制中文字幕和配音。 | — |
| [video-retalking](https://github.com/OpenTalker/video-retalking) | 7.3k | Python | Active | 2026-08-10 | 音频驱动的说话人视频唇形同步——嘴部动作与任意音频同步。 | — |
| [VideoLingo](https://github.com/Huanshere/VideoLingo) | 18.5k | Python | Active | 2026-09-27 | Netflix 级字幕切割、翻译、对齐与配音——一键全自动。 | — |
| [YouDub-webui](https://github.com/liuzhao1225/YouDub-webui) | 5.6k | Python | Active | 2026-09-22 | 带 WebUI 的 YouDub：YouTube/B站视频 AI 本地化与配音。 | [▶](https://www.youtube.com/watch?v=ii9Kh4XkA5g) |
| [SmartSub](https://github.com/buxuku/SmartSub) | 5.6k | — | Active | 2026-09-30 | 一站式桌面工具：视频转字幕、翻译、AI 配音与声音克隆、字幕烧录，本地 Whisper/FunASR。 | — |
| [Auto-Synced-Translated-Dubs](https://github.com/ThioJoe/Auto-Synced-Translated-Dubs) | 1.7k | Python | Active | 2026-05-11 | 基于字幕翻译视频，并生成与原片时间轴同步的 AI 配音。 | — |
| [SoniTranslate](https://github.com/R3gm/SoniTranslate) | 1.4k | Python | Active | 2026-08-29 | 视频同步翻译：声音克隆配音 + 字幕对齐。 | [▶](https://www.youtube.com/watch?v=SmGkFaSzq_Q) |
| [violin](https://github.com/shang-zhu/violin) | 1.1k | — | Active | 2026-09-04 | 面向编程 Agent 的开源视频翻译 skill。 | — |
| [video-translator](https://github.com/InsiderX-Pro/video-translator) | 929 | — | Active | 2026-06-17 | 实时视频翻译/配音 skill。 | — |
| [Pandrator](https://github.com/lukaszliniewicz/Pandrator) | 628 | Python | Active | 2026-09-27 | PDF/EPUB → 有声书；字幕/视频 → 翻译配音视频。 | — |
| [CapCap](https://github.com/notepower2k1/CapCap) | 341 | — | Active | 2026-09-23 | Windows 桌面应用：短视频本地化与配音。 | — |
| [youtube-auto-dub (heyncth)](https://github.com/heyncth/youtube-auto-dub) | 304 | Python | Active | 2026-07-22 | YouTube 自动配音流水线：Whisper 转写 → 翻译 → TTS 重配音。 | — |
| [youtube-auto-dub (mazzasaverio)](https://github.com/mazzasaverio/youtube-auto-dub) | 73 | Python | Active | 2026-09-29 | 本地优先的 YouTube 配音：把原声克隆到另一种语言。 | — |

## 视频字幕、转写与翻译工具

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [whisper](https://github.com/openai/whisper) | 109.8k | — | — | — | OpenAI Whisper：鲁棒语音识别模型，转写和字幕生成的事实标准，支持 99 种语言。 | — |
| [faster-whisper](https://github.com/SYSTRAN/faster-whisper) | 25.6k | — | — | — | 4 倍速 Whisper 推理（CTranslate2），更低内存，生产管线首选。 | [▶](https://www.youtube.com/watch?v=0u7tTptBo9I) |
| [whisperX](https://github.com/m-bain/whisperX) | 24.3k | — | — | — | Whisper 词级时间戳 + 说话人分离，精确字幕对齐必备。 | — |
| [FunClip](https://github.com/modelscope/FunClip) | 6.4k | — | — | — | 阿里开源视频裁剪：ASR 驱动、说话人感知、多段提取。 | — |
| [AutoSubtitle](https://github.com/Linwei-Chen/AutoSubtitle) | 14 | — | — | — | AI 视频字幕生成器：Whisper + LLM 翻译，支持多语言 SRT/VTT 输出。 | — |
| [autosubtitlegenerator](https://github.com/snigdhasingh77/autosubtitlegenerator) | 0 | — | — | — | 免费自动字幕生成器：Next.js + FastAPI + Whisper，支持 SRT/VTT 导出和字幕烧录。 | — |
| [pyvideotrans](https://github.com/jianchang512/pyvideotrans) | 19.2k | — | — | — | 视频翻译+配音+字幕工具：ASR → LLM 翻译 → TTS → 视频合成，50+ 语言。 | — |
| [Linly-Dubbing](https://github.com/Kedreamix/Linly-Dubbing) | 3.3k | — | — | — | 智能多语言 AI 配音与翻译：口型同步、声音克隆、字幕对齐。 | — |
| [NarratoAI](https://github.com/linyqh/NarratoAI) | 11.3k | Python | — | — | 影视解说自动化：自动剪辑+配音+字幕。非商用协议。 | — |
| [autoclip](https://github.com/zhouxiaoka/autoclip) | 9.1k | Python | — | — | 长视频 AI 高光提取：YouTube/B站下载→AI 分析→提取精彩片段→合成。 | — |
| [subtitle-burner](https://github.com/july-lyan/subtitle-burner) | 4 | Python | Medium | 2025-04 | Whisper 自动转写 + 一键烧录字幕到视频，支持 Web 界面和命令行 | — |
| [whisper-ctranslate2](https://github.com/Softcatala/whisper-ctranslate2) | 1.4k | Python | Active | 2026-09-22 | 使用 CTranslate2 的 Whisper 语音识别——比 OpenAI 原版快 4 倍。 | — |
| [video-subtitle-generator](https://github.com/YaoFANGUK/video-subtitle-generator) | 1.2k | Python | Moderate | 2024-02-01 | 音频生成 SRT 字幕，全本地 Transformer ASR，带 GUI。 | — |
| [SoloPup Subtitle Studio](https://github.com/OakcoderX/solopup-subtitle-studio) | 0 | Python | Active | 2026-10-28 | 本地 SDH 与中文配音英译审校；支持离线双 SRT 导入、可选 Qwen 辅助、ITT/SRT 导出。MIT；公开预览版；云端 AI 可能收费。 | — |


## 视频增强、超分与修复

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [FlashVSR](https://github.com/OpenImagingLab/FlashVSR) | 1.9k | — | — | — | 实时扩散视频超分：单步流式推理，单 A100 ~17 FPS，4 倍放大。 | — |
| [STCDiT](https://github.com/JyChen9811/STCDiT) | 78 | — | — | — | CVPR 2026：时空一致性扩散 Transformer，高质量视频超分辨率。 | — |
| [NanoVSR](https://github.com/filippawlicki/nanovsr) | 52 | — | — | — | ECCV 2026：边缘设备（Jetson Orin NX）实时 4 倍视频超分，644k 参数，ONNX/TensorRT 兼容。 | — |
| [Anime4K](https://github.com/bloc97/Anime4K) | 21.4k | — | — | — | 轻量 shader 驱动的动漫/线稿放大，实时处理，GPU 加速。 | — |
| [rife-ncnn-vulkan](https://github.com/nihui/rife-ncnn-vulkan) | 1.1k | — | — | — | GPU（Vulkan）实时插帧，视频插帧管线即插即用。 | — |
| [rembg](https://github.com/danielgatis/rembg) | 24.9k | — | — | — | U2-Net 背景去除工具，视频资产合成和数字人抠像必备。 | — |
| [demucs](https://github.com/adefossez/demucs) | 8.5k | — | — | — | 音乐源分离：人声、鼓、贝斯、其他——视频配音和 BGM 隔离必备。 | — |
| [ultimatevocalremovergui](https://github.com/Anjok07/ultimatevocalremovergui) | 26.4k | — | — | — | AI 人声分离/去除 GUI：MDX-Net + VR 架构，内容创作者首选。 | — |
| [VideoEraser](https://github.com/bluedream02/VideoEraser) | 14 | — | — | — | [EMNLP 2025] T2V 扩散中的概念擦除：移除对象、名人、风格。 | — |
| [Real-ESRGAN-ncnn-vulkan](https://github.com/xinntao/Real-ESRGAN-ncnn-vulkan) | 2.2k | — | — | — | GPU 实时视频超分：ncnn 推理，无需 Python。 | — |
| [BasicVSR++](https://github.com/ckkelvinchan/BasicVSR_PlusPlus) | 830 | — | — | — | CVPR 2022：双向传播与对齐的视频超分辨率。 | — |
| [RealBasicVSR](https://github.com/ckkelvinchan/RealBasicVSR) | 1.1k | — | — | — | CVPR 2022：实用视频修复，退化感知适配器。 | — |
| [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) | 37.0k | Python | — | — | 盲超分辨率，适用于噪点/压缩/低分辨率素材。编辑师的默认开源修复工具。 | [▶](https://www.youtube.com/watch?v=fxHWoDSSvSc) |
| [GFPGAN](https://github.com/TencentARC/GFPGAN) | 37.7k | Python | — | — | 盲人脸修复，适用于访谈编辑、社交短视频、档案扫描。与 Real-ESRGAN 搭配使用。 | — |
| [CodeFormer](https://github.com/sczhou/CodeFormer) | 18.2k | Python | — | — | 基于 Transformer 的人脸修复，平衡保真度和感知质量。适用于老旧素材中的退化人脸。 | [▶](https://youtu.be/d3VDpkXlueI) |
| [RIFE](https://github.com/hzwer/Practical-RIFE) | 1.0k | Python | — | — | 实时中间流估计视频插帧。丝滑慢动作和帧率转换。 | [▶](https://www.bilibili.com/video/BV1J3411t7qT) |
| [ProPainter](https://github.com/sczhou/ProPainter) | 7.0k | Python | — | — | 视频修复：物体移除、水印移除、画面补全。清理工作流必备。 | [▶](https://youtu.be/92EHfgCO5-Q) |
| [frame-interpolation](https://github.com/google-research/frame-interpolation) | 3.2k | Python | Active | 2026-06-20 | Google Research 大运动帧插值模型——FILM 可从任意两帧生成平滑慢动作。 | [▶](https://www.youtube.com/watch?v=OAD-BieIjH4) |
| [Video2X](https://github.com/k4yt3x/video2x) | 21.9k | C++ | Active | 2026-09-25 | 基于 ML 的视频超分辨率与帧插值框架——Real-ESRGAN + RIFE + waifu2x。 | [▶](https://youtu.be/mGEfasQl2Zo) |
| [RobustVideoMatting](https://github.com/PeterL1n/RobustVideoMatting) | 9.5k | Python | Active | 2026-07-10 | 鲁棒高分辨率视频抠图——无需绿幕的实时 Alpha 抠图。 | [▶](https://youtu.be/Jvzltozpbpk) |
| [obs-backgroundremoval](https://github.com/royshil/obs-backgroundremoval) | 4.6k | C++ | Active | 2026-09-20 | OBS Studio 实时人像背景移除插件——无需绿幕。 | [▶](https://youtu.be/jC3EKSpNjQk) |
| [BRIA-RMBG-2.0](https://github.com/BRIA-AI/RMBG-2.0) | 330 | Python | Active | 2026-08-30 | 业界领先的背景移除模型——商业级精度的图片和视频抠图。 | — |
| [BasicSR](https://github.com/XPixelGroup/BasicSR) | 8.4k | Python | Moderate | 2024-07-21 | 开源图像/视频修复工具箱：超分、去噪、去模糊（Real-ESRGAN 的诞生地）。 | — |
| [SparkVSR](https://github.com/taco-group/SparkVSR) | 740 | Python | Active | 2026-08-03 | [ECCV 2026] 稀疏关键帧传播的交互式视频超分。 | — |
| [FAST_Anime_VSR](https://github.com/Kiteretsu77/FAST_Anime_VSR) | 74 | Python | Moderate | 2024-01-02 | 动漫视频快速超分与修复（Real-CUGAN + Real-ESRGAN + VCISR）。 | — |

## ComfyUI 视频生态与自定义节点

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [ComfyUI-AnimateDiff-Evolved](https://github.com/Kosinkadink/ComfyUI-AnimateDiff-Evolved) | 3.5k | — | — | — | ComfyUI 增强 AnimateDiff：运动模块、ControlNet、稀疏控制。 | — |
| [ComfyUI-VideoHelperSuite](https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite) | 1.9k | — | — | — | ComfyUI 视频 I/O：加载/保存 MP4、GIF、WebM、帧插值。 | — |
| [ComfyUI-LTXVideo](https://github.com/Lightricks/ComfyUI-LTXVideo) | 4.1k | — | — | — | ComfyUI 的 LTX-Video 模型支持：文生视频和图生视频工作流。 | — |
| [ComfyUI-WanVideoWrapper](https://github.com/kijai/ComfyUI-WanVideoWrapper) | 6.7k | — | — | — | ComfyUI 的 Wan 视频模型封装：Wan 2.1/2.2 T2V/I2V，支持 LoRA。 | — |
| [ComfyUI-Manager](https://github.com/Comfy-Org/ComfyUI-Manager) | 16.3k | — | — | — | ComfyUI 包管理器：从 UI 安装/更新自定义节点、模型和工作流。 | — |
| [ComfyUI_FlashVSR](https://github.com/smthemex/ComfyUI_FlashVSR) | 397 | — | — | — | ComfyUI 的 FlashVSR 超分节点：实时 4 倍视频放大。 | — |
| [comfyui_loops](https://github.com/dicksensei69/comfyui_loops) | 1 | — | — | — | ComfyUI 简单循环节点：从图像序列生成无缝来回循环动画。 | — |
| [ComfyUI-vidflows](https://github.com/kustomzone/ComfyUI-vidflows) | — | — | — | — | ComfyUI 视频工作流：Sora2-ComfyUI、Veo 3、Story Creator 节点包。 | — |
| [ComfyUI-Agent-Kit](https://github.com/SlavaSexton/comfyui-agent-kit) | 105 | Python | Active | — | 一个 ComfyUI Skill 适配所有 AI 编程 Agent（Claude Code、Codex、Gemini CLI、Qwen Code）：75 个模型提示词配方、581 个模板、硬件感知选型。 | — |
| [ComfyUI-Frame-Interpolation](https://github.com/Fannovel16/ComfyUI-Frame-Interpolation) | 1.1k | Python | Active | 2026-03-29 | ComfyUI 视频补帧节点集。 | — |
| [Steerable-Motion](https://github.com/banodoco/Steerable-Motion) | 974 | Python | Active | 2025-10-03 | 用图像序列驱动视频——ComfyUI 关键帧引导运动。 | — |
| [ComfyUI-LatentSyncWrapper](https://github.com/ShmuelRonen/ComfyUI-LatentSyncWrapper) | 963 | Python | Active | 2025-09-04 | ComfyUI 的 LatentSync 唇形同步节点。 | — |
| [ComfyUI-QwenVL](https://github.com/1038lab/ComfyUI-QwenVL) | 898 | Python | Active | 2026-09-14 | ComfyUI 的 Qwen-VL 系列节点（Qwen2.5-VL、Qwen3-VL），视频/图像理解。 | — |
| [comfyui-vrgamedevgirl](https://github.com/vrgamegirl19/comfyui-vrgamedevgirl) | 758 | Python | Active | 2026-09-29 | 电影颗粒、色彩匹配与视频增强节点。 | — |
| [ComfyUI-PainterI2V](https://github.com/princepainter/ComfyUI-PainterI2V) | 634 | Python | Active | 2026-08-01 | 增强的 Wan2.2 图生视频节点，修复慢动作问题。 | — |
| [Vibe-Workflow](https://github.com/SamurAIGPT/Vibe-Workflow) | 605 | — | Active | 2026-09-17 | 开源 AI 媒体工作流节点画布（Weavy/Krea Nodes 的开源替代）。 | — |
| [ComfyUI_VLM_nodes](https://github.com/gokayfem/ComfyUI_VLM_nodes) | 589 | Python | Active | 2026-08-08 | 视觉语言模型节点：Qwen3-VL、Moondream 3、Florence-2、SmolVLM2。 | — |
| [Bjornulf_custom_nodes](https://github.com/justUmen/Bjornulf_custom_nodes) | 549 | Python | Active | 2025-06-11 | 163 个节点：文本、图像、视频、LoRA 等操作。 | [▶](https://www.youtube.com/watch?v=YiGgyh7nQRg) |
| [ComfyUI-LTXTricks](https://github.com/logtd/ComfyUI-LTXTricks) | 512 | Python | Active | 2025-03-05 | LTX Video 模型的额外控制节点。 | — |
| [ComfyUI-HunyuanLoom](https://github.com/logtd/ComfyUI-HunyuanLoom) | 492 | Python | Active | 2025-02-21 | 用混元视频模型做视频编辑的节点。 | — |

## FFmpeg 与 CLI 视频工具链

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [video-use](https://github.com/browser-use/video-use) | 28.3k | — | — | — | 用编程 Agent 剪视频（browser-use 团队）。 | — |
| [Auto-Editor](https://github.com/WyattBlue/auto-editor) | 5.4k | — | — | — | 高效媒体分析与渲染：自动检测静音、切空白、裁切。CLI 优先。 | — |
| [ffsubsync](https://github.com/smacke/ffsubsync) | 7.9k | — | — | — | 语音识别对齐字幕同步，自动字幕管线必备。 | — |
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | 194.4k | — | — | — | 素材采集主力：功能最全的命令行音视频下载器。 | [▶](https://www.youtube.com/watch?v=YE7VzlLtp-4) |
| [VideoHighlighter](https://github.com/Aseiel/VideoHighlighter) | 157 | — | — | — | 本地 AI 视频分析器：视觉搜索、自动高光、场景/对象/动作检测 + 字幕。 | — |
| [headless-screen-recorder](https://github.com/brianbaso/headless-screen-recorder) | — | TypeScript | — | — | Puppeteer 无头 Chrome 录屏插件，使用 beginFrame API。专业色彩校正。 | — |
| [shutter-encoder](https://github.com/paulpacifico/shutter-encoder) | 2.8k | Java | Active | 2026-06 | FFmpeg 视频编码、转换和处理 GUI，支持 AV1、HEVC、VP9 等多种编解码器和批处理。 | — |
| [ffmpeg-python](https://github.com/kkroening/ffmpeg-python) | 11.0k | Python | Medium | 2025-04 | FFmpeg 的 Python 绑定，支持复杂滤镜图 | — |

## Blender 与 3D

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [blender-auto-render](https://github.com/miolini/blender-auto-render) | 3 | — | — | — | Blender 自动化渲染管线：AI 生成的场景脚本 → CI/CD 无头渲染，Docker 兼容。 | — |
| [blender-python-toolkit](https://github.com/AleBrito124356/blender-python-toolkit) | 2 | — | — | — | Blender 无头自动化：程序化城市、产品转台、批量渲染、数据驱动 3D 图表，EEVEE 优先。 | — |
| [3DModelTurntableMaker](https://github.com/TuesdayPoetry/3DModelTurntableMaker) | 1 | — | — | — | 任意 3D 模型 → 循环转台动画，Blender 5.0 后台渲染，10+ 格式。 | — |
| [python-blender-video-automation](https://github.com/rbcommoncents/python-blender-video-automation) | 1 | — | — | — | Python 驱动的 Blender 动画场景构建设计自动化项目。 | — |
| [fake-bpy-module](https://github.com/nutti/fake-bpy-module) | 1.8k | — | — | — | Blender Python API 补全桩，IDE 自动补全必备。 | — |
| [blender-production-skills](https://github.com/XliuXjianX/blender-production-skills) | 243 | — | — | — | Claude Code 的 Blender 制作 Skills：3D 建模、动画和渲染自动化。 | — |
| [gsplat](https://github.com/nerfstudio-project/gsplat) | 5.7k | Cuda | Active | 2026-09-20 | Nerfstudio 的 CUDA Gaussian Splatting 库——快速可微光栅化器，用于 3DGS 训练和渲染。 | [▶](https://www.youtube.com/watch?v=ACPTiP98Pf8) |

## 角色、动捕与游戏资产

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [mixamo-llm-mocap](https://github.com/squall01337/mixamo-llm-mocap) | 345 | — | — | — | 任意视频 → Mixamo 骨骼动画：GVHMR 估计 + spec 驱动重定向 + Blender FK 应用。 | — |
| [blender-game-skills](https://github.com/majidmanzarpour/blender-game-skills) | 131 | — | — | — | Blender 游戏开发 Claude Code skills：概念图 → 绑定好的游戏级 3D 资产。 | — |
| [HY-Motion-1.0](https://github.com/Tencent-Hunyuan/HY-Motion-1.0) | 2.6k | Python | Active | 2025-12 | 十亿级 DiT 文本到 3D 人体动作生成，三阶段训练：预训练、微调、RLHF，指令跟随 SOTA。 | — |
| [FollowYourPose](https://github.com/THUSIGSICLAB/FollowYourPose) | 1 | Python | Moderate | 2024-03 | 基于无姿态视频的姿态引导文生视频，AAAI 2024，两阶段训练含零初始化姿态编码器。 | — |
| [godmodeanimation](https://github.com/lyogavin/godmodeanimation) | 283 | Python | Moderate | 2025-05 | 通过文生视频和图生视频模型生成 2D 游戏动画，AI 精灵图生成器。 | — |
| [DisPose](https://github.com/lihxxx/DisPose) | 376 | Python | Moderate | 2024-12 | 通过将骨骼姿态分解为运动场引导和关键点对应实现可控角色图像动画。 | — |
| [live2d-motion3](https://github.com/EasyLive2D/live2d-motion3) | 31 | Python | Moderate | 2025-08 | Live2D 动画 Python 实现：读取 motion3.json、控制模型动画、可视化曲线、GUI 编辑动作。 | — |

## 实时与交互式视频生成

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [StreamingT2V](https://github.com/Picsart-AI-Research/StreamingT2V) | 1.6k | — | — | — | 流式文生视频：80+ 帧生成，时间一致性，无自回归漂移。 | [▶](https://youtu.be/md4lp42vOGU) |
| [JoyAI-VL-Interaction](https://github.com/jd-opensource/JoyAI-VL-Interaction) | 1.9k | Python | — | — | 开放实时视频-语言交互系统。8B 视觉优先模型，持续观看并主动响应。 | — |
| [realtime-ai](https://github.com/realtime-ai/realtime-ai) | 184 | Go | — | — | 基于 WebRTC 的实时 AI 音视频处理框架。模块化管线：STT→LLM→TTS。 | — |
| [TeleFuser](https://github.com/Tele-AI/TeleFuser) | 31 | Python | — | — | 世界模型推理和多媒体生成高性能运行时。持续流式、WebRTC 控制、分布式 GPU。 | — |
| [krea-realtime-video](https://github.com/krea-ai/realtime-video) | 585 | Python | — | — | Krea Realtime 14B：开源实时 AI 视频模型。从 Wan 2.1 14B 用 Self-Forcing 蒸馏。B200 上 11fps。 | — |
| [CyberVerse](https://github.com/Lynpoint/CyberVerse) | 1.7k | Python | — | — | 自托管实时数字人 Agent 平台。WebRTC、角色记忆、工具、RAG、可选数字人视频。 | [▶](https://youtu.be/Lk88sew2x4o) |
| [livekit-agents](https://github.com/livekit/agents-js) | 938 | TypeScript | — | — | 用 Node.js 构建实时多模态 AI Agent。基于 WebRTC，灵活的 STT/LLM/TTS 集成，MCP 支持。 | — |

## 视频生成 API 与编排

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [augstai/awesome-ai-video-generation](https://github.com/augstai/awesome-ai-video-generation) | 9 | — | — | — | AI 视频生成工具：T2V 模型、数字人、UGC 广告生成器、口型同步、开源。 | — |
| [vargHQ/sdk](https://github.com/vargHQ/sdk) | 340 | — | — | — | "视频的 JSX"：一个 TypeScript API 调度 Kling、Flux、ElevenLabs、Sora。 | — |
| [MiniMax-MCP](https://github.com/MiniMax-AI/MiniMax-MCP) | 1.6k | — | — | — | MiniMax 官方 MCP server：TTS、图像、视频生成 API。 | — |
| [minimax-h3-cli](https://github.com/harlowprewitt7/minimax-h3-cli) | 30 | — | Active | 2026-10-04 | MiniMax H3 CLI 与视频 skill 指南：安装、模型配置、提示词工作流。 | — |

## 相关

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [Video-MME](https://github.com/MME-Benchmarks/Video-MME) | 0.8k | Python | — | — | 首个多模态 LLM 视频分析综合评测基准。900 个视频、254 小时、2700 问答对（CVPR 2025）。 | — |
| [LVBench](https://github.com/zai-org/LVBench) | 152 | Python | Moderate | 2024-08 | 极限长视频理解基准，评测长达 2 小时的视频，ICCV 2025，六大核心能力。 | — |
| [VideoLLaMA3](https://github.com/DAMO-NLP-SG/VideoLLaMA3) | 1.2k | Python | Active | 2025-02 | 前沿多模态基础模型，支持图像和视频理解，VideoMME 和 LVBench 排行榜最佳 7B 模型。 | — |
| [OVO-Bench](https://github.com/JoeLeelyf/OVO-Bench) | 164 | Python | Moderate | 2025-01 | 在线视频理解基准，CVPR 2025，评测回溯追踪、实时感知和前向主动响应。 | — |
| [VideoEspresso](https://github.com/hshjerry/VideoEspresso) | 143 | Python | Active | 2025-04 | 大规模思维链数据集，通过核心帧选择实现细粒度视频推理，CVPR 2025 Oral。 | — |
| [D3](https://github.com/Zig-HS/D3) | 46 | — | — | — | [ICCV 2025] 无训练 AI 生成视频检测，二阶特征方法。 | — |
| [InternVideo](https://github.com/OpenGVLab/InternVideo) | 2.4k | Python | — | — | 视频基础模型与数据，用于多模态理解。InternVideo2/2.5 支持长上下文建模。 | — |
| [VideoChat](https://github.com/OpenGVLab/Ask-Anything) | 3.4k | Python | — | — | VideoChatGPT：带视频理解的 ChatGPT。端到端视频多模态对话。MVBench 基准（CVPR 2024 Highlight）。 | — |
| [VILA](https://github.com/NVlabs/VILA) | 3.9k | Python | — | — | 高效视频理解和多图像理解的 SOTA 视觉语言模型。NVILA、LongVILA 系列。 | — |
| [TwelveLabs Python SDK](https://github.com/twelvelabs-io/twelvelabs-python) | 51 | Python | Medium | 2025-08 | Twelve Labs 视频理解和搜索 API 的 Python SDK | — |
| [VideoRAG](https://github.com/starsuzi/VideoRAG) | 86 | Python | Medium | 2025-06 | 视频语料库上的检索增强生成框架，支持动态视频检索和多模态表示 | — |
| [VideoRAG-Ren](https://github.com/shuhengchen/VideoRAG_Ren) | 500 | Python | High | 2025-09 | 面向超长上下文视频理解的 RAG 框架，采用双通道架构和知识图谱 | — |
| [Awesome-Multimodal-RAG](https://github.com/JarvisUSTC/Awesome-Multimodal-RAG) | 54 | — | High | 2025-09 | 多模态 RAG 最新进展精选列表，覆盖文本/图像/视频/音频 | — |
| [gaussian-splatting](https://github.com/graphdeco-inria/gaussian-splatting) | 24.0k | C++ | High | 2025-09 | 3D 高斯泼溅实时辐射场渲染 — SIGGRAPH 2023 参考实现 | [▶](https://youtu.be/T_kXY43VZnk) |
| [awesome-gaussians](https://github.com/longxiang-ai/awesome-gaussians) | 358 | — | High | 2025-09 | 自动更新的 3D 高斯泼溅论文精选列表，15 个分类 1000+ 条目 | — |
| [awesome-3D-gaussian-splatting](https://github.com/MrNeRF/awesome-3D-gaussian-splatting) | 8.9k | — | High | 2025-09 | 3D 高斯泼溅研究论文和资源精选列表 | [▶](https://www.youtube.com/watch?v=0xdPpKSkO3I) |
| [Nerfstudio](https://github.com/nerfstudio-project/nerfstudio) | 12.0k | Python | High | 2025-09 | NeRF 和 3DGS 训练、渲染与评估的模块化框架 | — |
| [Video-LLaVA](https://github.com/PKU-YuanGroup/Video-LLaVA) | 3.5k | Python | Active | 2026-08-20 | 通过对齐投影前的统一视觉表示来学习视频理解。 | [▶](https://www.youtube.com/watch?v=EFkN00rGq1U) |
| [VBench](https://github.com/Vchitect/VBench) | 1.8k | Python | Active | 2026-09-28 | CVPR 2024——视频生成模型综合评测基准，覆盖 16 个评估维度。 | [▶](https://www.youtube.com/watch?v=7IhCC8Qqn8Y) |
| [Video-Bench](https://github.com/Video-Bench/Video-Bench) | 81 | Python | Active | 2026-09-10 | 人类偏好对齐的视频生成评测基准——基于 MLLM 的 9 维度评分。 | [▶](https://www.youtube.com/watch?v=BMvgyWbWPFg) |
| [VGA-Bench](https://github.com/BestiVictory/VGA-Bench) | 3 | Python | Active | 2026-08-20 | CVPR 2026——视频美学、生成质量和文本-视频对齐的统一评测基准。 | — |
| [physics-IQ-benchmark](https://github.com/google-deepmind/physics-IQ-benchmark) | 365 | Python | Active | 2026-09-15 | DeepMind 的视频生成模型物理理解基准——真实物理场景评测。 | — |
| [OpenS2V-Nexus](https://github.com/PKU-YuanGroup/OpenS2V-Nexus) | 231 | Python | Active | 2026-09-20 | NeurIPS 2025——百万级数据集与基准，面向主体驱动视频生成。 | — |

## 相关：Unreal、WebGL 与 3D 资产生成

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [unreal-agent-harness](https://github.com/per-simmons/unreal-agent-harness) | 195 | — | — | — | AI Agent 通过 Unreal MCP 在虚幻引擎 5.8 里建城市。 | — |
| [webgl-animation-skills](https://github.com/iart-ai/webgl-animation-skills) | 18 | — | — | — | Claude Code 的 3D 动效/WebGL skills：Three.js、GLSL 着色器、粒子系统。 | — |
| [media2threejs](https://github.com/promptwhisper/media2threejs) | 2 | — | — | — | 从图片/视频重建可编辑、可动画的 Three.js 物体、角色与场景。 | — |
| [Hunyuan3D-2](https://github.com/Tencent-Hunyuan/Hunyuan3D-2) | 15.0k | — | — | — | 腾讯：大规模扩散模型的高分辨率 3D 资产生成。 | — |
| [ComfyUI-Trellis2](https://github.com/visualbruno/ComfyUI-Trellis2) | 847 | — | — | — | Microsoft Trellis.2 图生 3D 的 ComfyUI 封装。 | — |
| [claude-opus-5-5-demo](https://github.com/riba2534/claude-opus-5-5-demo) | 1.0k | — | — | — | 用 Claude Opus 5.5 做的 3D 游戏演示，含中文提示词。 | — |

## 相关 Awesome Lists

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [awesome-video-generation](https://github.com/backblaze-labs/awesome-video-generation) | 33 | — | — | — | AI 视频生成 API、SDK 和工具精选列表。覆盖商业服务、开源模型和生产基础设施。 | — |
| [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) | 75.9k | — | — | — | 全领域 Claude Skills 总清单。 | — |
| [awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) | 35.0k | — | — | — | 1000+ 适配 Claude Code 等工具的 agent skills。 | — |
| [Awesome-Video-Diffusion](https://github.com/showlab/Awesome-Video-Diffusion) | 5.8k | — | — | — | 学术向的视频生成/编辑扩散模型精选。 | [▶](https://www.youtube.com/watch?v=QmqWhUjPkJI) |
| [awesome-claude-video-skills](https://github.com/zhuyansen/awesome-claude-video-skills) | 457 | — | — | — | 让 Claude Code / Codex 做视频的 skills 与工具包。 | — |
| [awesome-ai-video](https://github.com/zhaotoday/awesome-ai-video) | 18 | — | — | — | AI 视频生产资源索引（中文）。 | — |
| [awesome-video-automation](https://github.com/renezander030/awesome-video-automation) | 4 | — | — | — | 编程视频工具与工作流综合索引。 | — |
| [awesome-ai-media-skills](https://github.com/JuneYaooo/awesome-ai-media-skills) | 5 | — | — | — | 精选 Claude Code Skills、MCP Server 与 Agent 能力，面向视频创作。 | — |
| [garden-skills](https://github.com/ConardLi/garden-skills) | 12.7k | — | — | — | 生产级 Agent Skills 合集，含 Web 视频演示。 | — |
| [ai-film-skills](https://github.com/62656456/ai-film-skills) | 60 | — | — | — | 21 个独立影视/视频 Skill 模块：分镜、导演、资产、风格管理。 | — |
| [archify](https://github.com/tt-a1i/archify) | 78.9k | — | — | — | 代码→技术图表 Agent Skill（架构可视化）。 | — |
| [awesome-ai-video-editing](https://github.com/Supersynergy/awesome-ai-video-editing) | 2 | — | — | — | 110+ AI 视频剪辑工具，Agent 原生导向。 | — |
| [awesome-ai-agents-2026](https://github.com/caramaschiHG/awesome-ai-agents-2026) | 1.9k | — | — | — | 340+ AI Agent 资源，20+ 类别，月度更新。 | — |
| [awesome-agent-everything](https://github.com/greasebig/awesome-agent-everything) | 0 | — | — | — | 所有 awesome Agent 仓库元索引：框架、Skills、MCP、安全。 | — |
| [awesome-video-super-resolution-diffusion](https://github.com/yjsunnn/Awesome-video-super-resolution-diffusion) | 224 | — | — | — | 扩散视频超分论文精选，每日从 arXiv 更新。 | — |
| [Aweosome-Video-Agent](https://github.com/haozheguo/Aweosome-Video-Agent) | 8 | — | — | — | 长视频理解与 Video Agent 论文、基准、代码。 | — |
| [trending-claude-skills](https://github.com/linny006/trending-claude-skills) | 123 | — | — | — | 自动更新的 Claude Skills 排行榜，每 15 分钟刷新。 | — |
| [awesome-ai-image-tools](https://github.com/stimQQ/awesome-ai-image-tools) | 5 | — | — | — | 100+ 开源 AI 图像与视频模型、库、API、插件。 | — |
| [awesome-cg-vfx-pipeline](https://github.com/cgwire/awesome-cg-vfx-pipeline) | 1.3k | — | — | — | CG/VFX 管线资源：资产管理、渲染农场、合成。 | — |
| [awesome-claude-video](https://github.com/opusvideo/awesome-claude-video) | 183 | — | — | — | Claude Opus 5.5 代码渲染视频的中英双语案例合集，含提示词。 | — |
| [awesome-ai-video-models](https://github.com/Anil-matcha/awesome-ai-video-models) | 197 | — | — | — | 最完整的 AI 视频生成模型对比——哪个模型、走哪个 API、什么价格、多快。 | [▶](https://www.youtube.com/watch?v=SOXsxqnQGlc) |
| [Awesome-World-Models](https://github.com/NeuraLiying/Awesome-World-Models) | 3 | — | Active | 2026-07 | 340+ 篇世界模型论文，覆盖视频生成、自动驾驶、机器人、3D/4D、物理仿真和基准。 | — |
| [Awesome-AI4Animation](https://github.com/yunlong10/Awesome-AI4Animation) | 215 | — | Active | 2025-07 | 赛璐璐动画 GenAI 最新论文、项目和数据集，ICCV 2025 AISTORY Workshop。 | [▶](https://www.youtube.com/watch?v=iUF-LsqFKpI) |
| [awesome-generative-ai](https://github.com/steven2358/awesome-generative-ai) | 12.7k | — | Active | 2026-09 | 现代生成式 AI 项目和服务精选列表，覆盖文本、编码、代理、图像、视频和音频生成。 | — |
| [top-100-comfyui](https://github.com/liusida/top-100-comfyui) | 422 | — | High | 2025-09 | 按 GitHub Stars 自动更新的 ComfyUI Top 100 仓库列表 | — |
| [awesome-rm-for-video-generation](https://github.com/chrisliu298/awesome-rm-for-video-generation) | 3 | — | Active | 2026-09 | 视频奖励模型论文、数据集和代码精选集，覆盖视频生成的 RLHF/DPO/GRPO 和 VideoLLM 评判。 | — |
| [Awesome-Streaming-Video-Understanding](https://github.com/Yang011013/Awesome-Streaming-Video-Understanding) | 31 | — | Active | 2025-10 | 流式/在线视频理解研究论文和基准精选，覆盖 StreamingVLM、StreamForest、LiveCC 等。 | — |
| [video-cnn-interpretability](https://github.com/MSWEIMZ/video-cnn-interpretability) | 2 | Python | Active | 2026-09 | 视频深度学习和可解释性论文自动策展，808 篇论文含趋势分析和交互式仪表板。 | — |
| [free-voice-clone](https://github.com/0xSojalSec/free-voice-clone) | 637 | — | Active | 2026-04-09 | 本地免费声音克隆 TTS 与音乐生成模型大全。 | — |
| [awesome-ai-voice](https://github.com/wildminder/awesome-ai-voice) | 499 | — | Active | 2026-09-23 | 开源 TTS、声音克隆与音乐生成模型精选。 | — |
| [awesome-ai-motion](https://github.com/gongnyang/awesome-ai-motion) | 58 | — | Active | 2026-09-30 | 637 种 AI 视频/信息图/滚动长页动效技巧——附渲染片段、配方与路线。 | — |

## On X

这个圈子在 X 上聊什么（2026-09-30 网搜核实）。

**值得关注的账号**

- [@HeyGen](https://x.com/HeyGen) — HyperFrames 发布与更新。
- [@remotion](https://x.com/remotion) — Remotion 官方。
- [@calesthioailabs](https://x.com/calesthioailabs) — OpenMontage 实验室。
- [@op7418](https://x.com/op7418) — 归藏，product video skill 作者。
- [@VincentWei93](https://x.com/VincentWei93) — video-shotcraft / anything2explainer / video-talkcraft 作者。
- [@slimer48484](https://x.com/slimer48484) — mexicat，pdoom MV 作者。
- [@anshuc](https://x.com/anshuc) — dream-loop（Blender 3D 视觉）。
- [@seekjourney](https://x.com/seekjourney) — hyperframes-motion-director。
- [@aikangarooking](https://x.com/aikangarooking) — 袋鼠帝，高产的中文 AI skills 作者。

**热帖与名场面**

- [X 趋势话题："AI Music Video Champions Progress Over Doom Warnings"](https://x.com/i/trending/2104161956634517980) —— pdoom-video 引爆的一波讨论（2026-09）。
- [mrdoob 聊 pdoom 视频](https://x.com/mrdoob/status/2104062526950613277) —— three.js 作者本人注意到了这支代码渲染的 MV。
- [HeyGen 官方 HyperFrames 发布帖](https://x.com/HeyGen/status/2044827454460871072)；另见 [AYi："HeyGen 这次开源，把 AI 做视频的最后一道门槛……"](https://x.com/AYi_AInotes/status/2045310892284199233)
- [OpenMontage 讨论](https://x.com/RoundtableSpace/status/2069929815994487022) —— 该仓库还冲上过 GitHub Trending 第 1。
- [Seedance 2.0 天天刷屏](https://x.com/vivimoneya/status/2074748410557759596) —— 以及付费墙之争。
- pdoom 仓库的 trending 数据可在 [trendshift.io](https://trendshift.io/repositories/264721) 追踪。

## 贡献

欢迎提交 Pull Request！添加的项目需开源，且与“用文本模型 / 代码 / Agent 做视频”（或其工作流）相关；请保持所在分区的表格格式，改动条目时顺手核实更新 Star 数。

## 许可

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

在法律允许的范围内，贡献者已放弃本作品的所有版权和相关权利。
