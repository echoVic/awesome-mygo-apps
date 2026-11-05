# awesome-mygo-apps

> 基于 [egoist/mygo](https://github.com/egoist/mygo)（纯 Go 原生桌面 UI 框架）的**可运行应用与组件库**精选清单 —— 每条都经过 go.mod 依赖实证，可追溯、可复现。

![stars](https://img.shields.io/badge/stars-223%20recommended-F0544E)
![license](https://img.shields.io/badge/license-见各条目-lightgrey)
![collected](https://img.shields.io/badge/data%20collected-2026--11--05-green)
![PR Welcome](https://img.shields.io/badge/PR-welcome-brightgreen)

---

## 生态背景

[mygo](https://github.com/egoist/mygo) 是 2026 年 9 月发布的纯 Go 桌面 UI 框架：无 Electron、无 cgo，GPU 绘制原生 UI，同时支持系统 WebView 承载 Web 前端。截至 2026-11-05，已实测收录 **223 个**基于 mygo 的完整应用、UI 组件库与工具，全部经 go.mod 依赖实证（少数 README 明确声明兜底，证据见 [候选项目盘点表](./候选项目盘点表.md)）。

## 目录

- [框架作者出品（egoist）](#框架作者出品egoist)
- [AI · 智能体](#ai--智能体)
- [编辑器 · 笔记](#编辑器--笔记)
- [终端 · 开发工具](#终端--开发工具)
- [网络 · 代理](#网络--代理)
- [媒体 · 播放下载](#媒体--播放下载)
- [生产力 · 菜单栏](#生产力--菜单栏)
- [系统 · 监控](#系统--监控)
- [游戏 · 趣味](#游戏--趣味)
- [UI 组件库](#ui-组件库)
- [工具 · 其他](#工具--其他)
- [贡献指南](#贡献指南)
- [更新日志](#更新日志)

---

## 框架作者出品（egoist）

mygo 作者 [egoist](https://github.com/egoist) 本人用自家框架写的应用，代表生态最高完成度：

- [egoist/kero](https://github.com/egoist/kero) — 面向 coding agent 的跨平台原生终端。⭐ 1421 · MIT · Release v2.1.33（2026-11-04）
- [egoist/mygo-cloudmusic](https://github.com/egoist/mygo-cloudmusic) — 第三方网易云音乐客户端（已归档：收到网易云音乐下线要求，仓库转为只读）。⭐ 776 · 未声明 · 无 release
- [egoist/lorca](https://github.com/egoist/lorca) — Grok Bot 替代：Rust CLI + MyGo 原生桌面端 + 手机端。⭐ 357 · GPL-3.0 · Release mobile-v1.0.11（2026-10-28）
- [egoist/gorex](https://github.com/egoist/gorex) — Rex 终端克隆，`go tool mygo build` 出 .app/.dmg。⭐ 236 · 未声明 · 无 release
- [egoist/godraw](https://github.com/egoist/godraw) — 无限画布，mygo 原生绘制。⭐ 231 · 未声明 · 无 release
- [egoist/godiff](https://github.com/egoist/godiff) — 原生 diff 查看器。⭐ 137 · 未声明 · 无 release
- [egoist/uma](https://github.com/egoist/uma) — Umami 统计的原生菜单栏应用。⭐ 44 · 未声明 · 无 release

## AI · 智能体

把 LLM / agent 装进原生桌面的聊天客户端、coding agent 前端、语音与转写工具：

- [nexmoe/DayBee](https://github.com/nexmoe/DayBee) — 桌面麦克风录音机：本地实时转写、自动分段与语音活动检测。⭐ 428 · 未声明 · Release v1.1.0（2026-10-18）
- [hehehai/AudioSmith](https://github.com/hehehai/AudioSmith) — Mac 上的语音、配音、有声书、转录与音频工作室。⭐ 217 · AGPL-3.0 · Release v0.5.0-beta.2（2026-11-03）
- [Bronya0/ally-agent](https://github.com/Bronya0/ally-agent) — 面向本地项目的桌面 AI 编程助手，理解代码、编辑文件。⭐ 137 · GPL-3.0 · Release v2.0.0（2026-11-01）
- [AstraFoundry/Arion](https://github.com/AstraFoundry/Arion) — 本地优先的语音输入：端侧识别、离线听写，macOS/Windows。⭐ 112 · AGPL-3.0 · Release v0.1.1（2026-11-03）
- [godwit-email/godwit](https://github.com/godwit-email/godwit) — 开源、可改造的 AI 邮件客户端。⭐ 83 · Apache-2.0 · Release v1.27.0（2026-11-05）
- [enowdev/enowx](https://github.com/enowdev/enowx) — 一个窗口运行并管理 Claude Code、Codex、OpenCode 等 coding agent。⭐ 38 · MIT · Release v0.7.0（2026-11-05）
- [ACAne0320/Tomoru](https://github.com/ACAne0320/Tomoru) — 为电脑上播放的视频、直播、游戏、会议叠加实时双语字幕。⭐ 27 · GPL-3.0 · Release v0.1.3（2026-11-03）
- [lbr77/lody-mygo](https://github.com/lbr77/lody-mygo) — Lody 的第三方原生桌面客户端（GPU 自绘、无 WebView）。⭐ 24 · 未声明 · Release v0.1.1（2026-10-30）
- [aio-proxy/aio-proxy](https://github.com/aio-proxy/aio-proxy) — 本地 AI 网关：一个端点服务 OpenAI/Anthropic/Gemini 客户端，附 MyGo 桌面控制端。⭐ 19 · MIT · Release v0.42.5（2026-10-12）
- [youfun/Handbean](https://github.com/youfun/Handbean) — 跑在本机的 Elixir/OTP 本地 AI agent，MyGo 桌面宿主。⭐ 18 · 未声明 · Release v0.3.6（2026-11-04）
- [kkkk2323/droi](https://github.com/kkkk2323/droi) — Factory Droid 会话的 Mac/Windows/iPhone 原生客户端。⭐ 13 · MIT · Release v1.90.0（2026-11-03）
- [ChisaAlter/ChisaCloudCode](https://github.com/ChisaAlter/ChisaCloudCode) — Windows 上连接云端 AI 编程工作区的桌面客户端。⭐ 9 · AGPL-3.0 · Release v0.1.11（2026-10-20）
- [kotuke/lumilo](https://github.com/kotuke/lumilo) — 本地 LLM 引擎的 macOS 菜单栏面板（Splash / llama.cpp）。⭐ 5 · MIT · Release v0.4.2（2026-10-31）
- [sorrycc/CCGuanjia](https://github.com/sorrycc/CCGuanjia) — 照看 Claude Code 的 Mac 应用（profiles/checklists）。⭐ 5 · MIT · Release v0.1.1（2026-10-22）
- [HycJack/mygo-agent](https://github.com/HycJack/mygo-agent) — Codex 风格的 MyGo 桌面 AI 编程 agent（内置 agent loop、技能与 MCP）。⭐ 3 · 未声明 · 无 release
- [xxww0098/tulai](https://github.com/xxww0098/tulai) — 跨平台批量图生图桌面工具，支持豆包与千问。⭐ 3 · MIT · Release v0.1.11（2026-11-04）
- [horizon0514/ds-search](https://github.com/horizon0514/ds-search) — 基于 DeepSeek Search API 的 macOS 菜单栏极简搜索。⭐ 2 · MIT · Release v0.2.1（2026-10-19）
- [tk103331/ChatGo](https://github.com/tk103331/ChatGo) — 多模型 AI 聊天客户端（Agents、工具、MCP、内置终端）。⭐ 2 · MIT · Release v0.11.0（2026-10-30）
- [Beeta/voxi](https://github.com/Beeta/voxi) — macOS 会议录音转写/摘要助手。⭐ 1 · MIT · Release v0.2.0（2026-10-13）
- [bunnywaffle/llama-manager](https://github.com/bunnywaffle/llama-manager) — llama.cpp 桌面管理器：分支对话、多模型、低占用。⭐ 1 · 未声明 · Release v0.1.7（2026-11-03）
- [hehehai/Auralink](https://github.com/hehehai/Auralink) — macOS 远程模型语音输入：说话即在光标处输入文字。⭐ 1 · AGPL-3.0 · 无 release
- [minifish-org/pith-desk](https://github.com/minifish-org/pith-desk) — 由 Pith 驱动的本地桌面 agent（工作区工具、MCP 连接）。⭐ 1 · AGPL-3.0 · Release v0.1.0-rc.48（2026-10-25）
- [xleotranx/wada_desktop_go](https://github.com/xleotranx/wada_desktop_go) — 原生 Go 桌面 AI 聊天/编程应用，可复用插件架构。⭐ 1 · MIT · 无 release
- [xwjdsh/ivy](https://github.com/xwjdsh/ivy) — 个人 AI agent：终端与 Mac 应用两种形态，支持 Anthropic/OpenAI 协议。⭐ 1 · MIT · 无 release

## 编辑器 · 笔记

原生代码编辑器、Markdown 笔记、文档与知识库工具：

- [sorrycc/Mayoi](https://github.com/sorrycc/Mayoi) — 迷い：Go 编写的小而快代码编辑器（GPU 原生 UI，无 webview/Electron，打包约 18MB）。⭐ 309 · MIT · Release v0.18.0（2026-11-04）
- [mu-zi-lee/Tangentry](https://github.com/mu-zi-lee/Tangentry) — 本地优先的内容聚合、阅读与笔记工具。⭐ 222 · MIT · Release v0.0.3.6（2026-10-31）
- [wibus-wee/see](https://github.com/wibus-wee/see) — 桌面源码阅读器：文件树、标签、搜索、符号、diff 与终端同窗。⭐ 18 · 未声明 · Release v0.1.17（2026-11-05）
- [echoVic/liubai](https://github.com/echoVic/liubai) — 留白：极简轻量 Markdown 写作桌（Go+MyGo 后端）。⭐ 13 · MIT · Release v0.6.7（2026-10-29）
- [fzn0x/Nether](https://github.com/fzn0x/Nether) — 自托管、本地优先的笔记应用，融合 Notion 与 Obsidian 特性。⭐ 5 · AGPL-3.0 · Release v0.0.1（2026-10-31）
- [oneo-me/locus](https://github.com/oneo-me/locus) — macOS 本地优先 Markdown 笔记本，笔记即普通文件，含 HTML 画布。⭐ 5 · MIT · Release v0.2026.1（2026-10-17）
- [sorrycc/Deckle](https://github.com/sorrycc/Deckle) — macOS 快速原生 Markdown 编辑器（GPU 自绘界面）。⭐ 5 · MIT · Release v0.2.0（2026-10-16）
- [tacshi/Leaflet](https://github.com/tacshi/Leaflet) — 人与 AI agent 共同写作的活文档，macOS/Windows 原生。⭐ 4 · MIT · Release v2026.11.8（2026-11-05）
- [gomeen/Zakki](https://github.com/gomeen/Zakki) — 多标签 Markdown 速记便签，Typora 式所见即所得。⭐ 3 · MIT · Release zakki-41-assets（2026-10-30）
- [kiwiflydream/yunji-uml](https://github.com/kiwiflydream/yunji-uml) — PlantUML / Mermaid / Flowchart.js 文本图表编辑器，MyGo 原生 UI。⭐ 3 · MIT · Release v0.2.0（2026-10-07）
- [Oranjekop/TextViewer](https://github.com/Oranjekop/TextViewer) — Go/MyGo 原生文本查看编辑器：大文件后台载入、多标签。⭐ 3 · MIT · Release v0.0.20（2026-11-05）
- [cliecy/Marginalia](https://github.com/cliecy/Marginalia) — 把 AI 对话沉淀为 Obsidian 兼容笔记的 macOS 知识库。⭐ 2 · MIT · Release v0.2.1（2026-10-28）
- [alvyn16/GOsidian](https://github.com/alvyn16/GOsidian) — Go + MyGo 写的 Obsidian 克隆，极早期双链笔记。⭐ 1 · MIT · Release v1.0.0（2026-10-24）
- [hunghg255/mycode](https://github.com/hunghg255/mycode) — 小而快的 Go 原生代码编辑器（GPU 自绘，约 18MB）。⭐ 1 · MIT · 无 release
- [LZD121/my-gotion](https://github.com/LZD121/my-gotion) — 本地优先 Notion 克隆：块级文档 + 多维表格，JSON 是唯一数据源。⭐ 1 · MIT · 无 release

## 终端 · 开发工具

终端、Git、API/数据库客户端、SSH 与研发工作台：

- [Licoy/sshyard](https://github.com/Licoy/sshyard) — 原生 SSH/SFTP 客户端：终端、文件管理与传输合一。⭐ 89 · AGPL-3.0 · Release v0.0.13（2026-11-05）
- [hyoban/peek](https://github.com/hyoban/peek) — macOS 原生 git diff 查看器，支持 Codex 写 commit 与评审。⭐ 73 · MIT · Release v0.7.0（2026-11-05）
- [Binaryify/MyGit](https://github.com/Binaryify/MyGit) — 面向 agent 改动的轻量原生 Git 客户端，三平台。⭐ 54 · MIT · Release v0.3.26（2026-11-03）
- [oneo-me/onegit](https://github.com/oneo-me/onegit) — 以 worktree 为中心、一窗浏览多个 Git 仓库的 macOS 应用。⭐ 10 · MIT · 无 release
- [jfut/ssh-keyselect](https://github.com/jfut/ssh-keyselect) — 交互式 SSH agent 代理：选择客户端可使用的密钥。⭐ 8 · Apache-2.0 · Release v0.2.0（2026-10-15）
- [nerv-base/mytoken](https://github.com/nerv-base/mytoken) — AI coding harness 的本地 token 与成本追踪器。⭐ 7 · MIT · Release v0.5.7（2026-10-29）
- [younland/apigo](https://github.com/younland/apigo) — MyGo 原生 UI 绘制的跨平台接口调试工具，形态对标 Hoppscotch。⭐ 7 · MIT · Release v0.1.3（2026-11-04）
- [saanuregh/dgopher](https://github.com/saanuregh/dgopher) — 快速原生数据库 GUI：PostgreSQL/MySQL/SQL Server/Oracle/ClickHouse/SQLite 等。⭐ 6 · Apache-2.0 · Release v0.7.0（2026-10-27）
- [welllog/otool](https://github.com/welllog/otool) — 纯 Go 原生桌面开发与日常运维工具箱（~15MB 常驻）。⭐ 6 · 未声明 · Release v0.1.4（2026-04-28）
- [ji233-Sun/easy-ssh-port](https://github.com/ji233-Sun/easy-ssh-port) — 一键开关 SSH 端口转发的 macOS 菜单栏应用（本地/远程/SOCKS5）。⭐ 5 · 未声明 · Release v1.0.0（2026-10-27）
- [fachrihawari/omaterm](https://github.com/fachrihawari/omaterm) — 并排跑 coding agent 的终端工作台，创建于框架同日。⭐ 4 · MIT · Release v0.13.2（2026-11-05）
- [tacshi/Yeek](https://github.com/tacshi/Yeek) — 纯 Go 原生跨平台 API 客户端（HTTP/GraphQL/gRPC/WebSocket）。⭐ 4 · MIT · Release v2026.10.7（2026-10-23）
- [CarlOpenLab/Gloss](https://github.com/CarlOpenLab/Gloss) — 为审阅 diff 而生的 Git 客户端：风险扫描、拓扑图、AI commit。⭐ 3 · MIT · Release v0.3.28（2026-11-03）
- [geeker-xiao/NanoAPI](https://github.com/geeker-xiao/NanoAPI) — 基于 MyGo 原生 UI 的轻量 API 桌面客户端，无 WebView 构建链。⭐ 3 · MIT · Release v1.0.2（2026-11-01）
- [javatoai/silverwing](https://github.com/javatoai/silverwing) — 小巧的多仓库研发工作台：任务、仓库、分支、资料与内置 Git 审阅。⭐ 3 · MIT · Release v0.0.12（2026-11-05）
- [jerryfane/herdrup-desktop](https://github.com/jerryfane/herdrup-desktop) — herdr 的桌面客户端，Go + 系统 WebView，三平台。⭐ 3 · Apache-2.0 · Release v0.1.0-preview.8（2026-11-04）
- [baka-world/dsh-gtk](https://github.com/baka-world/dsh-gtk) — 把 DeepSeek Harness 装进原生 GTK 窗口（Go + MyGo + WebKitGTK）。⭐ 2 · MIT · Release v0.1.3（2026-11-04）
- [contursofran/contr](https://github.com/contursofran/contr) — 极简原生 herdr 客户端，内置 herdr-agents 看板。⭐ 2 · Apache-2.0 · Release v0.1.3（2026-11-05）
- [iwangjie/Nemorous](https://github.com/iwangjie/Nemorous) — 多仓库 Git 协同与代码查阅的键盘优先桌面工具。⭐ 2 · MIT · Release v0.10.17（2026-11-05）
- [laojianzi/aster](https://github.com/laojianzi/aster) — Go + MyGo Native UI 写的 Kubernetes 工作台。⭐ 2 · Apache-2.0 · 无 release
- [Maidang1/hergo](https://github.com/Maidang1/hergo) — 原生 Herdr 桌面客户端：工作区、Git worktree、agent、分屏终端（原 herdr-ui）。⭐ 2 · MIT · Release v0.0.21（2026-11-05）
- [Maidang1/knack](https://github.com/Maidang1/knack) — 跨平台 AI Agent 技能管理器，统一浏览、共享、修复本地 skills。⭐ 2 · MIT · Release v0.1.0（2026-11-05）
- [oysterhyd/AgentMeter](https://github.com/oysterhyd/AgentMeter) — Windows 桌面端监控 Codex 配额、token 用量、成本与运行指标。⭐ 2 · 未声明 · Release v3.0.4（2026-10-22）
- [ychuo/tavu](https://github.com/ychuo/tavu) — 把终端、文件和改动放在手边的 macOS 原生工作区。⭐ 2 · 未声明 · Release v0.1.3（2026-10-19）
- [bencode/jun](https://github.com/bencode/jun) — 并排运行 Claude Code、Codex、Pi 等终端 agent 的 macOS 工作台。⭐ 1 · 未声明 · 无 release
- [cuikaipeng/kivrix](https://github.com/cuikaipeng/kivrix) — 跨平台原生 Redis 桌面客户端。⭐ 1 · MIT · Release v0.1.0（2026-11-02）
- [iwangjie/agentsmd](https://github.com/iwangjie/agentsmd) — 编辑 `~/.agents/AGENTS.md` 的 macOS 应用，发布 agent 读取的文档。⭐ 1 · MIT · 无 release
- [labstack/driga](https://github.com/labstack/driga) — 观察机器上所有 AI coding agent 会话：状态、项目、分支与收件箱。⭐ 1 · Apache-2.0 · Release v2026.10.29-alpha（2026-10-31）
- [legibet/myskills](https://github.com/legibet/myskills) — 跨 agent 管理 skills 的 CLI 与桌面应用。⭐ 1 · MIT · Release latest（2026-08-15）
- [preceeder/gui-redis](https://github.com/preceeder/gui-redis) — 单机 Redis 桌面客户端（SSH 隧道/SOCKS5）。⭐ 1 · 未声明 · Release v0.1.1（2026-10-25）
- [pteich/repo-hopper](https://github.com/pteich/repo-hopper) — 快速跳转到最近改动的本地 Git 仓库的原生启动器。⭐ 1 · MIT · Release v0.5.0（2026-11-02）
- [real-jacket/orbit](https://github.com/real-jacket/orbit) — tw93/mole CLI 的原生 macOS 客户端（Go + MyGo + WKWebView）。⭐ 1 · GPL-3.0 · 无 release
- [Riablo/skills-hub](https://github.com/Riablo/skills-hub) — 统一管理 agent skills 的桌面应用，可全局或按项目安装。⭐ 1 · 未声明 · Release v0.1.0（2026-10-08）
- [smallnest/hyla](https://github.com/smallnest/hyla) — smallnest 出品的跨平台原生终端（雨蛙）。⭐ 1 · MIT · Release v3.3.1（2026-11-05）
- [smallnest/nutty](https://github.com/smallnest/nutty) — smallnest 出品的 macOS 原生终端（otty.sh clone）。⭐ 1 · Apache-2.0 · Release v0.2.0（2026-10-13）
- [tiramission/oci-sync](https://github.com/tiramission/oci-sync) — 把本地文件或目录同步到 OCI 兼容镜像仓库。⭐ 1 · MIT · Release v0.8.0（2026-10-11）
- [version-fox/vfox-plus](https://github.com/version-fox/vfox-plus) — vfox 版本管理 CLI 的实验性 Web UI 与跨平台桌面应用。⭐ 1 · Apache-2.0 · 无 release
- [xinde/deepseek-harness-mygo](https://github.com/xinde/deepseek-harness-mygo) — 本地 DeepSeek Harness 的轻量 MyGo 桌面启动器。⭐ 1 · MIT · Release mygo-v0.1.1-798c33f126e9（2026-10-19）
- [xleotranx/wada-terminal](https://github.com/xleotranx/wada-terminal) — 面向 coding agent 的原生终端，基于 Go、MyGo 与 wada-kit。⭐ 1 · MIT · 无 release
- [echoVic/curlgo](https://github.com/echoVic/curlgo) — 轻量离线 API 客户端：原生 UI，支持 HTTP、SSE、WebSocket 与 curl 导入导出（维护者项目）。⭐ 0 · MIT · Release v0.1.1（2026-11-05）

## 网络 · 代理

代理客户端、流量分析、远程桌面与校园网工具：

- [AstraFoundry/KumoApp](https://github.com/AstraFoundry/KumoApp) — Mihomo 代理内核的 macOS 桌面客户端，Go + Web 前端。⭐ 297 · AGPL-3.0 · Release 0.0.15（2026-05-23）
- [lufficc/clash-traffic](https://github.com/lufficc/clash-traffic) — 看清 Clash Verge 流量去向：按应用、站点、节点、订阅与设备。⭐ 71 · 未声明 · Release v0.1.6（2026-11-03）
- [marukolibro/Hop](https://github.com/marukolibro/Hop) — macOS/Windows 的 mihomo（Clash.Meta）原生代理客户端。⭐ 18 · GPL-3.0 · Release v0.4.19（2026-11-03）
- [hygkui/v5vpn-rea-client](https://github.com/hygkui/v5vpn-rea-client) — 非官方 V5VPN/aTrust 客户端（协议逆向研究，自带免责声明）。⭐ 15 · Apache-2.0 · Release v0.6.0（2026-10-24）
- [xiaomai1011/GZIST-NetKeeper](https://github.com/xiaomai1011/GZIST-NetKeeper) — 广州理工学院校园网自动登录保活工具（Dr.COM/eportal）。⭐ 9 · 未声明 · Release v2.1.3（2026-10-10）
- [si-mods/MyVNC](https://github.com/si-mods/MyVNC) — 用 MyGo 写的纯 Go VNC 查看器（Windows），移植自 TigerVNC。⭐ 6 · GPL-2.0 · Release v0.1.0（2026-10-27）
- [margbug01/ShoesGUI](https://github.com/margbug01/ShoesGUI) — 给 shoes 内核做的 Windows/macOS 代理客户端 GUI。⭐ 5 · GPL-3.0 · Release v0.4.3（2026-10-29）
- [moxuun/sing-box-drover-go](https://github.com/moxuun/sing-box-drover-go) — sing-box 的托盘控制器，sing-box-dover 的 Go 重构版。⭐ 5 · MIT · Release v0.5.0（2026-10-26）
- [xiaomai1011/GZIST-Hotspot](https://github.com/xiaomai1011/GZIST-Hotspot) — 校园网有线转热点（广州理工学院），中文项目。⭐ 4 · MIT · Release v2.0.0（2026-10-09）
- [sakurasan/clashx-go](https://github.com/sakurasan/clashx-go) — macOS 菜单栏 ClashX 风格代理客户端，内置 mihomo core。⭐ 3 · AGPL-3.0 · Release v0.2.10（2026-11-03）
- [Souitou-iop/MyGO-Clash](https://github.com/Souitou-iop/MyGO-Clash) — 基于 mihomo 内核与 MyGo 的跨平台代理客户端。⭐ 3 · GPL-3.0 · Release v0.2.28-beta（2026-11-05）
- [zdyxry/TierGo](https://github.com/zdyxry/TierGo) — EasyTier 的非官方 MyGo 桌面客户端。⭐ 3 · MIT · 无 release
- [maximousblk/mochi](https://github.com/maximousblk/mochi) — Tailcat hosts 的原生桌面客户端。⭐ 2 · MIT · Release canary（2026-10-25）
- [Binaryify/proxy-bridge](https://github.com/Binaryify/proxy-bridge) — 用 TUN 把全部或选中应用流量送进 HTTP/HTTPS/SOCKS5 代理的 macOS 菜单栏工具。⭐ 1 · GPL-3.0 · Release v0.2.0（2026-10-16）
- [Jonkimi/mygo-naive-client](https://github.com/Jonkimi/mygo-naive-client) — 极轻量跨平台 NaiveProxy 客户端，纯 Go GPU 渲染原生 UI。⭐ 1 · AGPL-3.0 · Release v0.0.1（2026-11-04）
- [Kel077/pith](https://github.com/Kel077/pith) — 按应用、域名与 IP 选择 Mac 出口网卡的分流工具。⭐ 1 · MIT · 无 release
- [wyq09/kunpeng-clash](https://github.com/wyq09/kunpeng-clash) — 傻瓜化的 VPN 代理工具。⭐ 1 · 未声明 · Release v0.3.0（2026-10-28）

## 媒体 · 播放下载

音乐/视频播放器、下载器与音频处理工具：

- [bitxeno/atvloadly](https://github.com/bitxeno/atvloadly) — ATV 视频下载器 + mygo 桌面壳。⭐ 1640 · AGPL-3.0 · Release v0.8.2（2026-10-31）
- [elianiva/meiro](https://github.com/elianiva/meiro) — 轻量 YouTube Music 客户端。⭐ 296 · GPL-3.0 · Release desktop-v0.6.1（2026-11-05）
- [fzn0x/mixmusic](https://github.com/fzn0x/mixmusic) — 轻量 YouTube Music/Spotify 客户端，内存约 64MB。⭐ 259 · GPL-3.0 · Release v0.5.8（2026-11-02）
- [vst93/bili-fm](https://github.com/vst93/bili-fm) — 把 B 站节目当音频听的音乐/学习播放器，Go + mygo 原生。⭐ 78 · Apache-2.0 · Release mygo-v3.1.16（2026-11-02）
- [missuo/motrix-mygo](https://github.com/missuo/motrix-mygo) — Motrix 的 MyGo 原生 UI 版，驱动其 aria2 引擎，无 Electron/webview。⭐ 55 · 未声明 · Release v0.0.10（2026-10-15）
- [kamiertop/videodown](https://github.com/kamiertop/videodown) — 哔哩哔哩、抖音视频下载器。⭐ 52 · GPL-3.0 · Release v1.0.0-alpha.3（2026-11-03）
- [margbug01/MySpotify](https://github.com/margbug01/MySpotify) — Windows 上的非官方 Spotify 播放器，免费账号也能整首播放。⭐ 28 · AGPL-3.0 · Release v0.4.9（2026-11-03）
- [ca-x/lark](https://github.com/ca-x/lark) — 精致的 Web 音乐播放器，MyGo 原生桌面壳。⭐ 16 · AGPL-3.0 · Release v0.18.8（2026-11-05）
- [he-music/HE-Music](https://github.com/he-music/HE-Music) — 基于 SPlayer 的简约音乐播放器，MyGo 桌面形态。⭐ 14 · AGPL-3.0 · Release v2.0.0（2026-11-04）
- [yxxbc/haruhikage-app](https://github.com/yxxbc/haruhikage-app) — 春日影：Go 与 MyGo 写的跨平台音乐播放器，原生 UI 无 WebView。⭐ 9 · AGPL-3.0 · Release v0.1.23（2026-11-04）
- [Team-Quaver/quaver-astra](https://github.com/Team-Quaver/quaver-astra) — 轻量跨平台 Quaver 音乐客户端，由 MyGo 构建。⭐ 7 · AGPL-3.0 · Release snapshot-93cfb0d30f27（2026-11-05）
- [AMDL-Web/apple-music-downloader](https://github.com/AMDL-Web/apple-music-downloader) — Apple Music 下载后端：解析、下载、解密、重封装无损 ALAC。⭐ 6 · AGPL-3.0 · Release v2.0.0-rc.9（2026-11-03）
- [fazi-gondal/video-downloader-mygo](https://github.com/fazi-gondal/video-downloader-mygo) — yt-dlp/FFmpeg 桌面视频下载器。⭐ 4 · MIT · Release v3.2.0（2026-10-31）
- [FlashVCP/FlashMusic](https://github.com/FlashVCP/FlashMusic) — 原生跨平台多源音乐客户端：本地库 + 网易云。⭐ 3 · AGPL-3.0 · Release v0.1.4（2026-11-02）
- [j4ckxyz/Aurelia](https://github.com/j4ckxyz/Aurelia) — 为 Jellyfin 打造的快速原生音乐播放器。⭐ 3 · MIT · Release v0.3.0（2026-10-09）
- [yeshan333/tingsub](https://github.com/yeshan333/tingsub) — 本地双语直播字幕（英/日）工具，Apple Silicon + MLX。⭐ 2 · MIT · Release v0.3.0（2026-10-21）
- [yuxiaoLeeMarks/qqgo](https://github.com/yuxiaoLeeMarks/qqgo) — 第三方 QQ 音乐桌面客户端，三平台原生 UI。⭐ 2 · AGPL-3.0 · 无 release
- [ZypherChan/MusicComments](https://github.com/ZypherChan/MusicComments) — 网易云随机热评桌面应用，Go + MyGo 原生 UI。⭐ 2 · 未声明 · Release v1.0.1（2026-10-21）
- [biaobiaobiao108/fnmovie](https://github.com/biaobiaobiao108/fnmovie) — 把飞牛影视片库带到 Windows 桌面的原生客户端（libmpv 播放）。⭐ 1 · 未声明 · Release v1.3.2（2026-11-02）
- [freelxs/jstv-player](https://github.com/freelxs/jstv-player) — macOS 上的 JSTV/CatPawOpen 猫源协议播放器。⭐ 1 · MIT · Release v0.3.6（2026-10-24）
- [Itoktsnhc/WaveAlign](https://github.com/Itoktsnhc/WaveAlign) — 音视频波形自动对齐并导出新视频的桌面工具。⭐ 1 · MIT · Release v0.2.0（2026-11-03）
- [kindred-7/openDL](https://github.com/kindred-7/openDL) — 基于 MyGo 的开源下载器。⭐ 1 · MIT · Release 0.1.17（2026-11-04）
- [latiefahmad/ytbplus](https://github.com/latiefahmad/ytbplus) — 轻量 YouTube Music 客户端：无广告、Last.fm 记录、逐字歌词。⭐ 1 · GPL-3.0 · Release ytbplus-v1.0.2（2026-11-05）
- [rzh0504/Qmdr](https://github.com/rzh0504/Qmdr) — QQ 音乐与歌单下载器。⭐ 1 · GPL-3.0 · Release v0.3.3（2026-10-29）
- [ShellMonster/PudMusic](https://github.com/ShellMonster/PudMusic) — 跨平台桌面音乐播放器，播放 B 站音乐与本地音频。⭐ 1 · 未声明 · Release v0.2.2（2026-11-03）
- [tviber/voice-morph](https://github.com/tviber/voice-morph) — MorphVOX 风格实时变声器（Go DSP + MyGo 桌面壳）。⭐ 1 · 未声明 · 无 release
- [xptea/curb](https://github.com/xptea/curb) — 极简原生视频/音频下载器，粘贴链接选质量即可。⭐ 1 · MIT · Release v0.1.8（2026-10-17）
- [XueJie1/godrome](https://github.com/XueJie1/godrome) — Navidrome/Subsonic 原生桌面音乐播放器（进程内 libmpv）。⭐ 1 · MIT · 无 release

## 生产力 · 菜单栏

菜单栏小工具、剪贴板、启动器与日常效率应用：

- [Licoy/Quosparr](https://github.com/Licoy/Quosparr) — 菜单栏/托盘追踪 Codex、Claude Code、Grok 配额与重置时间。⭐ 318 · AGPL-3.0 · Release v1.11.2（2026-11-05）
- [henryyu333/rakko](https://github.com/henryyu333/rakko) — Mac 刘海工具：托盘、剪贴板历史、实时活动与快捷工具（由 shelf 改名）。⭐ 105 · Apache-2.0 · Release v1.13.3（2026-11-05）
- [Licoy/CPA-Bar](https://github.com/Licoy/CPA-Bar) — 菜单栏监控 CLIProxyAPI 服务。⭐ 15 · AGPL-3.0 · Release v1.0.38（2026-11-03）
- [oneo-me/neohm](https://github.com/oneo-me/neohm) — Home Assistant 菜单栏/托盘控制器（配套 onevra）。⭐ 9 · 未声明 · Release v0.2026.3（2026-10-20）
- [eziq1/golauncher](https://github.com/eziq1/golauncher) — Raycast 风格的 Windows/macOS 启动器，Go + MyGo 原生 UI。⭐ 6 · MIT · Release v0.13.1（2026-10-23）
- [iwangjie/xiangzhuan](https://github.com/iwangjie/xiangzhuan) — 菜单栏休息提醒：工作到点全屏燃香，一炷香尽回到案前。⭐ 4 · MIT · Release v0.9.0（2026-10-19）
- [echoVic/clipnest](https://github.com/echoVic/clipnest) — 现代轻量 Mac 剪贴板历史面板（快捷键+预览）。⭐ 2 · MIT · Release v0.1.9（2026-11-01）
- [mintonight/pomodoro](https://github.com/mintonight/pomodoro) — 极简桌面番茄钟：专注计时、统计热力图、托盘与 SQLite 本地存储。⭐ 2 · 未声明 · Release v0.3.1（2026-10-06）
- [qzz0518/Moniflip](https://github.com/qzz0518/Moniflip) — 一键把显示器切到另一台电脑（DDC/CI），菜单栏/托盘工具。⭐ 2 · MIT · Release v0.1.2（2026-10-13）
- [soidaken/ClipRecorder](https://github.com/soidaken/ClipRecorder) — Windows 原生截图/录屏/框选翻译工具。⭐ 2 · MIT · Release v1.4.4（2026-11-02）
- [0froq/snip](https://github.com/0froq/snip) — 基于 MyGo 原生 UI 的 macOS 剪贴板管理器原型。⭐ 1 · MIT · Release v0.1.0（2026-10-21）
- [FaintGhost/mac2mqtt](https://github.com/FaintGhost/mac2mqtt) — macOS 菜单栏 → Home Assistant over MQTT。⭐ 1 · MIT · Release v0.4.7（2026-11-04）
- [margbug01/mami](https://github.com/margbug01/mami) — 语音输入 + 划词翻译：右 Alt 说话，文字落到光标处。⭐ 1 · MIT · Release v2.10.6（2026-11-04）
- [michaelmjhhhh/Chaos](https://github.com/michaelmjhhhh/Chaos) — macOS 截图处理小工具。⭐ 1 · MIT · Release v1.1.0（2026-06-30）
- [mrzzmrzz/MySlack](https://github.com/mrzzmrzz/MySlack) — 轻量非官方 Slack 客户端，Go + MyGo 原生 UI、无 Electron。⭐ 1 · MIT · Release v0.1.5（2026-10-27）
- [qzz0518/moko](https://github.com/qzz0518/moko) — 在 Mac/Windows 上控制和查看夏普 KI-SX100 空气净化器。⭐ 1 · MIT · Release v0.1.1（2026-11-02）
- [sorrycc/Shun](https://github.com/sorrycc/Shun) — macOS 全局热键切换应用的菜单栏工具（Thor 风格）。⭐ 1 · 未声明 · Release v1.3.0（2026-10-30）
- [zyition/voke](https://github.com/zyition/voke) — Windows 启动器。⭐ 1 · MIT · Release v0.6.0（2026-11-04）

## 系统 · 监控

系统监控、清理、备份、存储与硬件管理工具：

- [Binaryify/MonitorBar](https://github.com/Binaryify/MonitorBar) — macOS 菜单栏 / Windows 托盘的显示器管理（输入源、音量）。⭐ 179 · MIT · Release v1.11.1（2026-10-22）
- [OUBIGFA/WinTab](https://github.com/OUBIGFA/WinTab) — Windows 11 资源管理器标签页工具（WinTab.Desktop 为 Go + MyGo 模块）。⭐ 113 · MIT · Release v2.4.7（2026-10-31）
- [OUBIGFA/WinTray](https://github.com/OUBIGFA/WinTray) — 把任意 Windows 程序自启动并最小化到托盘或后台。⭐ 93 · MIT · Release v3.5.0（2026-11-04）
- [DejavuMoe/Pail](https://github.com/DejavuMoe/Pail) — S3 兼容对象存储桌面管理器（S3/MinIO/R2/VersityGW 等）。⭐ 62 · MIT · Release v0.4.2（2026-11-05）
- [qzz0518/Charker](https://github.com/qzz0518/Charker) — Anker Prime 160W/250W 充电器的 macOS（SwiftUI）+ Windows（Go/MyGo）客户端。⭐ 62 · MIT · Release v0.5.7（2026-10-28）
- [pteich/us3ui](https://github.com/pteich/us3ui) — S3/对象存储/SFTP/FTP 的跨平台文件管理器。⭐ 38 · MIT · Release v0.13.0（2026-11-03）
- [voidksa/BootEase](https://github.com/voidksa/BootEase) — Windows BIOS/UEFI、恢复与系统工具（Loaderly.app）。⭐ 25 · GPL-3.0 · Release v3.0.0（2026-10-31）
- [Nigh/ReSoBackup](https://github.com/Nigh/ReSoBackup) — Reed-Solomon 纠删码 + AES-256 加密备份工具，GUI 与 CLI。⭐ 15 · LGPL-2.1 · Release v3.0.0（2026-10-10）
- [echoVic/cleanzo](https://github.com/echoVic/cleanzo) — macOS 深度清理工具（安全优先，Go+MyGo 原生）。⭐ 14 · MIT · Release v0.2.3（2026-10-21）
- [xbenduan/vitals](https://github.com/xbenduan/vitals) — macOS 菜单栏健康工具：CPU/内存/GPU/网速与应用内存档案。⭐ 12 · 未声明 · Release v0.3.2（2026-10-11）
- [e1roy/stage-manager-for-windows](https://github.com/e1roy/stage-manager-for-windows) — Windows 上的 macOS 风格 Stage Manager：当前应用留在台上，其余收进侧边栏分组（Go + MyGo）。⭐ 11 · MIT · Release 0.2.19（2026-11-04）
- [RedwindA/gotify-desktop](https://github.com/RedwindA/gotify-desktop) — Gotify 推送接收桌面客户端，三平台。⭐ 9 · GPL-3.0 · Release v0.3.10（2026-10-27）
- [younland/RcloneDrive](https://github.com/younland/RcloneDrive) — 基于 rclone 的跨平台云存储挂载工具，MyGo native 纯 Go 原生 UI。⭐ 9 · MIT · Release v0.2.4（2026-10-20）
- [Bush2021/pitstop](https://github.com/Bush2021/pitstop) — Windows 便携版 Chrome 的安装、更新与配置工具。⭐ 7 · GPL-3.0 · Release v1.1.0（2026-11-05）
- [RUBisco0211/unipac](https://github.com/RUBisco0211/unipac) — macOS 桌面包管理器：统一查看和操作多个包管理器安装的包。⭐ 7 · MIT · Release v0.2.0（2026-11-03）
- [LYJW131/anker-prime-desktop](https://github.com/LYJW131/anker-prime-desktop) — 通过蓝牙查看和控制 Anker Prime 充电器与移动电源。⭐ 3 · 未声明 · Release v1.0.2（2026-11-01）
- [DiiKhanh/burrow](https://github.com/DiiKhanh/burrow) — macOS 磁盘清理、空间可视化与系统健康监控。⭐ 2 · GPL-3.0 · Release v0.2.0（2026-11-04）
- [JohnsonRan/OpenSynapse](https://github.com/JohnsonRan/OpenSynapse) — 雷蛇鼠标与设备的开源设置应用。⭐ 1 · GPL-2.0 · Release v0.8.0（2026-10-30）
- [Magnetkopf/aim](https://github.com/Magnetkopf/aim) — Linux AppImage 安装器：双击即装、隔离路径。⭐ 1 · GPL-3.0 · Release nightly（2026-04-08）
- [meimingqi222/quick-cleaner](https://github.com/meimingqi222/quick-cleaner) — Windows 磁盘分析清理工具（已从 Rust/GPUI 重写为 Go + MyGo）。⭐ 1 · 未声明 · Release v0.0.24（2026-11-05）
- [yaffalhakim1/sweep](https://github.com/yaffalhakim1/sweep) — 找出吃掉磁盘的构建产物并一键清理，Go + MyGo 无 webview。⭐ 1 · MIT · Release v0.3.0（2026-10-14）

## 游戏 · 趣味

游戏辅助、模拟器与趣味项目：

- [Saramanda9988/LunaBox](https://github.com/Saramanda9988/LunaBox) — 轻量的视觉小说（Galgame）库管理与游戏统计工具。⭐ 387 · AGPL-3.0 · Release mygo-dev-latest（2026-10-28）
- [WonderLantern/z63-qemu](https://github.com/WonderLantern/z63-qemu) — 用 QEMU 跑尼康 Z6III 固件的实验，z63ui 桌面端把机器显示成一台相机。⭐ 18 · 未声明 · 无 release
- [zrcoder/ndor](https://github.com/zrcoder/ndor) — 用代码画画的小工具，给孩子和开发者。⭐ 11 · MIT · 无 release
- [echoVic/little-reef](https://github.com/echoVic/little-reef) — 小海底：用专注时间养出一片海的桌面挂件。⭐ 6 · MIT · Release v0.4.3（2026-11-01）
- [DanielZhangyc/Pinion](https://github.com/DanielZhangyc/Pinion) — 为 macOS 设计的鹰角游戏启动器，支持明日方舟与终末地。⭐ 1 · GPL-3.0 · Release v0.1.1（2026-11-02）
- [JayeGT002/rocom-egg-check](https://github.com/JayeGT002/rocom-egg-check) — 精灵蛋范围查询桌面应用（MyGo + Go + WebView）。⭐ 1 · 未声明 · Release v1.1.4（2026-10-13）
- [steampixel007/Dipper](https://github.com/steampixel007/Dipper) — 原生追番应用：Mikan 目录、RSS 与内置 BT 下载。⭐ 1 · 未声明 · Release v0.1.2（2026-11-01）
- [walm/agent-runner](https://github.com/walm/agent-runner) — 把 AI agent 放进霓虹雨夜城市里「开车」查看终端的小游戏。⭐ 1 · 未声明 · Release v1.0.0-run2（2026-11-02）
- [yaffalhakim1/nova](https://github.com/yaffalhakim1/nova) — 原生 Windows 游戏启动器，基于 MyGo，读取 Steam 美术素材。⭐ 1 · 未声明 · 无 release
- [zhengchalei/leagueakari-mygo](https://github.com/zhengchalei/leagueakari-mygo) — 国服 LOL 战绩/选人助手（源自 LeagueAkari，monorepo 内 mygo/go.mod 实证）。⭐ 1 · MIT · Release v0.5.6（2026-10-06）
- [zrcoder/ttoy](https://github.com/zrcoder/ttoy) — 开发者工具与小游戏合集，纯 Go + mygo 原生。⭐ 1 · MIT · 无 release

## UI 组件库

原生 UI 组件库、设计系统与配套工具链：

- [oneo-me/onevra](https://github.com/oneo-me/onevra) — 生态事实标准 Native UI 组件 + 打包器。⭐ 278 · MIT · Release source/v0.2026.17（2026-11-01）
- [caelyreth/untie](https://github.com/caelyreth/untie) — 纯 Go 的 TeX / Typst 数学排版渲染库，提供 MyGo 适配。⭐ 55 · Apache-2.0 · Release v0.5.0（2026-11-04）
- [ELY-Open-Source/CrychicUI](https://github.com/ELY-Open-Source/CrychicUI) — 1500 个 MyGo 原生 UI 组件，自带 MyGo 风格、动效与音效。⭐ 42 · MIT · 无 release
- [smallnest/uix](https://github.com/smallnest/uix) — smallnest 出品组件库（同时依赖 onevra）。⭐ 22 · MIT · 无 release
- [ELY-Open-Source/MujicaUI](https://github.com/ELY-Open-Source/MujicaUI) — 哥特风（Court-gothic）组件集。⭐ 17 · MIT · 无 release
- [ELY-Open-Source/8bitMyGoUI](https://github.com/ELY-Open-Source/8bitMyGoUI) — 16-bit 像素风组件集（含 wasm 浏览器演示）。⭐ 11 · MIT · 无 release
- [firede/mygo-platinum](https://github.com/firede/mygo-platinum) — 90 年代 Platinum 风格控件 + gallery。⭐ 3 · MIT · Release v0.2.2（2026-10-28）
- [josexy/nuxt-ui-go](https://github.com/josexy/nuxt-ui-go) — 受 Nuxt UI v4 启发的原生 Go 组件库（主题、表单、图表）。⭐ 2 · MIT · 无 release
- [yldm-tech/mygo-breeze-ui](https://github.com/yldm-tech/mygo-breeze-ui) — Tailwind 风格设计系统：原生组件 + CLI + MCP。⭐ 2 · MIT · 无 release
- [VaalaCat/mygo-kit](https://github.com/VaalaCat/mygo-kit) — Zed 风格原生组件库：连续面板、紧凑工具栏、One Light/Dark 主题。⭐ 1 · MIT · 无 release
- [xleotranx/wada-kit](https://github.com/xleotranx/wada-kit) — 可复用的 Go 插件内核 + 原生 MyGo 桌面工具包。⭐ 1 · MIT · Release v0.2.0（2026-11-04）

## 工具 · 其他

文件、图片、翻译、设备等实用工具：

- [LiorMoment/darkslide-gr](https://github.com/LiorMoment/darkslide-gr) — 给理光 GR III/IIIx 载入胶片外观与 LUT 的本地编辑器。⭐ 52 · GPL-2.0 · Release v1.6.1（2026-11-03）
- [zkeq/vibe-cook](https://github.com/zkeq/vibe-cook) — 烹饪教程 App（PWA + MyGo 桌面客户端）。⭐ 22 · 未声明 · Release v0.1.12（2026-10-27）
- [vfasky/mygo-vaultwarden](https://github.com/vfasky/mygo-vaultwarden) — Vaultwarden 的原生 macOS 客户端。⭐ 17 · 未声明 · Release v0.1.8（2026-10-13）
- [KirishimaRin/GDUT_Course_Helper](https://github.com/KirishimaRin/GDUT_Course_Helper) — 广东工业大学教务系统桌面抢课工具，支持课程浏览、收藏与并发抢课。⭐ 10 · 未声明 · Release v2.0.0（2026-10-25）
- [xiaomai1011/GZIST-DormSignin-Baiyun](https://github.com/xiaomai1011/GZIST-DormSignin-Baiyun) — 广州理工学院白云校区宿舍签到客户端（Go + MyGo）。⭐ 7 · 未声明 · Release v2.0.2（2026-10-16）
- [cainiao524/hd2-font-maker-go](https://github.com/cainiao524/hd2-font-maker-go) — 用自己的字体生成 Helldivers 2 字体替换 Mod 的 Windows 工具。⭐ 5 · MIT · Release v2.2.2（2026-11-05）
- [jhzhang09/gocompare](https://github.com/jhzhang09/gocompare) — 原生跨平台文件/文件夹对比：diff、三方合并、安全同步。⭐ 5 · MIT · Release v1.0.0（2026-11-04）
- [pplmx/aurora](https://github.com/pplmx/aurora) — 基于区块链的数字系统套件：VRF 抽奖、签名投票、预言机、NFT/FT，含桌面端。⭐ 5 · MIT · Release v1.1（2026-04-26）
- [hackerlengyue/binggan](https://github.com/hackerlengyue/binggan) — 基于 MyGo 和 Vue 的本地视频处理工具：密钥提取、课程播放编排、批量解密。⭐ 2 · GPL-3.0 · Release v2.0.0（2026-10-06）
- [ispacewang/quesora-native](https://github.com/ispacewang/quesora-native) — Quesora 刷题/考试的 Go + MyGo 原生 Windows 版。⭐ 2 · Apache-2.0 · Release v0.1.0-preview.4（2026-11-02）
- [LeuJasYoh/Type](https://github.com/LeuJasYoh/Type) — 绕过限制粘贴网站的输入工具。⭐ 2 · MIT · Release v2.0.0（2026-11-04）
- [margbug01/Candle](https://github.com/margbug01/Candle) — 照着 TradingView 做的 Binance K 线图桌面程序，原生 Win/macOS。⭐ 2 · MIT · Release v0.5.0（2026-10-29）
- [owocc/bowerbird](https://github.com/owocc/bowerbird) — 本地优先的素材与设计资源库管理器。⭐ 2 · 未声明 · Release v1.0.0-alpha-9（2026-11-03）
- [RSK21X/GoRss](https://github.com/RSK21X/GoRss) — Apple Silicon 原生 RSS/Atom 阅读器，内置可选 AI 摘要/翻译。⭐ 2 · 未声明 · Release v1.2.1（2026-10-15）
- [tacshi/Unscan](https://github.com/tacshi/Unscan) — 让扫描版 PDF 可搜索，或在 Mac 上重排为干净文本 PDF。⭐ 2 · MIT · Release v2026.10.6（2026-10-17）
- [0xletleon/ThunderstrikeControllerTool](https://github.com/0xletleon/ThunderstrikeControllerTool) — NVIDIA SHIELD TV 手柄固件刷写/降级/升级工具（Windows）。⭐ 1 · 未声明 · 无 release
- [aouyitanaka/Fsearch-Mygo-GUI](https://github.com/aouyitanaka/Fsearch-Mygo-GUI) — fsearch 全盘文件搜索的原生桌面 GUI（名称/内容检索）。⭐ 1 · 未声明 · 无 release
- [azusachino/felicia](https://github.com/azusachino/felicia) — 以地图为索引的旅行日记应用（实现阶段）。⭐ 1 · AGPL-3.0 · 无 release
- [CBR0/calc](https://github.com/CBR0/calc) — Windows 11 风格桌面计算器，纯 Go + MyGo 原生绘制。⭐ 1 · MIT · Release v0.1.1（2026-11-04）
- [Eurekaimer/TOUKO](https://github.com/Eurekaimer/TOUKO) — 把自己的图片存进自己的 Git 仓库，以树形仓库操作管理图库。⭐ 1 · MIT · Release v0.2.0（2026-10-22）
- [jiqing112/webdd-mygo-gui](https://github.com/jiqing112/webdd-mygo-gui) — 远程磁盘 dd 备份/恢复的 Windows GUI（MyGo + WebView2）。⭐ 1 · MIT · Release v1.0.0（2026-11-04）
- [lfcypo/pickphoto](https://github.com/lfcypo/pickphoto) — 快捷照片分类整理工具。⭐ 1 · MIT · Release v0.1.0（2026-10-07）
- [logdns/imyemail-cloud](https://github.com/logdns/imyemail-cloud) — 开源邮件客户端；其中 MyGo 原生版为预览形态。⭐ 1 · MIT · Release native-v0.2.4（2026-10-10）
- [msongd/kimquy](https://github.com/msongd/kimquy) — macOS 本地语义搜索：跨文本、文档、图片、PDF、音视频。⭐ 1 · MIT · 无 release
- [Nemuboshi/BadRename](https://github.com/Nemuboshi/BadRename) — 批量重命名工具，改名前可预览每个新名字。⭐ 1 · MIT · 无 release
- [oshell-desktop/oshell-desktop](https://github.com/oshell-desktop/oshell-desktop) — OShell 桌面端：共享 Go 核心与原生桌面 UI。⭐ 1 · GPL-3.0 · Release v0.3.2（2026-10-18）
- [rayorole/orole-os-desktop](https://github.com/rayorole/orole-os-desktop) — Orole OS：Windows 原生的个人操作环境（MyGo + Go daemon + React）。⭐ 1 · MIT · Release desktop-v0.4.4-dev（2026-10-21）
- [scialpicoody/linkdeck](https://github.com/scialpicoody/linkdeck) — 桌面串口/TCP 工作台：抓帧、发数据、自动化设备协议。⭐ 1 · 未声明 · 无 release
- [VeinsureLee/BYR-Client](https://github.com/VeinsureLee/BYR-Client) — 北邮人论坛本地桌面客户端。⭐ 1 · 未声明 · Release v0.1.1（2026-10-20）
- [wanan9999/android-tools](https://github.com/wanan9999/android-tools) — Windows 安卓设备工具箱：连接、投屏、文件管理与 Fastboot 刷机。⭐ 1 · 未声明 · Release v0.1.0（2026-10-28）
- [yangflow/oriel](https://github.com/yangflow/oriel) — RSS 与 RSSHub 的本地混合时间线阅读器，纯 Go + MyGo 原生 UI。⭐ 1 · MIT · Release v0.11.0（2026-10-25）

---

## 贡献指南

欢迎 PR 补充 mygo 生态项目！收录门槛与审核流程见 [收录标准草案.md](./收录标准草案.md)（两步核验：依赖与门槛 → 内容与格式）。要点：

1. **go.mod 证据**：根目录（或 monorepo 内实际模块路径）`go.mod` 含 `require github.com/egoist/mygo ...`，PR 中附 raw 链接。
2. **star ≥ 1**（维护者自有项目可例外，条目中会注明「维护者项目」）。
3. 非空壳、用途一句话、license、最新 Release 或可运行说明。

PR 条目格式：`- [owner/repo](url) — 一句话描述。⭐ N · License · Release/可运行说明`

> 数据约定：star / Release 为 2026-11-05 当日实测（当日晚间复核刷新过一次；前一轮为 2026-10-26），不引用第三方榜单数值。全量候选、依赖证据与排除项见 [候选项目盘点表.md](./候选项目盘点表.md)。

## 更新日志

- **2026-11-05**：全量复核并扩充至 223 条（新增收录 179 条，含维护者项目 curlgo；另有 11 个此前因 0★ 未收录的项目达星补入；2 个仓库改名已按新名收录：shelf→rakko、herdr-ui→hergo），star / Release 全部按当日实测刷新。
- **2026-10-26**：初版 33 条。
