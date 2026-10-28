# Awesome Video Skills

**English** | [中文](README_zh-CN.md)

> A curated collection of open-source projects for **making videos with text models**: the LLM (Claude / Opus / Codex…) writes the code — Remotion, HyperFrames, three.js, Blender, manim — and the code **renders** the video. Deterministic, editable, agent-native.
>
> Scope note: the core focus is *code-rendered* video. Prompt-driven video-generation-model workflows (Seedance & friends) get their [own dedicated section](#seedance--video-generation-model-workflows), and diffusion models / agentic studio platforms are kept brief at the end.

[![Awesome](https://cdn.jsdelivr.net/gh/sindresorhus/awesome@d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

**Data snapshot: 2026-10-07** · Star counts from the GitHub API on that date (`54.3k` = 54,300 stars). · **479 GitHub repos + X community signals**

---

## Contents

- [Showcase: Code-Rendered Works](#showcase-code-rendered-works) (8)
- [Render Engines (code → video)](#render-engines-code--video) (39)
- [AI Video Editing Agents](#ai-video-editing-agents) (36)
- [Agentic Production Systems & Short-Video Pipelines](#agentic-production-systems--short-video-pipelines) (28)
- [MCP & Control Layers](#mcp--control-layers) (13)
- [Video Skills: Product Films, Promos & Explainers](#video-skills-product-films-promos--explainers) (45)
- [Video Skills: Short Drama, Story & Recap](#video-skills-short-drama-story--recap) (9)
- [manim & Math-Education Videos](#manim--math-education-videos) (19)
- [Modeling Cases & Skills](#modeling-cases--skills) (16)
- [Seedance & Video-Generation-Model Workflows](#seedance--video-generation-model-workflows) (19)
- [Open-Source Video Generation Models](#open-source-video-generation-models) (36)
- [Digital Humans, Voice & Toolchain](#digital-humans-voice--toolchain) (45)
- [Video Translation & Lip Sync](#video-translation--lip-sync) (15)
- [Video Subtitle, Transcription & Translation Tools](#video-subtitle-transcription--translation-tools) (14)
- [Video Enhancement, Super-Resolution & Restoration](#video-enhancement-super-resolution--restoration) (25)
- [ComfyUI Video Ecosystem & Custom Nodes](#comfyui-video-ecosystem--custom-nodes) (20)
- [FFmpeg & CLI Video Toolchain](#ffmpeg--cli-video-toolchain) (8)
- [Blender & 3D](#blender--3d) (7)
- [Characters, Mocap & Game Assets](#characters-mocap--game-assets) (7)
- [Real-Time & Interactive Video Generation](#real-time--interactive-video-generation) (7)
- [Video Generation API & Orchestration](#video-generation-api--orchestration) (4)
- [Adjacent](#adjacent) (23)
- [Adjacent: Unreal, WebGL & 3D Asset Generation](#adjacent-unreal-webgl--3d-asset-generation) (6)
- [Related Awesome Lists](#related-awesome-lists) (31)
- [On X](#on-x)

## Showcase: Code-Rendered Works

Finished films whose entire pipeline was driven by a text model writing code. Clone them and read the code — that's the tutorial.

| | | |
|:---:|:---:|:---:|
| <a href="https://www.youtube.com/watch?v=5EoO5413dBY"><img src="https://img.youtube.com/vi/5EoO5413dBY/maxresdefault.jpg" width="300" alt="pdoom music video"></a> | <a href="https://youtu.be/gcVvRM_P3SM"><img src="https://raw.githubusercontent.com/Vincentwei1021/video-shotcraft/main/workbench/docs/overview.png" width="300" alt="video-shotcraft"></a> | <a href="https://github.com/op7418/guizang-product-video-skill"><img src="https://raw.githubusercontent.com/op7418/guizang-product-video-skill/main/assets/readme/hero.jpg" width="300" alt="guizang product video"></a> |
| **[pdoom-video](https://github.com/mexicat/pdoom-video)** · [▶ YouTube 4K](https://www.youtube.com/watch?v=5EoO5413dBY) | **[video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft)** · [▶ Demo](https://youtu.be/gcVvRM_P3SM) | **[guizang product video skill](https://github.com/op7418/guizang-product-video-skill)** |
| <a href="https://github.com/achimala/dream-loop"><img src="https://raw.githubusercontent.com/achimala/dream-loop/main/assets/vesper-preview.gif" width="300" alt="dream loop 3D"></a> | <a href="https://github.com/xiejunjie524/handdraw-story-video"><img src="https://raw.githubusercontent.com/xiejunjie524/handdraw-story-video/main/examples/soy-milk-at-4am/preview.jpg" width="300" alt="handdraw story video"></a> | <a href="https://github.com/Alisa0808/vox-director"><img src="https://raw.githubusercontent.com/Alisa0808/vox-director/main/assets/thumbs/football.jpg" width="300" alt="vox director"></a> |
| **[dream-loop](https://github.com/achimala/dream-loop)** | **[handdraw-story-video](https://github.com/xiejunjie524/handdraw-story-video)** | **[vox-director](https://github.com/Alisa0808/vox-director)** |
| <a href="https://www.youtube.com/watch?v=uEB5E67vcPA"><img src="https://img.youtube.com/vi/uEB5E67vcPA/maxresdefault.jpg" width="300" alt="PDoomVideo p5.js music video"></a> | <a href="https://github.com/gnipbao/story-to-handdrawn-video"><img src="https://raw.githubusercontent.com/gnipbao/story-to-handdrawn-video/main/references/style-examples/standard/colored-pencil-diary.png" width="300" alt="handdrawn diary video style"></a> | <a href="https://github.com/alexgreensh/anidoodle"><img src="https://raw.githubusercontent.com/alexgreensh/anidoodle/main/assets/banner.gif" width="300" alt="anidoodle code art"></a> |
| **[PDoomVideo](https://github.com/JohnHeibel/PDoomVideo)** · [▶ YouTube](https://www.youtube.com/watch?v=uEB5E67vcPA) | **[story-to-handdrawn-video](https://github.com/gnipbao/story-to-handdrawn-video)** | **[anidoodle](https://github.com/alexgreensh/anidoodle)** |

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [pdoom-video](https://github.com/mexicat/pdoom-video) | 2.4k | TypeScript | Active | 2026-09-28 | A generative music video made with **Claude Opus 5.5 in Claude Code**: TypeScript + three.js renderer, word-synced ka... | [▶](https://www.youtube.com/watch?v=5EoO5413dBY) |
| [functional-emotions-video](https://github.com/ledbetterljoshua/functional-emotions-video) | 63 | JavaScript | Active | 2026-09-23 | A painted music video by Claude Opus 5.5: custom GPU brushstroke renderer, runs live in the browser. | — |
| [frontier-friday-video](https://github.com/earlvanze/frontier-friday-video) | 1 | JavaScript | Active | 2026-09-28 | Code-rendered music videos: GPT 2D kinetic typography + Claude 3D renderer. | [▶](https://youtu.be/ZJCHKxBG43o) |
| [hyperframes-launches](https://github.com/heygen-com/hyperframes-launches) | 579 | HTML | Active | 2026-09-26 | Open-source HyperFrames compositions behind HeyGen's product launch videos. | — |
| [NullMotion](https://github.com/blixvip/NullMotion) | 814 | HTML | Active | 2026-09-29 | Launch-film preview: a finished motion-graphics ad over the black-and-white HyperFrames drafts it grew from. | — |
| [dream-loop](https://github.com/achimala/dream-loop) | 1.6k | — | — | — | A dreamy 3D loop animation made with Claude Opus 5.5 in Claude Code. | — |
| [Battle-of-Austerlitz-Film](https://github.com/WinterArc21/Battle-of-Austerlitz-Film) | 22 | — | — | — | 4–5 minute cinematic video about the Battle of Austerlitz (1805), built entirely in code: WebGL renderer, terrain dat... | — |
| [PDoomVideo](https://github.com/JohnHeibel/PDoomVideo) | 1.9k | — | — | — | Alternate p5.js rendition of the pdoom track (main entry: mexicat/pdoom-video) — p5.brush painterly rendering, headless Chrome capture, FFmpeg compositing. | [▶](https://youtu.be/8j-hR4fJywU) |

## Render Engines (code → video)

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [Remotion](https://github.com/remotion-dev/remotion) | 61.2k | TypeScript | Active | 2026-09-30 | Make videos programmatically with React. The de-facto standard for code video. | — |
| [HyperFrames](https://github.com/heygen-com/hyperframes) | 58.2k | TypeScript | Active | 2026-09-30 | Write HTML. Render video. Built for agents. (HeyGen) | — |
| [hyperframes-community-skills](https://github.com/heygen-com/hyperframes-community-skills) | 175 | JavaScript | Active | 2026-09-29 | Community-maintained skills for specialized HyperFrames workflows (official repo). | — |
| [html-anything](https://github.com/nexu-io/html-anything) | 9.0k | HTML | Active | 2026-09-15 | The agentic HTML editor: your local AI agent writes the HTML — 75 skills × 9 surfaces. | — |
| [manim](https://github.com/3b1b/manim) | 94.4k | Python | Active | 2026-09-09 | Animation engine for explanatory math videos (3Blue1Brown). | [▶](https://www.youtube.com/watch?v=rbu7Zu5X1zI) |
| [FFmpeg](https://github.com/FFmpeg/FFmpeg) | 64.7k | C | Active | 2026-09-30 | The universal audio/video toolkit every pipeline eventually calls. | — |
| [Shotcut](https://github.com/mltframework/shotcut) | 15.3k | C++ | Active | 2026-09-30 | Cross-platform FOSS non-linear video editor. | — |
| [html-video](https://github.com/nexu-io/html-video) | 4.6k | HTML | Active | 2026-06-21 | Programmatic video for coding agents: HTML, CSS & data → real MP4s on your laptop. | — |
| [remotion-template-three](https://github.com/remotion-dev/template-three) | 110 | TypeScript | Active | 2026-09-29 | Remotion + React Three Fiber template: 3D scenes rendered as video frames. | — |
| [Graphite](https://github.com/GraphiteEditor/Graphite) | 27.4k | Rust | Active | 2026-09-29 | Open-source 2D vector & raster editor with node-based procedural animation, GPU-accelerated. | — |
| [lottie-web](https://github.com/airbnb/lottie-web) | 32.1k | JavaScript | Active | 2025-09-01 | Render After Effects animations natively on web: JSON-driven, agent-writable format. | [▶](https://www.youtube.com/watch?v=5XMUJdjI0L8) |
| [react-three-fiber](https://github.com/pmndrs/react-three-fiber) | 32.6k | TypeScript | Active | 2026-09-30 | React renderer for Three.js: 3D scenes as React components, composable with Remotion for 3D video. | — |
| [p5.js](https://github.com/processing/p5.js) | 24.1k | JavaScript | Active | 2026-09-30 | Creative coding toolkit: sketches → canvas frames → video via CCapture. The pdoom-video substrate. | — |
| [Diffusion Studio editor](https://github.com/diffusionstudio/editor) | 3.2k | TypeScript | Active | 2026-09-29 | Open-source video editor built for agents: edits become code, code becomes video. | [▶](https://youtu.be/HEfHFsfGXjs) |
| [animspark](https://github.com/animspark/animspark) | 32 | TypeScript | Active | 2026-09-26 | The open-source video engine your coding agent can write films in: a film format + frame-exact renderer. | — |
| [presentation-ai](https://github.com/allweonedev/presentation-ai) | 3.0k | TypeScript | Active | 2026-06-05 | Open-source AI presentation generator (Gamma alternative). Code-driven slides → video export. | [▶](https://www.youtube.com/watch?v=UUePLJeFqVQ) |
| [codex-slides](https://github.com/nexu-io/codex-slides) | 922 | TypeScript | Active | 2026-07-21 | Open-source AI slide studio inside Codex: 45 templates, 73 styles, PPTX/PDF export. | — |
| [presenton](https://github.com/presenton/presenton) | 10.9k | TypeScript | Active | 2026-09-30 | Open-source AI presentation generator: self-hosted, BYOK, MCP server, PPTX/PDF export. | — |
| [Ultimate-AI-Media-Generator-Skill](https://github.com/ZeroLu/Ultimate-AI-Media-Generator-Skill) | 92 | MDX | Active | 2026-09-08 | Open-source AI media skill: image, video, audio via CyberBara API. Seedance, Sora, Kling support. | — |
| [manim-mcp](https://github.com/paulnegz/manim-mcp) | 20 | Python | Active | 2026-02-25 | Text-to-video animation via Manim: describe → code → rendered MP4. CLI, agent mode, MCP server. | — |
| [Motion-Canvas](https://github.com/motion-canvas/motion-canvas) | 19.2k | TypeScript | — | — | Code-driven animation framework (generator functions, tweening) for explanatory videos. | — |
| [editly](https://github.com/mifi/editly) | 5.5k | TypeScript | Moderate | 2025-05-12 | Node.js programmatic video editor: JSON/JS-driven multi-track editing with layers, transitions, and overlays. | [▶](https://youtu.be/LNeclLkxUEY) |
| [MotionAgent](https://github.com/leoisufa/MotionAgent) | 5 | Python | Active | 2025-10-22 | ICCV 2025: fine-grained controllable video generation via motion field agent + optical flow. | [▶](https://www.youtube.com/watch?v=O9WW2UpXsAI) |
| [claude-code-video-toolkit](https://github.com/digitalsamba/claude-code-video-toolkit) | 2.2k | Python | Active | 2026-09-28 | AI-native video production workspace for Claude Code: skills, commands, templates, brand profiles, transitions, proje... | — |
| [motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | 35 | JavaScript | Active | 2026-09-30 | Showreel-grade motion graphics from code with original soundtrack for every video. | — |
| [paint-video-skill](https://github.com/nzl153/paint-video-skill) | 1 | JavaScript | Active | 2026-09-30 | Hand-painted animated shorts and music videos in code: watercolor, ink, crayon. | — |
| [JIZURA](https://github.com/852wa/JIZURA) | 1.6k | HTML | Active | 2026-09-29 | Browser-based text PV auto-generator: 860+ components, kinetic typography engine. | [▶](https://852wa.github.io/JIZURA/) |
| [golive-skill](https://github.com/mikehasa/golive-skill) | 1.2k | TypeScript | Active | 2026-09-29 | Code-generated app one-click deploy: live preview → video capture pipeline. | — |
| [opus-video-prompts](https://github.com/joeseesun/opus-video-prompts) | 189 | — | Active | 2026-09-27 | Opus 5.5 code-rendered video prompt collection: 18 prompts + 54 examples. | [▶](https://www.bilibili.com/video/BV1qihf6rE6f) |
| [Revideo](https://github.com/redotvideo/revideo) | — | TypeScript | — | — | A Motion Canvas fork turned into a library: rendering API, templates, and automated pipelines for programmatic video. | — |
| [Diffusion-Studio-Core](https://github.com/diffusionstudio/core) | 1.2k | TypeScript | — | — | Browser video-compositing engine on WebCodecs (no wasm/ffmpeg); edit video with code. | — |
| [text-to-lottie](https://github.com/diffusionstudio/lottie) | 5.5k | TypeScript | — | — | Generate production-ready Lottie animations with Claude Code or Codex. Text-to-Lottie framework with live-update player. | — |
| [AnimTOON](https://github.com/srk0102/AnimTOON) | 20 | Python | — | — | AI model that animates any SVG into Lottie animation. Compact plain-text animation format designed for LLM generation. | — |
| [handanim](https://github.com/subroy13/handanim) | 48 | Python | Moderate | 2025-06 | Python library for whiteboard-style hand-drawn animations. Create educational videos with sketch-style strokes and ha... | — |
| [pytoon-dev](https://github.com/nitinthewiz/pytoon-dev) | 150 | Python | Moderate | 2025-03 | Python animation library for automatically animating cartoon character mouth movements and expressions synced with au... | [▶](https://www.youtube.com/watch?v=Sg2OBBNwF-k) |
| [ai-video-pipeline](https://github.com/shenyuhao1/ai-video-pipeline) | 1 | Python | Moderate | 2026-05 | AI video generation pipeline: Dify workflow + Manim animation + TTS narration + Whisper subtitles + FFmpeg compositin... | — |
| [ManimCommunity/manim](https://github.com/ManimCommunity/manim) | 41.1k | Python | Active | 2026-09-29 | Community-maintained manim: more stable API, better docs, broader plugin ecosystem — the version most skills target. | — |
| [Manim.js](https://github.com/JazonJiao/Manim.js) | 454 | JavaScript | Active | 2026-08-22 | Replicating 3Blue1Brown's manim in JavaScript (p5.js) — math animations that run in the browser. | — |
| [anidoodle](https://github.com/alexgreensh/anidoodle) | 834 | — | Active | 2026-09-28 | Art and animation written as code: illustrations, loops, interactive web art, launch videos. | — |

## AI Video Editing Agents

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [palmier-pro](https://github.com/palmier-io/palmier-pro) | 14.5k | — | — | — | macOS video editor built for AI. | — |
| [jianying-editor-skill](https://github.com/luoluoluo22/jianying-editor-skill) | 3.8k | — | — | — | Agent automates JianYing (CapCut CN) editing. [▶ B站演示](https://www.bilibili.com/video/BV1hLzCBzEDS) | [▶](https://www.bilibili.com/video/BV1hLzCBzEDS) |
| [FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) | 3.5k | — | — | — | AI video editing agent: manual editing → intention-driven direction. | — |
| [chengfeng-videocut-skills](https://github.com/Agentchengfeng/chengfeng-videocut-skills) | 3.0k | — | — | — | A video-cutting agent built with Claude Code Skills. | — |
| [OpenChatCut](https://github.com/0xsline/OpenChatCut) | 2.2k | — | — | — | Local-first conversational AI video editor: pro multi-track timeline + Agent Skills. | — |
| [VideoAgent](https://github.com/HKUDS/VideoAgent) | 1.9k | — | — | — | [EMNLP 2026] Agentic framework for video understanding, editing and remaking. | — |
| [open-edit](https://github.com/veedstudio/open-edit) | 1.6k | — | — | — | Agent-driven editing pipeline: subtitles, motion graphics, slides, edit & render. | — |
| [CutClaw](https://github.com/GVCLab/CutClaw) | 980 | — | — | — | Agentic hours-long video editing via music synchronization. | — |
| [ai-video-editor](https://github.com/MartinDelophy/ai-video-editor) | 881 | — | — | — | Local-first editor where creators and AI agents edit the same real timeline. | [▶](https://youtu.be/bqKhpPPa-qo) |
| [clipify](https://github.com/louisedesadeleer/clipify) | 583 | — | — | — | Claude Code skill: long videos → social-ready clips, auto-highlights, 9:16 reframe. | — |
| [chatgpt-video-editing-skills](https://github.com/Jaycheng1103/chatgpt-video-editing-skills) | 574 | — | — | — | ChatGPT / Codex short-form editing in 8 verifiable steps (繁體中文). | — |
| [velocut](https://github.com/open-ribbi/velocut) | 454 | — | — | — | AI-native local-first editor in the browser: Rust/WASM + WebGPU. | — |
| [ghost-editor](https://github.com/kurbaitaev/ghost-editor) | 66 | — | — | — | AI video editor for talking-head reels: 7 styles, face-safe captions, motion scenes. | — |
| [claude-video](https://github.com/bradautomates/claude-video) | 17.9k | — | — | — | Claude Code Skill: watch and analyze video files, extract key frames, generate summaries. | — |
| [Youtube-clipper-skill](https://github.com/op7418/Youtube-clipper-skill) | 2.2k | — | — | — | Download YouTube, AI semantic chapters, clip segments, bilingual subtitles, burn-in. | — |
| [viral-x-posts](https://github.com/shannhk/viral-x-posts) | 13 | — | — | — | Claude Code skill: 23 viral X/Twitter post formulas for video content distribution. | — |
| [video-ai-analysis](https://github.com/yangchen0991/video-ai-analysis) | 16 | — | — | — | AI-assisted film/TV analysis: shot-by-shot breakdown, scene detection, visual grammar. | — |
| [JoyAI-Video-Edit](https://github.com/jd-opensource/JoyAI-Video-Edit) | 1.9k | — | — | — | Real-time instruction-guided video editing: 30.19 FPS at 720p, autoregressive diffusion, style transfer. | — |
| [hermes-video-editing](https://github.com/argus-metis/hermes-video-editing) | 5 | — | — | — | Professional video editing skill: AI captioning, silence removal, scene detection, stabilisation, smart reframing. | — |
| [video-analytics-agent](https://github.com/AgenticAI-Ind/video-analytics-agent) | 0 | — | — | — | Enterprise video analysis agent: automatic transcription, scene detection, object tracking. | — |
| [SceneDetect](https://github.com/Breakthrough/PySceneDetect) | 5.2k | — | — | — | Video scene cut detection: content-aware and threshold-based, CLI + Python API. | — |
| [Kinocut](https://github.com/KyaniteLabs/kinocut) | 193 | — | — | — | Guardrailed video editing MCP server for AI agents. FFmpeg, Hyperframes, quality gates, Shorts/Reels repurposing. Apa... | — |
| [mcp-video](https://github.com/ipythonist/mcp-video) | 4 | — | — | — | Video intelligence MCP server: keyframe extraction, transcripts, analysis from 1000+ sites. | — |
| [ai-video-editor-review](https://github.com/vidio-research/ai-video-editor-review) | 2 | — | — | — | Collaborative open-access review of AI-powered video editing techniques (2025-2026). | — |
| [chatcut](https://github.com/ArtCog/chatcut) | — | Python | — | — | One command turns raw talking-head footage into a finished video — transcribe → cut pauses & stumbles → subtitles → m... | — |
| [video-clip-agent](https://github.com/neopen/video-clip-agent) | 39 | Python | — | — | AI video editing agent: analyzes footage, audio, emotion, then auto-trims, selects clips, syncs beats, adds subtitles... | — |
| [Director](https://github.com/video-db/Director) | 1.5k | — | — | — | Video Agent Framework: Search/Edit/Compile/Generate. Repo literally named "Director". | [▶](https://www.youtube.com/watch?v=Dncn_0RWrro) |
| [Monet](https://github.com/Monet-AI-Editor/Monet) | 116 | — | — | — | Coding-agent-native Video Editor: Timeline + Codex/Claude Code + MCP + Remotion. | — |
| [opencut](https://github.com/floomhq/opencut) | 7 | TypeScript | Active | 2026-09-29 | The open-source video editor built on Remotion — browser-based, React-driven timeline. | — |
| [auto-video-editor](https://github.com/benpiper/auto-video-editor) | 12 | Python | Active | 2026-08-25 | Auto-detect and remove silence, filler words, and freeze frames from videos — web UI + REST API. | — |
| [Clypra](https://github.com/AIEraDev/Clypra) | 3.3k | Rust | Active | 2026-09-30 | Hardware-accelerated video editor on Rust + Tauri v2 + React 19, sub-10ms frame delivery. | — |
| [vanta](https://github.com/itsjwill/vanta) | 132 | TypeScript | Active | 2026-07-26 | Open-source AI video engine on Remotion: voice cloning, AI avatars, animated captions. | — |
| [dissect](https://github.com/0xpratzyy/dissect) | 24 | — | Active | 2026-10-01 | Reverse-engineer any video (YouTube, TikTok, Reels, X) into a reusable blueprint for recreating it. | — |
| [remocn-studio](https://github.com/Remocn/remocn-studio) | 149 | TypeScript | Active | 2026-10-01 | Agent-native video editor: one sentence in, a rendered video out. | — |
| [short-video-maker (mushigaite)](https://github.com/mushigaite/short-video-maker) | 68 | Python | Active | 2026-10-05 | Free open-source tool turning YouTube videos into viral short videos. | — |
| [OpenCardboard](https://github.com/rakesh0x/OpenCardboard) | 57 | TypeScript | Active | 2026-10-04 | Local-first chat-to-edit AI video editor — your footage never leaves your machine. | — |

## Agentic Production Systems & Short-Video Pipelines

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) | 127.1k | — | — | — | Topic/keyword → HD short video via LLMs + automation. The category king. | — |
| [OpenMontage](https://github.com/calesthio/OpenMontage) | 64.8k | — | — | — | Open-source agentic video production: 12 pipelines, 100+ tools, 700+ agent skills. | — |
| [MoneyPrinterV2](https://github.com/FujiwaraChoki/MoneyPrinterV2) | 32.0k | — | — | — | Automate the process of making money online. | [▶](https://youtu.be/wAZ_ZSuIqfk) |
| [Pixelle-Video](https://github.com/ATH-MaaS/Pixelle-Video) | 28.5k | — | — | — | AI fully automated short-video engine. | [▶](https://www.bilibili.com/video/BV1WzyGBnEVp) |
| [hypit](https://github.com/hypit-ai/hypit) | 19.9k | — | — | — | Clone any viral video with AI agents: face, words, B-roll, whole workflow. | — |
| [Toonflow](https://github.com/HBAI-Ltd/Toonflow-app) | 16.6k | — | — | — | Infinite canvas + agents + visual workflows for video/storyboard/short-drama creation. | — |
| [huobao-drama](https://github.com/chatfire-AI/huobao-drama) | 15.6k | — | — | — | 火宝短剧：一句话生成完整短剧，剧本到成片全自动. | — |
| [waoowaoo](https://github.com/waooAI/waoowaoo) | 14.3k | — | — | — | Industry-grade AI agent platform for controllable film & video production. | — |
| [ViMax](https://github.com/HKUDS/ViMax) | 12.5k | — | — | — | Agentic video generation: director, screenwriter, producer, generator all-in-one. | — |
| [OpenCreator](https://github.com/krillinai/OpenCreator) | 12.5k | — | — | — | Formerly KrillinAI: Codex-powered AI workspace for creators. | — |
| [ShortGPT](https://github.com/RayVentura/ShortGPT) | 8.0k | — | — | — | AI framework for YouTube Shorts / TikTok channel automation. | [▶](https://youtu.be/hpoSHq-ER8U) |
| [MoneyPrinterPlus](https://github.com/ddean2009/MoneyPrinterPlus) | 7.2k | — | — | — | Batch short-video generation + auto-publish to Douyin/Kuaishou/Xiaohongshu/Channels. | [▶](https://www.bilibili.com/video/BV16VVGefEp1) |
| [dramaclaw](https://github.com/dramaclaw/dramaclaw) | 6.6k | — | — | — | General-purpose AIGC video engine: script → finished film in one pipeline. | [▶](https://www.bilibili.com/video/BV1iQV26cE4S) |
| [Jellyfish](https://github.com/Forget-C/Jellyfish) | 6.5k | — | — | — | End-to-end workspace for AI short dramas: script → storyboard → cut. | — |
| [ArcReel](https://github.com/ArcReel/ArcReel) | 5.3k | — | — | — | Novels/scripts → assets, storyboards, video and JianYing drafts; cross-shot consistency. | — |
| [youtube-automation-agent](https://github.com/darkzOGx/youtube-automation-agent) | 4.1k | — | — | — | AI agents run a YouTube channel 24/7: create, optimize, publish. | — |
| [ai-podcast-generator](https://github.com/gordonho/ai-podcast-generator) | 0 | — | — | — | AI podcast video generator: script → TTS → avatar animation → video output. | — |
| [AiToEarn](https://github.com/yikart/AiToEarn) | 26.6k | — | — | — | Full-stack AI content growth & monetization: video creation + distribution + analytics. | [▶](https://www.youtube.com/watch?v=5041jEKaiU8) |
| [screenplay-agent](https://github.com/596600892/screenplay-agent) | 0 | — | — | — | AI screenplay writing and video scene generation: logline to Hollywood-format script + MoneyPrinterTurbo bridge. | — |
| [script-to-storyboard](https://github.com/lookme2012/script-to-storyboard) | 14 | — | — | — | AI-assisted screenplay + storyboard: 8-step workflow, multi-LLM, Electron desktop app. | — |
| [ClipForge-CLI](https://github.com/gitstq/ClipForge-CLI) | 0 | — | — | — | Lightweight terminal AI short video script generator: 7 styles, storyboard, multi-format export, TUI dashboard. | — |
| [ai-video-generation-pipeline](https://github.com/SainathPattipati/ai-video-generation-pipeline) | 8 | — | — | — | End-to-end AI video: concept to script to storyboard to consistent characters to video. | — |
| [awesome-generative-ai-apps](https://github.com/Anil-matcha/awesome-generative-ai-apps) | 3.4k | — | — | — | 50+ open-source AI SaaS templates: video tools, headshot generators, one-click deploy. | [▶](https://www.youtube.com/watch?v=X_kbyQyhgmI) |
| [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) | 140.3k | — | — | — | 100+ AI agents & skills: meme generator, music, podcast, video analysis agents. | — |
| [Free-AI-Social-Media-Scheduler](https://github.com/Korexer/Free-AI-Social-Media-Scheduler) | — | — | — | — | Free AI social media scheduler: auto-post videos with optimal timing. | — |
| [vox-ai-motion-graphics-generator](https://github.com/Anil-matcha/vox-ai-motion-graphics-generator) | 242 | Python | High | 2025-09 | Turn any topic into a Vox-style paper-collage explainer video with script, animation, voice-over and captions | [▶](https://www.youtube.com/watch?v=chK_pnV1wqQ) |
| [aimv-studio](https://github.com/shaozheng0503/aimv-studio) | 20 | Python | Active | 2026-09-10 | Multi-agent MV generation system: AI composes music, writes lyrics, generates visuals, edits final video. | — |
| [bang-story](https://github.com/bangtutorial/bang-story) | 71 | TypeScript | Active | 2026-10-02 | Desktop app (Indonesian): turn a story idea into a finished YouTube video with AI (from the bang-motion author). | — |

## MCP & Control Layers

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [mcp-for-blender](https://github.com/ahujasid/mcp-for-blender) | 29.7k | — | — | — | Community plugin to control Blender 3D with any LLM. [▶ Demo](https://www.youtube.com/watch?v=I29rn92gkC4) | [▶](https://www.youtube.com/watch?v=I29rn92gkC4) |
| [scenario-labs/skills](https://github.com/scenario-labs/skills) | 898 | — | — | — | Production-ready images, video, audio and 3D from any AI agent. | — |
| [blend-ai](https://github.com/HoldMyBeer-gg/blend-ai) | 151 | — | — | — | MCP server for Blender: 186 tools for modeling, materials, rendering and more, driven by Claude / Cursor. | — |
| [blender-mcp-bridge](https://github.com/seehiong/blender-mcp-bridge) | 65 | — | — | — | Automate Blender modeling via MCP: 93 tools incl. sculpting, architecture/MEP, materials. | — |
| [blender-mcp-pro](https://github.com/youichi-uda/blender-mcp-pro) | 31 | — | — | — | MCP server with 100+ tools: lights, modifiers, animation, shader nodes, geometry nodes. | — |
| [Blender-Extension](https://github.com/suryansh00001/Blender-Extension) | 25 | — | — | — | In-Blender LLM assistant: natural language → 3D creations instantly. | — |
| [mcp-blender](https://github.com/RFingAdam/mcp-blender) | 19 | — | — | — | 218 tools for 3D modeling, AI generation and MSFS content creation. | — |
| [video-generation-mcp](https://github.com/ricleedo/video-generation-mcp) | 0 | — | — | — | MCP server for video generation: text-to-video, image-to-video via Kling, MiniMax, fal.ai APIs. | — |
| [xai-mcp-server](https://github.com/joemccann/xai-mcp-server) | 1 | — | — | — | MCP server for xAI Grok APIs including video generation capabilities. | — |
| [browser-automation](https://github.com/howar31/browser-automation) | 0 | — | — | — | Claude Code skill for driving a real headless browser (Puppeteer + Playwright) — screenshots, network intercept, CDP ... | — |
| [video-audio-mcp](https://github.com/misbahsy/video-audio-mcp) | 87 | Python | Medium | 2025-07 | FFmpeg-powered MCP server for video/audio editing: format conversion, trimming, overlays, transitions | — |
| [ffmpeg-skill](https://github.com/MastroMimmo/ffmpeg-skill) | 21 | Python | Medium | 2025-08 | Natural language video editing skill for Claude Code — 18 commands covering cut, merge, compress, subtitle, GIF, wate... | — |
| [short-video-maker](https://github.com/gyoridavid/short-video-maker) | 1.4k | TypeScript | Active | 2026-09-20 | Short-video generator: script → TTS voiceover → auto subtitles → background footage → MP4. | — |

## Video Skills: Product Films, Promos & Explainers

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | 10.5k | TypeScript | Active | 2026-09-28 | Cinematic product videos with Remotion for Claude Code & Codex: 152 shot recipe cards, 209 motion presets. [▶ Demo 1]... | [▶](https://youtu.be/gcVvRM_P3SM) |
| [pixel2motion](https://github.com/nolangz/pixel2motion) | 2.4k | Python | Active | 2026-08-21 | Turn raster logos into smooth SVG animation, animated HTML demos, GIF/video previews. | — |
| [anything2explainer](https://github.com/Vincentwei1021/anything2explainer) | 2.3k | TypeScript | Active | 2026-09-18 | Topic in, narrated black-canvas explainer video out. | — |
| [lanshu-create-ai-presenter-video](https://github.com/cclank/lanshu-create-ai-presenter-video) | 2.4k | Python | Active | 2026-09-27 | Provider-neutral Codex skill for verified AI presenter videos from a script. | — |
| [video-talkcraft](https://github.com/Vincentwei1021/video-talkcraft) | 1.4k | HTML | Active | 2026-09-22 | Claude Code / Codex as a motion-design studio for voiceover-driven explainer videos. | — |
| [hyperframes-student-kit](https://github.com/nateherkai/hyperframes-student-kit) | 1.2k | HTML | Active | 2026-09-28 | Edit videos, reels and Shorts with Codex or Claude Code: 14 skills, transcript-driven cuts, 406 motion presets. | — |
| [video-spec-builder](https://github.com/feicaiclub/video-spec-builder) | 1.0k | JavaScript | Active | 2026-05-18 | Forces "I want a video" into a second-precise storyboard spec (`video-spec.md`), then hands it to HyperFrames. One-li... | — |
| [onetake](https://github.com/feitangyuan/onetake) | 1.8k | Python | Active | 2026-09-29 | Motion films that never cut: every beat grows out of the previous one, one continuous camera. | — |
| [capcut-cli](https://github.com/renezander030/capcut-cli) | 833 | JavaScript | Active | 2026-09-28 | The CapCut/JianYing CLI any LLM agent can drive: zero dependencies, JSON in/out, build drafts from scratch. | [▶](https://www.youtube.com/watch?v=cl8SP3PjspQ) |
| [pyJianYingDraft](https://github.com/GuanYixuan/pyJianYingDraft) | 4.5k | Python | Active | 2026-09-26 | Lightweight Python library to generate and export JianYing (剪映) drafts for automated edit pipelines. | — |
| [pyCapCut](https://github.com/GuanYixuan/pyCapCut) | 687 | Python | Active | 2026-09-30 | CapCut-targeted sibling of pyJianYingDraft: generates and exports CapCut drafts from Python. | — |
| [bang-motion](https://github.com/bangtutorial/bang-motion) | 568 | HTML | Active | 2026-09-15 | Browser motion graphics: openers, promos, bumpers, kinetic typography, 5 explainer styles. | — |
| [Orkas-VideoStudio](https://github.com/Orkas-AI/Orkas-VideoStudio) | 497 | TypeScript | Active | 2026-09-22 | Turn your coding agent into a video studio: describe a video in plain language; the agent writes the timeline and ren... | — |
| [motion-video-kit](https://github.com/echris6/motion-video-kit) | 1.1k | Python | Active | 2026-09-28 | Claude Code skill kit for premium business videos with an independent critic loop. | — |
| [llm-video-maker](https://github.com/GoldLegendW80/llm-video-maker) | 26 | JavaScript | Active | 2026-06-17 | One prompt → finished MP4, for Claude Code / Cursor / Codex / Windsurf. | — |
| [brand-motion-design-skill](https://github.com/ouerf-man/brand-motion-design-skill) | 30 | JavaScript | Active | 2026-09-27 | Showreel-grade brand motion videos (launch, promo, teaser) in code with HyperFrames. | — |
| [claude-promo-video](https://github.com/smit-vanani/claude-promo-video) | 15 | JavaScript | Active | 2026-07-16 | Website URL → premium, beat-locked product promo video with Remotion. | — |
| [motion-skills](https://github.com/iart-ai/motion-skills) | 729 | HTML | Active | 2026-09-23 | 50 open-source skills that teach your AI coding agent motion graphics, animation & video. | — |
| [hyperframes-motion-director](https://github.com/geekjourneyx/hyperframes-motion-director) | 450 | JavaScript | Active | 2026-07-26 | Chinese-first HyperFrames motion-video production from articles, products and websites. | — |
| [remotion-video-skill](https://github.com/wshuyi/remotion-video-skill) | 384 | Python | Active | 2026-01-25 | A Claude Code skill for creating programmatic videos with the Remotion framework. | — |
| [super-video-maker-skill](https://github.com/Bomx/super-video-maker-skill) | 305 | Python | Active | 2026-08-09 | One skill, many engines: HeyGen avatars, Seedance b-roll, OpenAI images, Remotion & HyperFrames. | — |
| [marketing-studio](https://github.com/ucsandman/marketing-studio) | 248 | JavaScript | Active | 2026-09-06 | Create product-launch assets with Remotion, then review & distribute through guarded dry-runs. | — |
| [erduo-broll-loop-engineering](https://github.com/erduo1998-cell/erduo-broll-loop-engineering) | 205 | TypeScript | Active | 2026-09-21 | SRT-driven b-roll agent skill: auto-routes HyperFrames / Remotion, ships with 152 Shotcraft shot cards. | — |
| [film-studio-skills](https://github.com/machina-exm/film-studio-skills) | 143 | — | Active | 2026-08-14 | 7 installable skills that run the pipeline behind $2M AI video productions — script to locked cut. | — |
| [claude-motion-design](https://github.com/howseen-ai/claude-motion-design) | 282 | — | — | — | Motion design videos in pure code: HTML + Playwright + ffmpeg. No After Effects. | — |
| [Claude-Code-Video-Toolkit](https://github.com/wilwaldon/Claude-Code-Video-Toolkit) | 88 | — | — | — | Skills, MCP servers and tools for producing video with Claude Code (Remotion & friends). | — |
| [super-prototyping](https://github.com/ReScienceLab/super-prototyping) | 87 | — | — | — | Idea → logo → product → brand → launch video in two hours, for AI agents. | — |
| [vox-director](https://github.com/Alisa0808/vox-director) | 2.2k | — | — | — | One topic → finished Vox-style paper-collage explainer/ad video, end to end. | — |
| [guizang-product-video-skill](https://github.com/op7418/guizang-product-video-skill) | 697 | — | — | — | 归藏's skill: reuse real product components & design language to make software-update promos with code — storyboard, or... | — |
| [motion-graphics-skill](https://github.com/AidenChenCode/motion-graphics-skill) | 0 | — | — | — | A Claude Code skill that turns a brand brief (optionally plus a reference video) into a finished motion-graphics MP4. | — |
| [video-production-skills](https://github.com/Pluviobyte/video-production-skills) | 666 | — | Active | 2026-07-14 | Reusable AI video production skills: creation, recreation, motion design, openers. | — |
| [reelbench-skills](https://github.com/eternityspring/reelbench-skills) | 850 | — | Active | 2026-09-21 | Learning notes and tooling skills for AI video workflows. | — |
| [simon-skills](https://github.com/trustfuture/simon-skills) | 324 | — | Active | 2026-09-24 | Faceless video-channel skills: research long-form + hand-drawn whiteboard explainers, one-line topic to finished video. | — |
| [editor-pro-max](https://github.com/Hainrixz/editor-pro-max) | 257 | TypeScript | Active | 2026-03-26 | AI-powered video editor built with Remotion + Claude Code: describe the video you want. | — |
| [one-prompt-video-skills](https://github.com/huangbai-AI/one-prompt-video-skills) | 86 | — | Active | 2026-09-29 | One sentence → complete talking-head video: scriptwriting, digital-human presenter, b-roll, HyperFrames compositing, frame-level QA (Claude Code skills). | — |
| [adu-motion-video](https://github.com/adunext/adu-motion-video) | 168 | — | Active | 2026-09-28 | 阿杜 × Opus 5.5 motion-template skill: pick a template & style, cut talking-head footage and assets into video; 11,028 curated Lottie animations. | — |
| [whiteboard-video](https://github.com/Cuongyd196/whiteboard-video) | 27 | — | Active | 2026-09-30 | Turn a topic, script or SRT into a finished whiteboard hand-drawn video: the agent writes, draws and narrates. | — |
| [nd-video-studio](https://github.com/vakovalskii/nd-video-studio) | 20 | — | Active | 2026-09-29 | Explainer videos from HTML (HyperFrames → MP4) with AI narrator, music and mixing — Claude Code skill. | — |
| [xilo-opus-video](https://github.com/Kianzzz/xilo-opus-video) | 26 | — | Active | 2026-09-28 | Opus 5.5 code-rendered video: three concepts with previews first, frame-by-frame rendering after approval (Canvas / WebGL / Three.js / Remotion / HyperFrames). | — |
| [livecanvas](https://github.com/pengchujin/livecanvas) | 417 | Swift | Active | 2026-09-30 | Turn one sentence into a Live Photo with a designed cover and animation (live image / animated cover). | — |
| [motion-video-skill](https://github.com/unclejobs-ai/motion-video-skill) | 102 | Python | Active | 2026-10-02 | Claude Code skill (Korean): motion graphics & video production workflow with step-by-step verification gates (30–90s clips). | — |
| [motionmaxxing](https://github.com/Tejashmakwana/motionmaxxing) | 75 | JavaScript | Active | 2026-10-06 | Looksmaxxing for motion graphics: an agent skill that polishes AI-slop videos into films with real motion design. | — |
| [kar-plain](https://github.com/Burntgogi/kar-plain) | 42 | HTML | Active | 2026-10-05 | Compact Codex/Claude skill (Korean/English) that explains topics in four formats — prose, diagrams, web pages and video. Inspired by Karpathy. | — |
| [ecommerce-video-skills](https://github.com/xianyu110/ecommerce-video-skills) | 35 | Python | Active | 2026-10-04 | 12 个电商短视频 Agent Skills：3秒钩子、卖点分镜、图生视频提示词、edge-tts 配音、字幕花字、ffmpeg 自动成片，导出抖音/TikTok Shop/视频号格式。 | — |
| [mortiflix-oss](https://github.com/GTKottman/mortiflix-oss) | 242 | JavaScript | Active | 2026-10-05 | A motion design studio on your own machine: Claude builds the video step by step, you approve each stage. | — |

## Video Skills: Short Drama, Story & Recap

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [drama-skills](https://github.com/zenstory-ai/drama-skills) | 2.6k | — | — | — | AI short-drama / comic-drama suite: script, character assets, storyboards, image/video prompts, review. Claude Code &... | — |
| [video-recap-skills](https://github.com/zenstory-ai/video-recap-skills) | 554 | — | — | — | Video → Chinese narration recap (影视解说): scene detection, ASR, VLM, script, render. | — |
| [handdraw-story-video](https://github.com/xiejunjie524/handdraw-story-video) | 775 | — | — | — | Hand-drawn story video skill: turn any story into a hand-drawn animated short with narration. | — |
| [Open-AI-Micro-Drama-Generator](https://github.com/Anil-matcha/Open-AI-Micro-Drama-Generator) | 518 | Python | — | — | AI short drama & micro-drama video generator: turns any idea into a complete short-form drama using multi-agent AI pi... | — |
| [story-to-handdrawn-video](https://github.com/gnipbao/story-to-handdrawn-video) | 2.2k | — | Active | 2026-09-22 | Agent skill: Chinese story copy or ordered images → hand-drawn diary-comic animation video. | — |
| [html-anime](https://github.com/blixvip/html-anime) | 16 | — | Active | 2026-09-27 | HTML anime generator: prompt a scene, get a shot sheet, render with Claude / Codex / Cursor (from the NullMotion author). | — |
| [cinematic-film](https://github.com/minosdevs/cinematic-film) | 21 | TypeScript | Active | 2026-09-30 | Claude Code skill: turn any subject into a cinematic animated film with Remotion + three.js. | — |
| [vocaloid-style-mv-pipeline](https://github.com/EGSECDA/vocaloid-style-mv-pipeline) | 52 | JavaScript | Active | 2026-10-04 | Production pipeline + Claude Code skill for Vocaloid-style hand-drawn lyric music videos. | — |
| [Muse-animated-short-film](https://github.com/sonlovinbot/Muse-animated-short-film) | 31 | — | Active | 2026-10-03 | Skill (Vietnamese) for making animated short films on Muse AI — idea to MP4: characters, script, keyframes. | — |

## manim & Math-Education Videos

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [manim-skill](https://github.com/Yusuke710/manim-skill) | 165 | — | — | — | SKILL.md for manim: the coding agent autonomously plans scenes and writes the animation code. | — |
| [Math-To-Manim](https://github.com/HarleyCoops/Math-To-Manim) | 2.7k | — | — | — | Multi-pipeline Manim generation (Claude/Gemini/Kimi K2.5), 55+ examples across physics, math, CS. | — |
| [3brown1blue](https://github.com/AmitSubhash/3brown1blue) | 36 | — | — | — | First-principles manim skill for Claude Code: mathematical animation from scratch, paper-explainer style. | — |
| [math-concept-film](https://github.com/liangdabiao/math-concept-film) | 30 | — | — | — | 你说一个数学概念，AI 还你一部带旁白的数学动画短片（Claude Code / Codex）. | [▶](https://www.bilibili.com/video/BV1ws4R6fEHh) |
| [recursive-math-animator](https://github.com/Science-Prof-Robot/recursive-math-animator) | 13 | — | — | — | Cursor / Claude Code skill: manim + manim-voiceover, git-based scene versioning. | — |
| [animus](https://github.com/KacemMathlouthi/animus) | 15 | — | — | — | Agent producing narrated, research-grounded explainer videos with code-driven visuals. | — |
| [Chalkboard](https://github.com/nicglazkov/Chalkboard) | 9 | — | — | — | Multi-agent pipeline: any topic → narrated manim animation. | — |
| [manim-skill (awesome-skills)](https://github.com/awesome-skills/manim-skill) | 7 | — | — | — | Manim animation skill for technical blogs and education. | — |
| [manim-skill (vumichien)](https://github.com/vumichien/manim-skill) | 6 | — | — | — | Ideas, papers and math → manim animations via a 4-role Claude Code agent pipeline. | — |
| [paper2video](https://github.com/edwardyen724-g/paper2video) | 6 | — | — | — | Any technical article → 2–5 min 3Blue1Brown-style explainer video, end to end. | — |
| [notes-to-video](https://github.com/cymcymcymcym/notes-to-video) | 5 | — | — | — | Notes → animated explainers in the style popularized by 3Blue1Brown. | — |
| [ManimML](https://github.com/helblazer811/ManimML) | 3.5k | — | — | — | Animations and visualizations of common machine learning concepts with Manim Community Library. | — |
| [manim_graphic](https://github.com/theaashaychahande/manim_graphic) | 0 | — | — | — | Premium motion-graphics animation built entirely in Python with Manim CE. Particle systems, 3D pop-out, camera zooms,... | — |
| [manim-plugintemplate](https://github.com/ManimCommunity/manim-plugintemplate) | 78 | — | — | — | Official scaffold for developing custom Manim plugins with project structure and tests. | — |
| [Code2Video](https://github.com/showlab/Code2Video) | 2.1k | Python | — | — | Agentic, code-centric framework generating educational videos from knowledge points via executable Manim code. Tri-Ag... | — |
| [TheoremExplainAgent](https://github.com/TIGER-AI-Lab/TheoremExplainAgent) | 1.5k | Python | — | — | Dual-agent system (Planner + Coder) that auto-generates up to 10-minute theorem explanation videos via Manim animatio... | — |
| [ManimCat](https://github.com/Wing900/ManimCat) | 464 | Python | Active | 2026-09-26 | AI-generated math animations from natural language, with high-quality manim rendering. | — |
| [KimiK3Manim](https://github.com/HarleyCoops/KimiK3Manim) | 143 | Python | Active | 2026-07-29 | Math & physics explainer animations generated with Kimi K3. | — |
| [manim-notebook](https://github.com/Manim-Notebook/manim-notebook) | 49 | Python | Active | 2026-08-05 | ManimGL with interactive previewing inside VSCode. | [▶](https://youtu.be/rbu7Zu5X1zI) |

## Modeling Cases & Skills

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [holo-card-studio](https://github.com/EverettFish/holo-card-studio) | 1.9k | — | — | — | Description or reference image → finished, editable Blender holo-card: layered compositing, GLB export, Three.js view... | — |
| [camera-to-blender](https://github.com/ahujasid/camera-to-blender) | 842 | — | — | — | Take a photo of real objects and paste them into Blender. | — |
| [GameFactory-3A](https://github.com/OpenDCAI/GameFactory-3A) | 839 | — | — | — | Comprehensive open-source 3A game-generation skill and asset framework. | — |
| [CozyClay](https://github.com/NomaDamas/CozyClay) | 761 | — | — | — | Open-source previs in the browser: block a scene, pose characters, author camera moves. | — |
| [3dviz-pro-max](https://github.com/viettranx/3dviz-pro-max) | 680 | — | — | — | Agent skill for creative 3D visualization: idea → explorable Three.js/Blender scene. | — |
| [RuiC-card-skill](https://github.com/HRuiCcc/RuiC-card-skill) | 501 | — | — | — | One sentence → draggable, glowing 3D holo-card web page, with an editable Blender project. | — |
| [awesome-astra-prompts](https://github.com/TripoGrowthLab/awesome-astra-prompts) | 327 | — | — | — | 200+ curated GPT-6 Astra prompts and 3D examples for games, Blender scenes and interactive worlds. | — |
| [autoremesher-blender-bridge](https://github.com/adriflex/autoremesher-blender-bridge) | 301 | — | — | — | Blender bridge for AutoRemesher: quad-remesh assets inside agent pipelines. | — |
| [blender-skills](https://github.com/arjun988/blender-skills) | 272 | — | — | — | 94 specialist Blender skills for Cursor / Claude Code / Kiro / Codex: MCP-powered production pipelines. | — |
| [blender-skills (kevinbadi)](https://github.com/kevinbadi/blender-skills) | 140 | — | — | — | Blender skills for Claude Code: 3D product generation and camera-animation workflows. | — |
| [cc-blender-skill](https://github.com/RobLe3/cc-blender-skill) | 84 | — | — | — | Drive Blender 5.x like a senior 3D artist via natural language: 10 chain-loadable skills. | — |
| [BlenderXAlpha-3DGenSkill](https://github.com/ig-shadow-walker/BlenderXAlpha-3DGenSkill) | 29 | — | — | — | Plain-English scene descriptions → AI-generated 3D models built live in Blender. | — |
| [blender-kiln](https://github.com/elithril/blender-kiln) | 29 | — | — | — | Blender skill + plugin for Claude Code: text brief → production GLB asset pipeline. | — |
| [awesome-3d-prompts](https://github.com/TripoGrowthLab/awesome-3d-prompts) | 16 | — | — | — | 3D prompts for games, scenes, assets, animation and interactive worlds across Astra, Claude and Kimi. | — |
| [RemakeBench/skills](https://github.com/RemakeBench/skills) | 11 | — | — | — | Evidence-driven Claude Code skills for building and verifying playable 3D worlds. | — |
| [claude-code-handbook](https://github.com/ThamJiaHe/claude-code-handbook) | 206 | — | — | — | Practical guide to making programmatic videos using Claude Code and Remotion: setup, core concepts, prompt templates,... | — |

## Seedance & Video-Generation-Model Workflows

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [seedance2-skill](https://github.com/dexhunter/seedance2-skill) | 4.2k | — | — | — | Skill to create the best prompts for generating videos with Seedance 2.0. | — |
| [seedance-prompt-skill](https://github.com/songguoxs/seedance-prompt-skill) | 2.9k | — | — | — | Seedance 2.0 视频提示词生成 skill. | — |
| [awesome-seedance](https://github.com/ZeroLu/awesome-seedance) | 2.6k | — | — | — | The ultimate collection of high-fidelity Seedance 2.0 prompts and resources. | — |
| [Seedance2-Storyboard-Generator](https://github.com/liangdabiao/Seedance2-Storyboard-Generator) | 2.5k | — | — | — | Novel/story → structured Seedance 2.0 storyboard script, open-source drama skill. | — |
| [awesome-seedance (LearnPrompt)](https://github.com/LearnPrompt/awesome-seedance) | 1.8k | — | — | — | Evidence-led Seedance 2.5/2.0 prompt library: 463 cases traced to original posts. | — |
| [manju-laoli-skill](https://github.com/lixiaoxiao9888-create/manju-laoli-skill) | 1.1k | — | — | — | 漫剧老李 AIGC 全流程技能包：模型三选一锁（Seedance 等）+ 工业化短剧产线. | — |
| [higgsfield-seedance2-jineng](https://github.com/beshuaxian/higgsfield-seedance2-jineng) | 874 | — | — | — | Seedance 2.0 × Higgsfield: 15 Claude prompt skills — cinematic, 3D CGI, anime, e-commerce. | — |
| [seedance2.0-prompt-skill](https://github.com/MapleShaw/seedance2.0-prompt-skill) | 803 | — | — | — | Seedance 2.0 prompt skill. | — |
| [make-prompt-seedance2](https://github.com/liangdabiao/make-prompt-seedance2) | 685 | — | — | — | Seedance 2.0 结构化提示词与通用 skill. | [▶](https://www.bilibili.com/video/BV17qb26vEED) |
| [higgsfield-ai-prompt-skill](https://github.com/OSideMedia/higgsfield-ai-prompt-skill) | 698 | — | — | — | 32 sub-skills covering Seedance 2.5 (omni-reference, video-to-video…). | — |
| [ai-shortfilm-prompts](https://github.com/jnMetaCode/ai-shortfilm-prompts) | 458 | — | — | — | Idea → cinematic, model-ready prompts for Sora · Kling · Veo · Seedance. | — |
| [cinematic-video-prompt-skill](https://github.com/Rylaispirit/cinematic-video-prompt-skill) | 146 | — | — | — | AI video prompt cheat sheet & Claude skill: camera angles, movement, lighting, composition. | — |
| [awesome-seedance-2.5-prompts-skills](https://github.com/AtlasCloudAI/awesome-seedance-2.5-prompts-skills) | 222 | — | — | — | 100+ Seedance 2.5 prompts with real video previews + installable agent skill. | — |
| [Happy-Horse-1.1](https://github.com/CalvintheBear/Happy-Horse-1-1-Released) | 0 | — | — | — | Alibaba 15B model: T2V/I2V/R2V + native audio + 7-language lip-sync, #1 Video Arena. | — |
| [visual-skills](https://github.com/smixs/visual-skills) | 481 | — | Active | — | AI Film Director Skills: Murch Editing, Blocking, Montage, Cinematography, Seedance 2.5 Syntax. Pure Skill approach. | — |
| [Seedance-ShotDesign-Skills](https://github.com/woodfantasy/Seedance-ShotDesign-Skills) | 119 | — | — | — | Shot Design / Director Skill for Seedance 2.5: 4–180s, Extend, Multi-ref, partial editing, Viewpoint Reconstruction, ... | — |
| [seedance-tvc-director](https://github.com/nutllwhy/seedance-tvc-director) | 293 | — | — | — | Seedance 2.5 TVC Director: 15s/30s/Custom TVC, Shot Planning, VO Routing, Evidence-driven Retake. | — |
| [Seedance-CLI](https://github.com/L1angjy/Seedance-CLI) | 1 | — | — | — | Seedance/Dreamina CLI: Agent-facing toolkit for video generation task submission + download. Works with OpenClaw, Her... | — |
| [ai-media-generator](https://github.com/Hao0321/ai-media-generator) | 254 | — | — | — | AI Media Agent Skill: auto-create Senior Director-level prompts, shots, references, cross-platform generation. | — |

## Open-Source Video Generation Models

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [Wan2.2](https://github.com/Wan-Video/Wan2.2) | 17.7k | — | — | — | Open large-scale video generative models. | — |
| [CogVideo](https://github.com/zai-org/CogVideo) | 13.0k | — | — | — | CogVideoX (2024) & CogVideo (ICLR 2023). | [▶](https://www.youtube.com/watch?v=5UCkMzP2VLE) |
| [HunyuanVideo](https://github.com/Tencent-Hunyuan/HunyuanVideo) | 12.6k | — | — | — | Tencent's systematic framework for large video generation. | — |
| [LTX-Video](https://github.com/Lightricks/LTX-Video) | 11.0k | — | — | — | Official LTX-Video repository. | — |
| [LTX-2](https://github.com/Lightricks/LTX-2) | 9.6k | — | — | — | LTX-2 audio–video generative model: inference & LoRA trainer. | — |
| [VideoCrafter](https://github.com/AILab-CVC/VideoCrafter) | 5.1k | — | — | — | High-quality video diffusion under data limitations. | [▶](https://www.youtube.com/watch?v=0NfmIsNAg-g) |
| [HunyuanVideo-1.5](https://github.com/Tencent-Hunyuan/HunyuanVideo-1.5) | 4.6k | — | — | — | Leading lightweight video generation model. | — |
| [FastVideo](https://github.com/hao-ai-lab/FastVideo) | 4.5k | — | — | — | Unified inference & post-training for accelerated video generation. | — |
| [SkyReels-V2](https://github.com/SkyworkAI/SkyReels-V2) | 7.6k | — | — | — | Infinite-length video generation model: auto-regressive diffusion for film-length content. | — |
| [VACE](https://github.com/ali-vilab/VACE) | 4.0k | — | — | — | [ICCV 2025] All-in-one video creation and editing. | — |
| [Self-Forcing](https://github.com/guandeh17/Self-Forcing) | 3.5k | — | — | — | Bridging training & inference in autoregressive video diffusion. | — |
| [Open-Sora-V1.2](https://github.com/hpcaitech/Open-Sora) | 29.9k | — | — | — | Open-source Sora replication V1.2: 3D VAE + DiT, multi-resolution, single-GPU inference. | [▶](https://www.bilibili.com/video/BV1ow4m1e7PX) |
| [Vchitect-2.0](https://github.com/Vchitect/Vchitect-2.0) | 921 | — | — | — | Sparse-to-dense video generation: progressive training for high-quality T2V. | — |
| [Stable-Video-Diffusion](https://github.com/Stability-AI/generative-models) | 27.3k | — | — | — | Stability AI SVD: image-to-video diffusion, camera control, 25 frames at 6fps. | [▶](https://www.youtube.com/watch?v=dtqj-s50ynU) |
| [AnimateDiff](https://github.com/guoyww/AnimateDiff) | 12.3k | — | — | — | Personalize text-to-image models for video without tuning: motion module injection. | — |
| [ModelScope-T2V](https://github.com/modelscope/modelscope) | 9.2k | — | — | — | Alibaba ModelScope text-to-video: 1.7B model, multi-stage training, open weights. | — |
| [I2VGen-XL](https://github.com/ali-vilab/I2VGen-XL) | 9 | — | — | — | Alibaba image-to-video: high-quality, consistent with input image, stylizable. | — |
| [Show-1](https://github.com/showlab/Show-1) | 1.1k | — | — | — | NUS Show Lab: pixel-level T2V via interleaved frame-by-frame and segment-level generation. | — |
| [Open-Sora-Plan](https://github.com/PKU-YuanGroup/Open-Sora-Plan) | 12.2k | — | — | — | PKU open-source Sora plan: CausalVid VAE + DiT, progressive training. | [▶](https://youtu.be/IiWTdx2EHCY) |
| [Prompt-A-Video](https://github.com/jiyt17/Prompt-A-Video) | 25 | — | — | — | ICCV 2025: LLM-based prompt booster for text-to-video, reward-based evolution + DPO. | — |
| [Allegro](https://github.com/rhymes-ai/Allegro) | 1.1k | — | — | — | Rhymes AI: high-quality text-to-video, 15s 1080p, DiT architecture. | — |
| [Sana](https://github.com/NVlabs/Sana) | 9.2k | — | — | — | NVIDIA: high-resolution image & video generation via linear DiT, 4K output. | [▶](https://www.youtube.com/watch?v=ztdkfIMkdJ4) |
| [OpenVid](https://github.com/NJU-PCALab/OpenVid-1M) | 471 | — | — | — | Open video generation benchmark: 1M text-video pairs, evaluation toolkit. | — |
| [Wan2.1](https://github.com/Wan-Video/Wan2.1) | 17.1k | Python | Active | — | Alibaba Wan 2.1/2.2: MoE architecture, 1.3B–14B variants. First open-source MoE video generation model. 8GB VRAM for ... | — |
| [Mochi](https://github.com/genmoai/mochi) | 3.7k | Python | — | — | Genmo Mochi 1: ~10B parameters, strongest photorealism among open-source video models. Best fine-tuning base with off... | — |
| [VideoTuna](https://github.com/VideoVerses/VideoTuna) | 554 | Python | — | — | All-in-one video generation codebase: inference & fine-tune T2V/I2V/T2I/V2V models. Supports Wan2.1, HunyuanVideo, Co... | — |
| [ConsisID](https://github.com/PKU-YuanGroup/ConsisID) | 862 | Python | — | — | Identity-preserving text-to-video generation by frequency decomposition (CVPR 2025 Highlight). Tuning-free DiT-based ... | [▶](https://www.youtube.com/watch?v=PhlgC-bI5SQ) |
| [MagicTime](https://github.com/PKU-YuanGroup/MagicTime) | 1.3k | Python | — | — | Time-lapse video generation models as metamorphic simulators (TPAMI 2025). ChronoMagic dataset with 460K pairs. | [▶](https://www.bilibili.com/video/BV1wx421U7Gn) |
| [Latte](https://github.com/Vchitect/Latte) | 1.9k | Python | Active | 2025-03 | Latent Diffusion Transformer for Video Generation. TMLR 2025. Supports T2V and T2I with temporal decoder VAE. | — |
| [FasterCache](https://github.com/Vchitect/FasterCache) | 268 | Python | Active | 2024-11 | Training-free video diffusion model acceleration. ICLR 2025. Supports Open-Sora, CogVideoX, Latte, Mochi, Vchitect 2.0. | — |
| [UniAnimate](https://github.com/ali-vilab/UniAnimate) | 1.2k | Python | Active | 2025-04 | Unified video diffusion for consistent human image animation. SCIS 2025. Supports long video generation with first-fr... | — |
| [SCEPTER](https://github.com/modelscope/scepter) | 550 | Python | Active | 2025-01 | Open-source framework for generative training, fine-tuning, and inference. Supports FLUX, SD3, CogVideoX, ACE++, Comf... | — |
| [CausVid](https://github.com/tianweiy/CausVid) | 1.4k | Python | Medium | 2025-06 | CVPR 2025 — 4-step autoregressive video generation at 9.4 FPS with causal attention | — |
| [Helios](https://github.com/PKU-YuanGroup/Helios) | 2.2k | Python | Medium | 2025-05 | Minute-level video generation at 19.5 FPS via progressive training | [▶](https://www.youtube.com/watch?v=vd_AgHtOUFQ) |
| [LightX2V](https://github.com/ModelTC/LightX2V) | 2.9k | Python | High | 2025-08 | Lightweight video generation inference framework supporting multiple models | — |
| [StreamingVLM](https://github.com/mit-han-lab/streaming-vlm) | 1.1k | Python | Medium | 2025-03 | Streaming vision-language model for real-time video understanding | — |

## Digital Humans, Voice & Toolchain

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [Deep-Live-Cam](https://github.com/hacksider/Deep-Live-Cam) | 96.9k | — | — | — | Real-time face swap with a single image. Use responsibly. | [▶](https://www.youtube.com/watch?v=OlNWCpFdVMA) |
| [VoiceStudio](https://github.com/debpalash/VoiceStudio) | 54.4k | — | — | — | Fully-local ElevenLabs alternative: voice cloning, design, video dubbing. | — |
| [LivePortrait](https://github.com/KlingAIResearch/LivePortrait) | 19.1k | — | — | — | Bring portraits to life (Kling team). | — |
| [Duix-Avatar](https://github.com/duixcom/Duix-Avatar) | 15.6k | — | — | — | Open-source digital-human toolkit: offline video generation & cloning. | — |
| [video-subtitle-remover](https://github.com/YaoFANGUK/video-subtitle-remover) | 13.1k | — | — | — | AI hard-subtitle/watermark removal, fully local. | [▶](https://b23.tv/guEbl9C) |
| [video-subtitle-extractor](https://github.com/YaoFANGUK/video-subtitle-extractor) | 9.5k | — | — | — | Hard-coded subtitles → SRT via local OCR, GUI included. | [▶](https://www.bilibili.com/video/bv11L4y1Y7Tj) |
| [EchoMimicV2](https://github.com/antgroup/echomimic_v2) | 4.7k | — | — | — | [CVPR 2025] Semi-body human animation. | [▶](https://www.youtube.com/watch?v=2ab6U1-nVTQ) |
| [PersonaLive](https://github.com/GVCLab/PersonaLive) | 3.9k | — | — | — | [CVPR 2026] Expressive portrait animation for live streaming. | — |
| [MiniMax CLI](https://github.com/MiniMax-AI/cli) | 2.2k | — | — | — | Generate text, images, video, speech and music from the command line. | — |
| [douyin-mcp-server](https://github.com/yzfly/douyin-mcp-server) | 1.3k | — | — | — | MCP server / skill: watermark-free Douyin links + transcripts. | — |
| [comfyui-mcp](https://github.com/artokun/comfyui-mcp) | 793 | — | — | — | Agent-native control plane for ComfyUI: MCP server + sidebar agent. | — |
| [Lumi-Digital-Human](https://github.com/QwenchC/Lumi-Digital-Human) | 2 | — | — | — | Local streaming digital human: real-time lip-sync, multiple TTS engines, browser-based. | — |
| [Talking-Head](https://github.com/Bomou-AI/Talking-Head) | 38 | — | — | — | 100+ languages, 350+ voice models. Open-source talking-head video generation. | — |
| [Talking-Avatar](https://github.com/Bomou-AI/Talking-Avatar) | 14 | — | — | — | Avatar animation from Talking-Head: facial expression + body gesture sync. | — |
| [ip-human-agent](https://github.com/fa1314/ip-human-agent) | 53 | — | — | — | Super IP Agent 4.0: digital human oral broadcast full-chain automation. | — |
| [dlp3d.ai](https://github.com/dlp3d-ai/dlp3d.ai) | 363 | — | — | — | SIGGRAPH Asia 2025: open-source autonomous 3D character (LLM + 3D avatar). | [▶](https://www.youtube.com/watch?v=cNEMW6IHKl8) |
| [Motion-Agent](https://github.com/szqwu/Motion-Agent) | 123 | — | — | — | ICLR 2025: LLM dialogue framework for human motion generation. | — |
| [awesome-motion-style-transfer](https://github.com/GuangtaoLyu/awesome-motion-style-transfer) | 1 | — | — | — | Auto-updated list of human motion style transfer and stylized motion generation papers. | — |
| [MuseTalk](https://github.com/TMElyralab/MuseTalk) | 6.7k | — | — | — | Tencent Music: real-time lip-sync for talking heads, 30fps+ on consumer GPU. | — |
| [MuseV](https://github.com/TMElyralab/MuseV) | 2.8k | — | — | — | Tencent Music: infinite-length virtual human video via diffusion, consistent identity. | [▶](https://www.bilibili.com/video/BV1ux4y1v7pF) |
| [ER-NeRF](https://github.com/Fictionarry/ER-NeRF) | 1.3k | — | — | — | Efficient region-aware NeRF for talking-head: real-time, high-fidelity. | [▶](https://youtu.be/Gc2d3Z8MMuI) |
| [GeneFace++](https://github.com/yerfor/GeneFacePlusPlus) | 1.8k | — | — | — | ICLR 2024: generalized NeRF-based talking-face with audio-to-motion domain adaptation. | — |
| [AniPortrait](https://github.com/Zejun-Yang/AniPortrait) | 5.0k | — | — | — | Tencent: audio + reference portrait → expressive animation, diffusion-based. | [▶](https://www.bilibili.com/video/BV1H4421F7dE) |
| [Hallo](https://github.com/fudan-generative-vision/hallo) | 8.7k | — | — | — | Fudan: hierarchical audio-driven portrait animation, high-fidelity lip-sync. | — |
| [Awesome-AIGC-Image-Video-Detection](https://github.com/ant-research/Awesome-AIGC-Image-Video-Detection) | 460 | — | — | — | AI-generated image & video detection: datasets, benchmarks, papers, tools. | [▶](https://www.bilibili.com/video/BV1teuc63E6D) |
| [Open-AI-UGC](https://github.com/Anil-matcha/Open-AI-UGC) | 349 | JavaScript | — | — | Free, open-source alternative to Arcads and MakeUGC. Generate AI UGC video ads with realistic AI actors using Veo 3.1... | — |
| [Wav2Lip](https://github.com/Rudrabha/Wav2Lip) | 13.2k | Python | — | — | Lip-sync for any face in any video: accurate lip movement generation from audio. | [▶](https://youtu.be/0fXaDCZNOJc) |
| [facefusion](https://github.com/facefusion/facefusion) | 30.1k | Python | — | — | Next-generation face swapping and enhancement tool. Most mature repo for face-centric video edits. | — |
| [ChatTTS](https://github.com/2noise/ChatTTS) | 39.9k | Python | — | — | Open-source high-quality Chinese TTS. Natural prosody with laughter and pause modeling. | [▶](https://www.bilibili.com/video/BV1zn4y1o7iV) |
| [CosyVoice](https://github.com/FunAudioLLM/CosyVoice) | — | Python | — | — | Multi-lingual large voice generation model from Alibaba: TTS, voice cloning, cross-lingual synthesis. | — |
| [GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS) | 62.3k | Python | — | — | Few-shot voice cloning & TTS: 1-minute reference audio → voice clone. Zero-shot and few-shot modes. | [▶](https://www.bilibili.com/video/BV12g4y1m7Uw) |
| [EchoMimicV3](https://github.com/antgroup/echomimic_v3) | 1.1k | Python | — | — | 1.3B parameters for unified multi-modal and multi-task human animation. Audio-driven talking face and body animation. | [▶](https://www.bilibili.com/video/BV1W8tdzEEVN) |
| [MimicTalk](https://github.com/yerfor/MimicTalk) | 830 | Python | — | — | NeRF-based talking face: 15-minute training for personalized 3D talking head. Audio-driven, highly realistic. | — |
| [OpenAvatarChat](https://github.com/HumanAIGC-Engineering/OpenAvatarChat) | 3.8k | Python | — | — | Open-source platform for creating lifelike digital avatars with real-time interaction. Realistic expressions, low-lat... | [▶](https://www.bilibili.com/video/BV1sv8QzLEC2) |
| [Wan-Animate](https://github.com/wan-animate/wananimate) | 6 | Python | — | — | Unified AI framework for character animation and replacement by Alibaba. Animate photos with reference video movement... | — |
| [Fay](https://github.com/xszyou/Fay) | 13.6k | Python | — | — | Real-time conversational digital human system integrating ASR, TTS, and LLM. Virtual anchor, voice assistant scenarios. | — |
| [KodaCut](https://github.com/wade56754/KodaCut) | 4 | Python | Active | 2026-07 | Open-source AI talking-head editing agent for Chinese creators. Rough cut, compact captions, evidence-driven B-roll, ... | — |
| [TEN-framework](https://github.com/TEN-framework/ten-framework) | 11.1k | Go | Active | 2026-08 | Open-source framework for real-time multimodal conversational AI. Voice assistant, lip-sync avatars, SIP calls, ESP32... | — |
| [awesome-heygen-ai-alternatives](https://github.com/furudo-erika/awesome-heygen-ai-alternatives) | 18 | — | Moderate | 2025-08 | Curated list of open-source HeyGen alternatives for AI talking-head and digital human video generation. | — |
| [Duix-Mobile](https://github.com/duixcom/Duix-Mobile) | 8.3k | Kotlin | High | 2025-09 | Real-time interactive AI avatar with on-premise deployment and <1.5s latency for mobile | — |
| [Linly-Talker](https://github.com/Kedreamix/Linly-Talker) | 3.5k | Python | Active | 2026-02-10 | Digital avatar conversational system: LLM + talking-head + voice, interactive digital human. | [▶](https://www.bilibili.com/video/BV1rN4y1a76x) |
| [Qwen3-TTS](https://github.com/QwenLM/Qwen3-TTS) | 13.6k | Python | Active | 2026-03-17 | Qwen team's open-source TTS model series: multilingual, zero-shot voice cloning. | — |
| [Qwen3-Audiobook-Converter](https://github.com/WhiskeyCoder/Qwen3-Audiobook-Converter) | 1.1k | Python | Active | 2026-04-07 | PDF/EPUB/DOCX/TXT → high-quality audiobooks with Qwen3-TTS. | — |
| [yovoice](https://github.com/leemysw/yovoice) | 367 | — | Active | 2026-09-29 | Open-source voice creation for macOS/Windows: local TTS, voice cloning, emotion control. | — |
| [speech-studio](https://github.com/soniqo/speech-studio) | 68 | — | Active | 2026-08-30 | Desktop voice-cloning studio for creators: clone a voice, script lines with emotion. | [▶](https://www.youtube.com/watch?v=EuIU8tOWyzg) |

## Video Translation & Lip Sync

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [LatentSync](https://github.com/bytedance/LatentSync) | 6.1k | — | — | — | ByteDance lip-sync from audio: Stable Diffusion latent diffusion for end-to-end lip-synced video generation. | — |
| [SadTalker](https://github.com/OpenTalker/SadTalker) | 14.1k | — | — | — | Static portrait + audio → talking head video: 3D face model driven by audio features, lightweight. | [▶](https://www.bilibili.com/video/BV1Dc411W7V6) |
| [YouDub](https://github.com/liuzhao1225/YouDub) | 615 | Python | — | — | YouTube video auto-localization: download → separate audio → recognize → translate → voice clone → re-encode with Chi... | — |
| [video-retalking](https://github.com/OpenTalker/video-retalking) | 7.3k | Python | Active | 2026-08-10 | Audio-driven lip-sync for talking-head video — synchronize mouth movements with any audio. | — |
| [VideoLingo](https://github.com/Huanshere/VideoLingo) | 18.5k | Python | Active | 2026-09-27 | Netflix-level subtitle cutting, translation, alignment and dubbing — one-click, fully automated. | — |
| [YouDub-webui](https://github.com/liuzhao1225/YouDub-webui) | 5.6k | Python | Active | 2026-09-22 | YouDub with a WebUI: AI video localization & dubbing for YouTube/Bilibili. | [▶](https://www.youtube.com/watch?v=ii9Kh4XkA5g) |
| [SmartSub](https://github.com/buxuku/SmartSub) | 5.6k | — | Active | 2026-09-30 | One-stop desktop tool: subtitles from video, translation, AI dubbing & voice cloning, burn-in. Local Whisper/FunASR. | — |
| [Auto-Synced-Translated-Dubs](https://github.com/ThioJoe/Auto-Synced-Translated-Dubs) | 1.7k | Python | Active | 2026-05-11 | Translate a video from its subtitles and generate AI voice dubs synced to the original timing. | — |
| [SoniTranslate](https://github.com/R3gm/SoniTranslate) | 1.4k | Python | Active | 2026-08-29 | Synchronized translation for videos: dubbing with voice cloning and subtitle alignment. | [▶](https://www.youtube.com/watch?v=SmGkFaSzq_Q) |
| [violin](https://github.com/shang-zhu/violin) | 1.1k | — | Active | 2026-09-04 | Open-source video translation skill for coding agents. | — |
| [video-translator](https://github.com/InsiderX-Pro/video-translator) | 929 | — | Active | 2026-06-17 | Real-time video translation / dubbing skill. | — |
| [Pandrator](https://github.com/lukaszliniewicz/Pandrator) | 628 | Python | Active | 2026-09-27 | PDFs/EPUBs → audiobooks; subtitles or videos → dubbed videos with translated TTS. | — |
| [CapCap](https://github.com/notepower2k1/CapCap) | 341 | — | Active | 2026-09-23 | Windows desktop app for short-form video localization and dubbing. | — |
| [youtube-auto-dub (heyncth)](https://github.com/heyncth/youtube-auto-dub) | 304 | Python | Active | 2026-07-22 | YouTube auto-dubbing pipeline: Whisper transcribe → translate → TTS re-voice. | — |
| [youtube-auto-dub (mazzasaverio)](https://github.com/mazzasaverio/youtube-auto-dub) | 73 | Python | Active | 2026-09-29 | Local-first YouTube dubbing that clones the original voice into another language. | — |

## Video Subtitle, Transcription & Translation Tools

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [whisper](https://github.com/openai/whisper) | 109.8k | — | — | — | OpenAI Whisper: robust speech recognition for transcription and subtitle generation, supports 99 languages. | — |
| [faster-whisper](https://github.com/SYSTRAN/faster-whisper) | 25.6k | — | — | — | 4x faster Whisper inference with CTranslate2, lower memory, popular for production pipelines. | [▶](https://www.youtube.com/watch?v=0u7tTptBo9I) |
| [whisperX](https://github.com/m-bain/whisperX) | 24.3k | — | — | — | Word-level timestamps + speaker diarization for Whisper, essential for precise subtitle alignment. | — |
| [FunClip](https://github.com/modelscope/FunClip) | 6.4k | — | — | — | FunASR-powered video transcription, subtitle generation, and LLM-assisted clipping with local Gradio UI. | — |
| [AutoSubtitle](https://github.com/Linwei-Chen/AutoSubtitle) | 14 | — | — | — | AI video subtitle generator with Whisper + LLM translation, supports multilingual SRT/VTT output. | — |
| [autosubtitlegenerator](https://github.com/snigdhasingh77/autosubtitlegenerator) | 0 | — | — | — | Free auto subtitle generator: Next.js + FastAPI + Whisper, supports SRT/VTT export and subtitle burn-in. | — |
| [pyvideotrans](https://github.com/jianchang512/pyvideotrans) | 19.2k | — | — | — | Video translation + dubbing + subtitle tool: ASR → LLM translate → TTS → video synthesis, 50+ languages. | — |
| [Linly-Dubbing](https://github.com/Kedreamix/Linly-Dubbing) | 3.3k | — | — | — | Intelligent multilingual AI dubbing & translation with lip sync, voice cloning, subtitle alignment. | — |
| [NarratoAI](https://github.com/linyqh/NarratoAI) | 11.3k | Python | — | — | Automated film/TV narration: auto-clip + voiceover + subtitles. Non-commercial license. | — |
| [autoclip](https://github.com/zhouxiaoka/autoclip) | 9.1k | Python | — | — | AI highlight extraction from long videos: YouTube/Bilibili download → AI analysis → extract best moments → compile. | — |
| [subtitle-burner](https://github.com/july-lyan/subtitle-burner) | 4 | Python | Medium | 2025-04 | Whisper auto-transcription + one-click subtitle burning to video with web UI | — |
| [whisper-ctranslate2](https://github.com/Softcatala/whisper-ctranslate2) | 1.4k | Python | Active | 2026-09-22 | Whisper speech recognition using CTranslate2 — 4x faster than OpenAI's original implementation. | — |
| [video-subtitle-generator](https://github.com/YaoFANGUK/video-subtitle-generator) | 1.2k | Python | Moderate | 2024-02-01 | Audio → SRT subtitles, fully local Transformer ASR, GUI included. | — |
| [SoloPup Subtitle Studio](https://github.com/OakcoderX/solopup-subtitle-studio) | 0 | Python | Active | 2026-10-28 | Local SDH and Chinese-to-English subtitle review; offline paired-SRT import, optional Qwen assistance, ITT/SRT export. MIT; public preview; cloud AI may cost money. | — |


## Video Enhancement, Super-Resolution & Restoration

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [FlashVSR](https://github.com/OpenImagingLab/FlashVSR) | 1.9k | — | — | — | Real-time diffusion VSR: one-step streaming at ~17 FPS on single A100, 4x upscaling. | — |
| [STCDiT](https://github.com/JyChen9811/STCDiT) | 78 | — | — | — | CVPR 2026: spatio-temporally consistent diffusion Transformer for high-quality video super-resolution. | — |
| [NanoVSR](https://github.com/filippawlicki/nanovsr) | 52 | — | — | — | ECCV 2026: real-time 4x VSR on edge devices (Jetson Orin NX), 644k params, ONNX/TensorRT compatible. | — |
| [Anime4K](https://github.com/bloc97/Anime4K) | 21.4k | — | — | — | Lightweight shader-driven upscaling for anime/line art, real-time capable, GPU-accelerated. | — |
| [rife-ncnn-vulkan](https://github.com/nihui/rife-ncnn-vulkan) | 1.1k | — | — | — | Real-time frame interpolation on GPU (Vulkan), drop-in for video interpolation pipelines. | — |
| [rembg](https://github.com/danielgatis/rembg) | 24.9k | — | — | — | Background removal tool using U2-Net, essential for compositing video assets and digital humans. | — |
| [demucs](https://github.com/adefossez/demucs) | 8.5k | — | — | — | Music source separation: vocals, drums, bass, other — critical for video dubbing and BGM isolation. | — |
| [ultimatevocalremovergui](https://github.com/Anjok07/ultimatevocalremovergui) | 26.4k | — | — | — | GUI for AI vocal/removal with MDX-Net and VR architecture, popular for content creators. | — |
| [VideoEraser](https://github.com/bluedream02/VideoEraser) | 14 | — | — | — | [EMNLP 2025] Concept erasure in T2V diffusion: remove objects, celebrities, styles from generated video. | — |
| [Real-ESRGAN-ncnn-vulkan](https://github.com/xinntao/Real-ESRGAN-ncnn-vulkan) | 2.2k | — | — | — | Real-time video super-resolution on GPU: ncnn inference, no Python needed. | — |
| [BasicVSR++](https://github.com/ckkelvinchan/BasicVSR_PlusPlus) | 830 | — | — | — | CVPR 2022: video super-resolution with bidirectional propagation and alignment. | — |
| [RealBasicVSR](https://github.com/ckkelvinchan/RealBasicVSR) | 1.1k | — | — | — | CVPR 2022: practical video restoration, degradation-aware adapter. | — |
| [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) | 37.0k | Python | — | — | Blind super-resolution for noisy/compressed/low-res footage. Default open-source restoration tool for editors. | [▶](https://www.youtube.com/watch?v=fxHWoDSSvSc) |
| [GFPGAN](https://github.com/TencentARC/GFPGAN) | 37.7k | Python | — | — | Blind face restoration for interview edits, social clips, archival scans. Pairs well with Real-ESRGAN. | — |
| [CodeFormer](https://github.com/sczhou/CodeFormer) | 18.2k | Python | — | — | Transformer-based face restoration balancing fidelity and perceptual quality. Useful for degraded faces in old footage. | [▶](https://youtu.be/d3VDpkXlueI) |
| [RIFE](https://github.com/hzwer/Practical-RIFE) | 1.0k | Python | — | — | Real-Time Intermediate Flow Estimation for video frame interpolation. Smooth slow-motion and frame rate conversion. | [▶](https://www.bilibili.com/video/BV1J3411t7qT) |
| [ProPainter](https://github.com/sczhou/ProPainter) | 7.0k | Python | — | — | Video inpainting for object removal, watermark removal, and completion. Essential for cleanup workflows. | [▶](https://youtu.be/92EHfgCO5-Q) |
| [frame-interpolation](https://github.com/google-research/frame-interpolation) | 3.2k | Python | Active | 2026-06-20 | Google Research's large-motion frame interpolation model — FILM for smooth slow-motion from any two frames. | [▶](https://www.youtube.com/watch?v=OAD-BieIjH4) |
| [Video2X](https://github.com/k4yt3x/video2x) | 21.9k | C++ | Active | 2026-09-25 | ML-based video super-resolution and frame interpolation framework — Real-ESRGAN + RIFE + waifu2x. | [▶](https://youtu.be/mGEfasQl2Zo) |
| [RobustVideoMatting](https://github.com/PeterL1n/RobustVideoMatting) | 9.5k | Python | Active | 2026-07-10 | Robust High-Resolution Video Matting — real-time alpha matting without green screen. | [▶](https://youtu.be/Jvzltozpbpk) |
| [obs-backgroundremoval](https://github.com/royshil/obs-backgroundremoval) | 4.6k | C++ | Active | 2026-09-20 | OBS Studio plugin for real-time background removal in portrait video — no green screen needed. | [▶](https://youtu.be/jC3EKSpNjQk) |
| [BRIA-RMBG-2.0](https://github.com/BRIA-AI/RMBG-2.0) | 330 | Python | Active | 2026-08-30 | State-of-the-art background removal model — commercial-grade accuracy for images and video. | — |
| [BasicSR](https://github.com/XPixelGroup/BasicSR) | 8.4k | Python | Moderate | 2024-07-21 | Open-source image & video restoration toolbox: super-resolution, denoise, deblurring (Real-ESRGAN's home). | — |
| [SparkVSR](https://github.com/taco-group/SparkVSR) | 740 | Python | Active | 2026-08-03 | [ECCV 2026] Interactive video super-resolution via sparse keyframe propagation. | — |
| [FAST_Anime_VSR](https://github.com/Kiteretsu77/FAST_Anime_VSR) | 74 | Python | Moderate | 2024-01-02 | Fast anime video super-resolution & restoration (Real-CUGAN + Real-ESRGAN + VCISR). | — |

## ComfyUI Video Ecosystem & Custom Nodes

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [ComfyUI-AnimateDiff-Evolved](https://github.com/Kosinkadink/ComfyUI-AnimateDiff-Evolved) | 3.5k | — | — | — | AnimateDiff integration for ComfyUI: motion modules, sliding context, batch scheduling. | — |
| [ComfyUI-VideoHelperSuite](https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite) | 1.9k | — | — | — | Video import, frame extraction, combine-to-video, and format conversion nodes for ComfyUI. | — |
| [ComfyUI-LTXVideo](https://github.com/Lightricks/ComfyUI-LTXVideo) | 4.1k | — | — | — | LTX-Video model support for ComfyUI: text-to-video and image-to-video workflows. | — |
| [ComfyUI-WanVideoWrapper](https://github.com/kijai/ComfyUI-WanVideoWrapper) | 6.7k | — | — | — | Wan video model wrapper for ComfyUI: Wan 2.1/2.2 T2V/I2V with LoRA support. | — |
| [ComfyUI-Manager](https://github.com/Comfy-Org/ComfyUI-Manager) | 16.3k | — | — | — | ComfyUI package manager: install/update custom nodes, models, and workflows from UI. | — |
| [ComfyUI_FlashVSR](https://github.com/smthemex/ComfyUI_FlashVSR) | 397 | — | — | — | FlashVSR super-resolution node for ComfyUI: real-time 4x video upscaling. | — |
| [comfyui_loops](https://github.com/dicksensei69/comfyui_loops) | 1 | — | — | — | Simple ComfyUI loop node: creates seamless back-and-forth loop animations from image sequences. | — |
| [ComfyUI-vidflows](https://github.com/kustomzone/ComfyUI-vidflows) | — | — | — | — | ComfyUI video workflows: Sora2-ComfyUI, Veo 3, Story Creator node packs. | — |
| [ComfyUI-Agent-Kit](https://github.com/SlavaSexton/comfyui-agent-kit) | 105 | Python | Active | — | One ComfyUI skill for every AI coding agent (Claude Code, Codex, Gemini CLI, Qwen Code): 75 model prompt recipes, 581... | — |
| [ComfyUI-Frame-Interpolation](https://github.com/Fannovel16/ComfyUI-Frame-Interpolation) | 1.1k | Python | Active | 2026-03-29 | Video frame interpolation node set for ComfyUI. | — |
| [Steerable-Motion](https://github.com/banodoco/Steerable-Motion) | 974 | Python | Active | 2025-10-03 | Drive videos with batches of images — keyframe-steered motion in ComfyUI. | — |
| [ComfyUI-LatentSyncWrapper](https://github.com/ShmuelRonen/ComfyUI-LatentSyncWrapper) | 963 | Python | Active | 2025-09-04 | LatentSync lip-sync node for ComfyUI. | — |
| [ComfyUI-QwenVL](https://github.com/1038lab/ComfyUI-QwenVL) | 898 | Python | Active | 2026-09-14 | Qwen-VL series nodes (Qwen2.5-VL, Qwen3-VL) for video/image understanding in ComfyUI. | — |
| [comfyui-vrgamedevgirl](https://github.com/vrgamegirl19/comfyui-vrgamedevgirl) | 758 | Python | Active | 2026-09-29 | Film grain, color matching and video enhancement nodes. | — |
| [ComfyUI-PainterI2V](https://github.com/princepainter/ComfyUI-PainterI2V) | 634 | Python | Active | 2026-08-01 | Enhanced Wan2.2 image-to-video node fixing the slow-motion issue. | — |
| [Vibe-Workflow](https://github.com/SamurAIGPT/Vibe-Workflow) | 605 | — | Active | 2026-09-17 | Open-source node canvas for AI media workflows (Weavy/Krea-nodes alternative). | — |
| [ComfyUI_VLM_nodes](https://github.com/gokayfem/ComfyUI_VLM_nodes) | 589 | Python | Active | 2026-08-08 | VLM nodes: Qwen3-VL, Moondream 3, Florence-2, SmolVLM2. | — |
| [Bjornulf_custom_nodes](https://github.com/justUmen/Bjornulf_custom_nodes) | 549 | Python | Active | 2025-06-11 | 163 nodes for text, images, videos, loras and more. | [▶](https://www.youtube.com/watch?v=YiGgyh7nQRg) |
| [ComfyUI-LTXTricks](https://github.com/logtd/ComfyUI-LTXTricks) | 512 | Python | Active | 2025-03-05 | Additional control nodes for the LTX Video model. | — |
| [ComfyUI-HunyuanLoom](https://github.com/logtd/ComfyUI-HunyuanLoom) | 492 | Python | Active | 2025-02-21 | Video editing nodes using the Hunyuan Video model. | — |

## FFmpeg & CLI Video Toolchain

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [video-use](https://github.com/browser-use/video-use) | 28.3k | — | — | — | Edit videos with coding agents: transcript-driven editing via ElevenLabs Scribe + FFmpeg. | — |
| [Auto-Editor](https://github.com/WyattBlue/auto-editor) | 5.4k | — | — | — | Auto-detect and cut silence, muting, and inactive periods from videos; supports many formats. | — |
| [ffsubsync](https://github.com/smacke/ffsubsync) | 7.9k | — | — | — | Synchronize subtitles to video by speech recognition alignment, essential for auto-subtitle pipelines. | — |
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | 194.4k | — | — | — | Command-line video download tool: YouTube, Bilibili, and 1000+ sites, fundamental for video workflows. | [▶](https://www.youtube.com/watch?v=YE7VzlLtp-4) |
| [VideoHighlighter](https://github.com/Aseiel/VideoHighlighter) | 157 | — | — | — | Local AI video analyzer: visual search, auto highlights, scene/object/action detection + subtitles. | — |
| [headless-screen-recorder](https://github.com/brianbaso/headless-screen-recorder) | — | TypeScript | — | — | Puppeteer plugin for headless Chrome screen recording using HeadlessExperimental.beginFrame API. Professional color c... | — |
| [shutter-encoder](https://github.com/paulpacifico/shutter-encoder) | 2.8k | Java | Active | 2026-06 | FFmpeg GUI for video encoding, conversion, and processing. Supports AV1, HEVC, VP9, and many other codecs with batch ... | — |
| [ffmpeg-python](https://github.com/kkroening/ffmpeg-python) | 11.0k | Python | Medium | 2025-04 | Python bindings for FFmpeg with complex filter graph support | — |

## Blender & 3D

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [blender-auto-render](https://github.com/miolini/blender-auto-render) | 3 | — | — | — | Automated Blender rendering pipeline for CI/CD with AI-generated scene scripts. Headless, Docker-compatible. | — |
| [blender-python-toolkit](https://github.com/AleBrito124356/blender-python-toolkit) | 2 | — | — | — | Headless Blender automation: procedural cities, product turntables, batch rendering, data-driven 3D charts. EEVEE-first. | — |
| [3DModelTurntableMaker](https://github.com/TuesdayPoetry/3DModelTurntableMaker) | 1 | — | — | — | Turn any 3D model into looping turntable animation. Blender 5.0 background rendering. 10+ formats. | — |
| [python-blender-video-automation](https://github.com/rbcommoncents/python-blender-video-automation) | 1 | — | — | — | Design-automation project for constructing animated Blender scenes with Python. | — |
| [fake-bpy-module](https://github.com/nutti/fake-bpy-module) | 1.8k | — | — | — | Python API completion stubs for Blender scripting. Essential for IDE autocomplete. | — |
| [blender-production-skills](https://github.com/XliuXjianX/blender-production-skills) | 243 | — | — | — | Blender production skills for Claude Code: 3D modeling, animation, and rendering automation. | — |
| [gsplat](https://github.com/nerfstudio-project/gsplat) | 5.7k | Cuda | Active | 2026-09-20 | Nerfstudio's CUDA Gaussian Splatting library — fast differentiable rasterizer for 3DGS training and rendering. | [▶](https://www.youtube.com/watch?v=ACPTiP98Pf8) |

## Characters, Mocap & Game Assets

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [mixamo-llm-mocap](https://github.com/squall01337/mixamo-llm-mocap) | 345 | — | — | — | Any video → Mixamo-rig animation: GVHMR estimator, spec-driven retarget, FK apply in Blender. | — |
| [blender-game-skills](https://github.com/majidmanzarpour/blender-game-skills) | 131 | — | — | — | Claude Code skills for game dev in Blender: concept art → rigged, game-ready 3D assets. | — |
| [HY-Motion-1.0](https://github.com/Tencent-Hunyuan/HY-Motion-1.0) | 2.6k | Python | Active | 2025-12 | Text-to-3D human motion generation with billion-scale DiT. Three-stage training: pre-training, fine-tuning, RLHF. SOT... | — |
| [FollowYourPose](https://github.com/THUSIGSICLAB/FollowYourPose) | 1 | Python | Moderate | 2024-03 | Pose-guided text-to-video generation using pose-free videos. AAAI 2024. Two-stage training with zero-initialized pose... | — |
| [godmodeanimation](https://github.com/lyogavin/godmodeanimation) | 283 | Python | Moderate | 2025-05 | 2D game animation generation via text-to-video and image-to-video models. AI sprite generator for professional game a... | — |
| [DisPose](https://github.com/lihxxx/DisPose) | 376 | Python | Moderate | 2024-12 | Controlled character image animation by decomposing skeletal pose into motion field guidance and key-point correspond... | — |
| [live2d-motion3](https://github.com/EasyLive2D/live2d-motion3) | 31 | Python | Moderate | 2025-08 | Python implementation of Live2D animation. Read motion3.json, control model animation, visualize curves, and edit mot... | — |

## Real-Time & Interactive Video Generation

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [StreamingT2V](https://github.com/Picsart-AI-Research/StreamingT2V) | 1.6k | — | — | — | Streaming text-to-video: 80+ frame generation with temporal consistency, no autoregression drift. | [▶](https://youtu.be/md4lp42vOGU) |
| [JoyAI-VL-Interaction](https://github.com/jd-opensource/JoyAI-VL-Interaction) | 1.9k | Python | — | — | Open real-time video-language interaction system. 8B vision-first model that watches continuously and responds proact... | — |
| [realtime-ai](https://github.com/realtime-ai/realtime-ai) | 184 | Go | — | — | WebRTC-based real-time AI framework for audio/video processing. Modular pipeline: STT → LLM → TTS. Gemini, OpenAI int... | — |
| [TeleFuser](https://github.com/Tele-AI/TeleFuser) | 31 | Python | — | — | High-performance runtime for world model inference and multimodal generation. Continuous streaming, WebRTC control, d... | — |
| [krea-realtime-video](https://github.com/krea-ai/realtime-video) | 585 | Python | — | — | Krea Realtime 14B: open-source real-time AI video model. Distilled from Wan 2.1 14B using Self-Forcing. 11 fps on B200. | — |
| [CyberVerse](https://github.com/Lynpoint/CyberVerse) | 1.7k | Python | — | — | Self-hosted real-time digital human agent platform. WebRTC, persona memory, tools, RAG, optional digital-human video. | [▶](https://youtu.be/Lk88sew2x4o) |
| [livekit-agents](https://github.com/livekit/agents-js) | 938 | TypeScript | — | — | Build realtime multimodal AI agents with Node.js. WebRTC-based, flexible STT/LLM/TTS integrations, MCP support. | — |

## Video Generation API & Orchestration

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [augstai/awesome-ai-video-generation](https://github.com/augstai/awesome-ai-video-generation) | 9 | — | — | — | AI video generation tools: T2V models, avatars, UGC ad generators, lip sync, open source. | — |
| [vargHQ/sdk](https://github.com/vargHQ/sdk) | 340 | — | — | — | "JSX for videos": one TypeScript API for Kling, Flux, ElevenLabs, Sora, Veed. | — |
| [MiniMax-MCP](https://github.com/MiniMax-AI/MiniMax-MCP) | 1.6k | — | — | — | Official MiniMax MCP server: TTS, image, video generation APIs. | — |
| [minimax-h3-cli](https://github.com/harlowprewitt7/minimax-h3-cli) | 30 | — | Active | 2026-10-04 | MiniMax H3 CLI and video skill guide: installation, model configuration, prompt workflows. | — |

## Adjacent

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [Video-MME](https://github.com/MME-Benchmarks/Video-MME) | 0.8k | Python | — | — | First comprehensive evaluation benchmark of multimodal LLMs in video analysis. 900 videos, 254 hours, 2700 QA pairs (... | — |
| [LVBench](https://github.com/zai-org/LVBench) | 152 | Python | Moderate | 2024-08 | Extreme long video understanding benchmark. Evaluates models on videos up to 2 hours. ICCV 2025. Six core capabilities. | — |
| [VideoLLaMA3](https://github.com/DAMO-NLP-SG/VideoLLaMA3) | 1.2k | Python | Active | 2025-02 | Frontier multimodal foundation models for image and video understanding. Best 7B model on VideoMME and LVBench leader... | — |
| [OVO-Bench](https://github.com/JoeLeelyf/OVO-Bench) | 164 | Python | Moderate | 2025-01 | Online video understanding benchmark. CVPR 2025. Evaluates backward tracing, real-time perception, and forward active... | — |
| [VideoEspresso](https://github.com/hshjerry/VideoEspresso) | 143 | Python | Active | 2025-04 | Large-scale chain-of-thought dataset for fine-grained video reasoning via core frame selection. CVPR 2025 Oral. | — |
| [D3](https://github.com/Zig-HS/D3) | 46 | — | — | — | [ICCV 2025] Training-free AI-generated video detection using second-order features. | — |
| [InternVideo](https://github.com/OpenGVLab/InternVideo) | 2.4k | Python | — | — | Video foundation models & data for multimodal understanding. InternVideo2/2.5 with long and rich context modeling. | — |
| [VideoChat](https://github.com/OpenGVLab/Ask-Anything) | 3.4k | Python | — | — | VideoChatGPT: ChatGPT with video understanding. End-to-end video-centric multimodal dialogue. MVBench benchmark (CVPR... | — |
| [VILA](https://github.com/NVlabs/VILA) | 3.9k | Python | — | — | State-of-the-art vision language models for efficient video understanding and multi-image understanding. NVILA, LongV... | — |
| [TwelveLabs Python SDK](https://github.com/twelvelabs-io/twelvelabs-python) | 51 | Python | Medium | 2025-08 | Python SDK for Twelve Labs video understanding and search API | — |
| [VideoRAG](https://github.com/starsuzi/VideoRAG) | 86 | Python | Medium | 2025-06 | Retrieval-Augmented Generation over video corpus with dynamic video retrieval and multimodal representation | — |
| [VideoRAG-Ren](https://github.com/shuhengchen/VideoRAG_Ren) | 500 | Python | High | 2025-09 | RAG framework for extreme long-context video understanding with dual-channel architecture and knowledge graphs | — |
| [Awesome-Multimodal-RAG](https://github.com/JarvisUSTC/Awesome-Multimodal-RAG) | 54 | — | High | 2025-09 | Curated list of latest advancements in multimodal RAG across text, image, video, and audio | — |
| [gaussian-splatting](https://github.com/graphdeco-inria/gaussian-splatting) | 24.0k | C++ | High | 2025-09 | 3D Gaussian Splatting for real-time radiance field rendering — SIGGRAPH 2023 reference implementation | [▶](https://youtu.be/T_kXY43VZnk) |
| [awesome-gaussians](https://github.com/longxiang-ai/awesome-gaussians) | 358 | — | High | 2025-09 | Auto-updated curated list of 3D Gaussian Splatting papers with 1000+ entries across 15 categories | — |
| [awesome-3D-gaussian-splatting](https://github.com/MrNeRF/awesome-3D-gaussian-splatting) | 8.9k | — | High | 2025-09 | Curated list of papers and resources focused on 3D Gaussian Splatting research | [▶](https://www.youtube.com/watch?v=0xdPpKSkO3I) |
| [Nerfstudio](https://github.com/nerfstudio-project/nerfstudio) | 12.0k | Python | High | 2025-09 | Modular framework for NeRF and 3DGS training, rendering, and evaluation | — |
| [Video-LLaVA](https://github.com/PKU-YuanGroup/Video-LLaVA) | 3.5k | Python | Active | 2026-08-20 | Learning United Visual Representation by Alignment Before Projection for video understanding. | [▶](https://www.youtube.com/watch?v=EFkN00rGq1U) |
| [VBench](https://github.com/Vchitect/VBench) | 1.8k | Python | Active | 2026-09-28 | CVPR 2024 — comprehensive benchmark suite for video generative models with 16 evaluation dimensions. | [▶](https://www.youtube.com/watch?v=7IhCC8Qqn8Y) |
| [Video-Bench](https://github.com/Video-Bench/Video-Bench) | 81 | Python | Active | 2026-09-10 | Human preference aligned video generation benchmark — MLLM-based scoring across 9 dimensions. | [▶](https://www.youtube.com/watch?v=BMvgyWbWPFg) |
| [VGA-Bench](https://github.com/BestiVictory/VGA-Bench) | 3 | Python | Active | 2026-08-20 | CVPR 2026 — unified benchmark for video aesthetics, generation quality, and text-video alignment. | — |
| [physics-IQ-benchmark](https://github.com/google-deepmind/physics-IQ-benchmark) | 365 | Python | Active | 2026-09-15 | DeepMind's benchmark for physical understanding in generative video models — real-world physics scenarios. | — |
| [OpenS2V-Nexus](https://github.com/PKU-YuanGroup/OpenS2V-Nexus) | 231 | Python | Active | 2026-09-20 | NeurIPS 2025 — million-scale dataset and benchmark for subject-to-video generation. | — |

## Adjacent: Unreal, WebGL & 3D Asset Generation

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [unreal-agent-harness](https://github.com/per-simmons/unreal-agent-harness) | 195 | — | — | — | AI agents building cities in Unreal Engine 5.8 via Unreal MCP. | — |
| [webgl-animation-skills](https://github.com/iart-ai/webgl-animation-skills) | 18 | — | — | — | 3D motion / WebGL skills for Claude Code: Three.js, GLSL shaders, particle systems. | — |
| [media2threejs](https://github.com/promptwhisper/media2threejs) | 2 | — | — | — | Rebuild objects, characters and scenes from images/video as editable, animation-ready Three.js. | — |
| [Hunyuan3D-2](https://github.com/Tencent-Hunyuan/Hunyuan3D-2) | 15.0k | — | — | — | High-resolution 3D asset generation with large-scale diffusion models (Tencent). | — |
| [ComfyUI-Trellis2](https://github.com/visualbruno/ComfyUI-Trellis2) | 847 | — | — | — | ComfyUI wrapper for Microsoft Trellis.2 image-to-3D. | — |
| [claude-opus-5-5-demo](https://github.com/riba2534/claude-opus-5-5-demo) | 1.0k | — | — | — | 3D game demo made with Claude Opus 5.5, includes Chinese prompts. | — |

## Related Awesome Lists

| Project | Stars | Language | Activity | Last Update | Description | Demo |
|---------|-------|----------|----------|-------------|-------------|------|
| [awesome-video-generation](https://github.com/backblaze-labs/awesome-video-generation) | 33 | — | — | — | Curated list of AI video generation APIs, SDKs, and tools. Covers commercial services, open source models, and produc... | — |
| [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) | 75.9k | — | — | — | The master list of Claude Skills across all domains. | — |
| [awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) | 35.0k | — | — | — | 1000+ agent skills for Claude Code and friends. | — |
| [Awesome-Video-Diffusion](https://github.com/showlab/Awesome-Video-Diffusion) | 5.8k | — | — | — | Academic-curated video diffusion models. | [▶](https://www.youtube.com/watch?v=QmqWhUjPkJI) |
| [awesome-claude-video-skills](https://github.com/zhuyansen/awesome-claude-video-skills) | 457 | — | — | — | Skills & toolkits for Claude Code / Codex video making. | — |
| [awesome-ai-video](https://github.com/zhaotoday/awesome-ai-video) | 18 | — | — | — | AI 视频生产资源索引（中文）. | — |
| [awesome-video-automation](https://github.com/renezander030/awesome-video-automation) | 4 | — | — | — | Comprehensive index of programmatic video tools and workflows. | — |
| [awesome-ai-media-skills](https://github.com/JuneYaooo/awesome-ai-media-skills) | 5 | — | — | — | Curated Claude Code skills, MCP servers, and agent capabilities for video creation. | — |
| [garden-skills](https://github.com/ConardLi/garden-skills) | 12.7k | — | — | — | Production-grade Agent Skills collection with web video demos. | — |
| [ai-film-skills](https://github.com/62656456/ai-film-skills) | 60 | — | — | — | 21 independent film/TV skill modules: storyboard, director, asset, style management. | — |
| [archify](https://github.com/tt-a1i/archify) | 78.9k | — | — | — | Code → technical diagram Agent Skill (architecture visualization). | — |
| [awesome-ai-video-editing](https://github.com/Supersynergy/awesome-ai-video-editing) | 2 | — | — | — | 110+ agent-native tools: Claude Code skills, MCP servers, CLI pipelines. | — |
| [awesome-ai-agents-2026](https://github.com/caramaschiHG/awesome-ai-agents-2026) | 1.9k | — | — | — | 340+ AI agent resources across 20+ categories, updated monthly. | — |
| [awesome-agent-everything](https://github.com/greasebig/awesome-agent-everything) | 0 | — | — | — | Meta-index of ALL awesome agent repos: frameworks, skills, MCP, safety. | — |
| [awesome-video-super-resolution-diffusion](https://github.com/yjsunnn/Awesome-video-super-resolution-diffusion) | 224 | — | — | — | Curated diffusion-based VSR papers, updated daily from arXiv. | — |
| [Aweosome-Video-Agent](https://github.com/haozheguo/Aweosome-Video-Agent) | 8 | — | — | — | Long-video understanding and Video Agent papers, benchmarks, code. | — |
| [trending-claude-skills](https://github.com/linny006/trending-claude-skills) | 123 | — | — | — | Auto-updated leaderboard of trending agent skills, refreshed every 15 minutes. | — |
| [awesome-ai-image-tools](https://github.com/stimQQ/awesome-ai-image-tools) | 5 | — | — | — | 100+ open-source AI image & video models, libraries, APIs, plugins. | — |
| [awesome-cg-vfx-pipeline](https://github.com/cgwire/awesome-cg-vfx-pipeline) | 1.3k | — | — | — | CG/VFX pipeline resources: asset management, render farms, compositing. | — |
| [awesome-claude-video](https://github.com/opusvideo/awesome-claude-video) | 183 | — | — | — | Bilingual case collection of Claude Opus 5.5 code-rendered videos with prompts. | — |
| [awesome-ai-video-models](https://github.com/Anil-matcha/awesome-ai-video-models) | 197 | — | — | — | Most complete, up-to-date comparison of AI video generation models — which model, via which API, at what price, and h... | [▶](https://www.youtube.com/watch?v=SOXsxqnQGlc) |
| [Awesome-World-Models](https://github.com/NeuraLiying/Awesome-World-Models) | 3 | — | Active | 2026-07 | 340+ world model papers covering video generation, autonomous driving, robotics, 3D/4D, physics simulation, and bench... | — |
| [Awesome-AI4Animation](https://github.com/yunlong10/Awesome-AI4Animation) | 215 | — | Active | 2025-07 | Latest papers, projects and datasets on GenAI for cel-animation. ICCV 2025 AISTORY Workshop. Covers scripting, storyb... | [▶](https://www.youtube.com/watch?v=iUF-LsqFKpI) |
| [awesome-generative-ai](https://github.com/steven2358/awesome-generative-ai) | 12.7k | — | Active | 2026-09 | Curated list of modern generative AI projects and services. Covers text, coding, agents, image, video, and audio gene... | — |
| [top-100-comfyui](https://github.com/liusida/top-100-comfyui) | 422 | — | High | 2025-09 | Auto-updated list of top 100 ComfyUI repositories by GitHub stars | — |
| [awesome-rm-for-video-generation](https://github.com/chrisliu298/awesome-rm-for-video-generation) | 3 | — | Active | 2026-09 | Curated collection of papers, datasets, and code for video reward models. Covers RLHF/DPO/GRPO for video generation a... | — |
| [Awesome-Streaming-Video-Understanding](https://github.com/Yang011013/Awesome-Streaming-Video-Understanding) | 31 | — | Active | 2025-10 | Curated list of research papers and benchmarks on streaming/online video understanding. Covers StreamingVLM, StreamFo... | — |
| [video-cnn-interpretability](https://github.com/MSWEIMZ/video-cnn-interpretability) | 2 | Python | Active | 2026-09 | Automated paper curation for video deep learning & explainability. 808 papers with trending analysis and interactive ... | — |
| [free-voice-clone](https://github.com/0xSojalSec/free-voice-clone) | 637 | — | Active | 2026-04-09 | List of local & free voice-clone TTS and music generation models. | — |
| [awesome-ai-voice](https://github.com/wildminder/awesome-ai-voice) | 499 | — | Active | 2026-09-23 | Curated list of open-source TTS, voice cloning and music generation models. | — |
| [awesome-ai-motion](https://github.com/gongnyang/awesome-ai-motion) | 58 | — | Active | 2026-09-30 | 637 motion techniques for AI video, infographics and scroll decks — rendered clips, recipes, roadmaps. | — |

## On X

Where this scene talks on X (verified via web search, 2026-09-30).

**Accounts to follow**

- [@HeyGen](https://x.com/HeyGen) — HyperFrames launch & updates.
- [@remotion](https://x.com/remotion) — Remotion official.
- [@calesthioailabs](https://x.com/calesthioailabs) — OpenMontage lab.
- [@op7418](https://x.com/op7418) — 归藏, author of the product-video skill.
- [@VincentWei93](https://x.com/VincentWei93) — video-shotcraft / anything2explainer / video-talkcraft.
- [@slimer48484](https://x.com/slimer48484) — mexicat, creator of the pdoom music video.
- [@anshuc](https://x.com/anshuc) — dream-loop (Blender 3D visuals).
- [@seekjourney](https://x.com/seekjourney) — hyperframes-motion-director.
- [@aikangarooking](https://x.com/aikangarooking) — 袋鼠帝, prolific Chinese AI-skills builder.

**Posts & moments**

- [X trending topic: "AI Music Video Champions Progress Over Doom Warnings"](https://x.com/i/trending/2104161956634517980) — the pdoom-video wave, Sept 2026.
- [mrdoob on the pdoom video](https://x.com/mrdoob/status/2104062526950613277) — the three.js author noticing a code-rendered MV.
- [HeyGen's HyperFrames announcement](https://x.com/HeyGen/status/2044827454460871072); see also [AYi: "HeyGen 这次开源，把 AI 做视频的最后一道门槛…"](https://x.com/AYi_AInotes/status/2045310892284199233)
- [OpenMontage discussion](https://x.com/RoundtableSpace/status/2069929815994487022) — also hit #1 on GitHub Trending.
- [Seedance 2.0 flooding timelines](https://x.com/vivimoneya/status/2074748410557759596) — and the paywall debate.
- Trending stats for the pdoom repo are tracked on [trendshift.io](https://trendshift.io/repositories/264721).

## Contributing

Pull requests welcome! Added projects should be open source and related to making video with text models / code / agents (or their workflows). Keep the table format of the section you're editing, and verify star counts when you touch an entry.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this work.
