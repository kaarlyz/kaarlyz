<div align="center">

<img src="assets/banner.svg" width="100%" alt="Eka Restu Syahputra - Fullstack and Autonomous AI Systems" />

<a href="https://github.com/kaarlyz">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&pause=1200&color=38BDF8&center=true&vCenter=true&width=720&height=36&lines=Turning+ideas+into+production-grade+software;Autonomous+AI+pipelines+%26+fullstack+web;Building+Tanka%3A+a+grounded+AI+study+engine;Learn+%E2%86%92+Build+%E2%86%92+Ship+%E2%86%92+Own" alt="Typing animation" />
</a>

<p>
  <img src="https://img.shields.io/badge/STATUS-SHIPPING-38bdf8?style=for-the-badge&labelColor=0b1220" />
  <img src="https://img.shields.io/badge/FOCUS-AUTONOMOUS_AI-a78bfa?style=for-the-badge&labelColor=0b1220" />
  <img src="https://img.shields.io/badge/ARCH_LINUX-WAYLAND-1793d1?style=for-the-badge&logo=arch-linux&logoColor=white&labelColor=0b1220" />
  <img src="https://img.shields.io/badge/BASE-INDONESIA-10b981?style=for-the-badge&labelColor=0b1220" />
</p>

<p>
  <a href="#-01--selected-work"><b>Work</b></a> &nbsp;·&nbsp;
  <a href="#-02--flagship-tanka"><b>Tanka</b></a> &nbsp;·&nbsp;
  <a href="#-03--tech-arsenal"><b>Stack</b></a> &nbsp;·&nbsp;
  <a href="#-04--how-i-engineer"><b>Principles</b></a> &nbsp;·&nbsp;
  <a href="#-05--telemetry"><b>Telemetry</b></a>
</p>

</div>

<br/>

<div align="center">
  <img src="assets/terminal.svg" width="90%" alt="Terminal: whoami, stack and current status" />
</div>

<br/>

> **I build things that run.** Autonomous AI pipelines, local-first data layers, and interfaces that stay out of your way. Every repo below started as a real friction and ended as a shipped artifact.

<br/>

## 🛰️ 01 · Selected Work

<img src="assets/hdr-work.svg" width="100%" alt="Selected Work" />

<p align="center">
  <a href="https://github.com/kaarlyz/Tanka"><img src="assets/card-tanka.svg" width="49%" alt="Tanka" /></a>
  <a href="https://github.com/kaarlyz/myfxjournal"><img src="assets/card-kafx.svg" width="49%" alt="KAFX Journal" /></a>
  <a href="https://github.com/kaarlyz/janka"><img src="assets/card-janka.svg" width="49%" alt="Janka" /></a>
  <a href="https://github.com/kaarlyz/Particle-shape-gesture"><img src="assets/card-aether.svg" width="49%" alt="AetherParticles 3D" /></a>
  <a href="https://github.com/kaarlyz/nanonanabot"><img src="assets/card-router.svg" width="49%" alt="9Router Command Hub" /></a>
  <a href="https://github.com/kaarlyz/HOPDIS"><img src="assets/card-hopdis.svg" width="49%" alt="HOPDIS" /></a>
</p>

<details open>
<summary><b>🖼️ Interface previews</b></summary>
<br/>
<p align="center">
  <a href="https://github.com/kaarlyz/Tanka"><img src="assets/screenshot-tanka.png" width="32%" alt="Tanka UI" /></a>
  <a href="https://github.com/kaarlyz/myfxjournal"><img src="assets/screenshot-myfxjournal.png" width="32%" alt="KAFX Journal UI" /></a>
  <a href="https://github.com/kaarlyz/janka"><img src="assets/screenshot-janka.png" width="32%" alt="Janka UI" /></a>
</p>
</details>

**🔬 Experiments & side quests**

- 📈 **[MCP-TradingView](https://github.com/kaarlyz/MCP-TRADINGVIEW)**: Model Context Protocol server that lets AI agents drive TradingView Desktop charts over Chrome DevTools Protocol. `Node.js` `MCP` `CDP`
- 🤖 **[RemiBot](https://github.com/kaarlyz/remibot)**: modular WhatsApp automation on the Baileys socket library: structured workflows and broadcast queues. `JavaScript` `Baileys`
- ☕ **[MyCoffee](https://github.com/kaarlyz/mycoffee)**: coffee ordering storefront experiment. `Next.js` `TypeScript`

<br/>

## 🧠 02 · Flagship: Tanka

<img src="assets/hdr-tanka.svg" width="100%" alt="Flagship: Tanka" />

**Tanka (短歌)** turns textbooks, handwritten notes, PDFs, and YouTube videos into a structured mastery system for Indonesian SMA/UTBK students. The core idea: **generation must be grounded.** Content is built from verified concepts extracted from the source, not from the model's imagination.

<p align="center">
  <img src="assets/tanka-pipeline.svg" width="100%" alt="Tanka pipeline: ingest, segment, ground, generate, retain" />
</p>

| Layer | Implementation |
|:--|:--|
| **Server** | Native Node.js HTTP server, no Express |
| **Storage** | SQLite in WAL mode via `better-sqlite3`, local-first |
| **Ingestion** | `extract_text.py`: `pdftotext`, Tesseract OCR, PPTX/DOCX XML parsing, vision API for images |
| **Grounding** | Two-pass pipeline: `document_segments` → `document_concepts` (tagged `source` or `ai_enrichment`) → generated content |
| **AI gateway** | 9Router: model routing, cooldowns, token-saver bypass |
| **Tutor** | "Tanya Nara": session-isolated chat with two-layer persistence (localStorage + SQLite) |
| **Active recall** | HOTS quizzes, hidden formula cards, Leitner flashcards, mistakes bank, Feynman test with `MediaRecorder` → `faster-whisper` |
| **Frontend** | Vite + React + TypeScript, KaTeX for exact-science typesetting, installable PWA |

**What makes it different**

- 🎯 **Provenance by design:** concepts carry an origin tag, so source-backed facts and AI enrichment never get mixed up.
- 📐 **Adaptive domains:** exact sciences get KaTeX equations and UTBK-style worked examples; practical topics get playbook-style output.
- 🔍 **Self-audited:** I regularly stress-test my own prompts and pipeline: context truncation, tone consistency, mobile table/diagram rendering, OCR typo correction.

<br/>

## ⚙️ 03 · Tech Arsenal

<img src="assets/hdr-stack.svg" width="100%" alt="Tech Arsenal" />

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=ts,js,react,vite,tailwind,nodejs,express,python,sqlite,linux,arch,bash,neovim,git,github,figma&theme=dark&perline=8" alt="Tech icons" />
  </a>
</p>

**Frontend & experience** <br/>
![TypeScript](https://img.shields.io/badge/TypeScript-0f172a?style=flat-square&logo=typescript&logoColor=38bdf8)
![React](https://img.shields.io/badge/React_18/19-0f172a?style=flat-square&logo=react&logoColor=38bdf8)
![Vite](https://img.shields.io/badge/Vite-0f172a?style=flat-square&logo=vite&logoColor=a78bfa)
![Tailwind](https://img.shields.io/badge/Tailwind-0f172a?style=flat-square&logo=tailwindcss&logoColor=38bdf8)
![KaTeX](https://img.shields.io/badge/KaTeX-0f172a?style=flat-square)
![PWA](https://img.shields.io/badge/PWA-0f172a?style=flat-square)
![Design](https://img.shields.io/badge/Editorial_UI_systems-0f172a?style=flat-square)

**Backend & core systems** <br/>
![Node.js](https://img.shields.io/badge/Node.js_raw_HTTP-0f172a?style=flat-square&logo=nodedotjs&logoColor=34d399)
![Express](https://img.shields.io/badge/Express-0f172a?style=flat-square&logo=express&logoColor=white)
![Python](https://img.shields.io/badge/Python-0f172a?style=flat-square&logo=python&logoColor=fbbf24)
![SQLite](https://img.shields.io/badge/SQLite_WAL-0f172a?style=flat-square&logo=sqlite&logoColor=38bdf8)
![WebSockets](https://img.shields.io/badge/WebSockets-0f172a?style=flat-square)
![Protobuf](https://img.shields.io/badge/Protocol_Buffers-0f172a?style=flat-square)

**AI & automation** <br/>
![Pipelines](https://img.shields.io/badge/Multi--stage_AI_pipelines-0f172a?style=flat-square)
![Grounding](https://img.shields.io/badge/Grounded_generation-0f172a?style=flat-square)
![MCP](https://img.shields.io/badge/MCP_+_CDP-0f172a?style=flat-square)
![9Router](https://img.shields.io/badge/9Router_gateway-0f172a?style=flat-square)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0f172a?style=flat-square)
![Whisper](https://img.shields.io/badge/faster--whisper-0f172a?style=flat-square)
![OCR](https://img.shields.io/badge/Tesseract_OCR-0f172a?style=flat-square)

**Environment & ops** <br/>
![Arch](https://img.shields.io/badge/Arch_Linux-0f172a?style=flat-square&logo=archlinux&logoColor=1793d1)
![Bash](https://img.shields.io/badge/Bash_/_Zsh-0f172a?style=flat-square&logo=gnubash&logoColor=34d399)
![systemd](https://img.shields.io/badge/systemd-0f172a?style=flat-square)
![Git](https://img.shields.io/badge/Git-0f172a?style=flat-square&logo=git&logoColor=fb923c)
![Neovim](https://img.shields.io/badge/Neovim-0f172a?style=flat-square&logo=neovim&logoColor=34d399)
![Rclone](https://img.shields.io/badge/Rclone-0f172a?style=flat-square)

<br/>

## 🧭 04 · How I Engineer

<img src="assets/hdr-principles.svg" width="100%" alt="How I Engineer" />

- 🧱 **Grounded > fluent.** AI output should trace back to a source, or be labeled as enrichment.
- 🏠 **Local-first, low-dependency.** Raw Node HTTP and SQLite WAL: fewer moving parts, easier to debug and ship on a single box.
- 🔬 **Audit your own pipeline.** Prompts, context limits, tone drift, and OCR noise all get tested, not assumed.
- 📦 **Ship artifacts, not tutorials.** Study retention, trade discipline, warehouse paperwork, OS migration: each project solves a friction I actually had or saw.
- 🎨 **Design is engineering.** Dark, editorial, no template slop, with real typesetting (KaTeX) and mobile-first PWAs.

<br/>

## 📡 05 · Telemetry

<img src="assets/hdr-telemetry.svg" width="100%" alt="Telemetry" />

<p align="center">
  <img src="https://github-readme-stats-fast.vercel.app/api?username=kaarlyz&show_icons=true&theme=tokyonight&title_color=38bdf8&text_color=94a3b8&icon_color=a78bfa&hide_border=true&bg_color=0d1117" height="165" alt="GitHub stats" />
  <img src="https://github-readme-stats-fast.vercel.app/api/top-langs/?username=kaarlyz&layout=compact&theme=tokyonight&title_color=38bdf8&text_color=94a3b8&hide_border=true&bg_color=0d1117" height="165" alt="Top languages" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=kaarlyz&bg_color=0d1117&color=38bdf8&line=38bdf8&point=f8fafc&area=true&area_color=38bdf8&hide_border=true&custom_title=Contribution%20Graph" width="100%" alt="Contribution graph" />
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/kaarlyz/kaarlyz/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/kaarlyz/kaarlyz/output/github-contribution-grid-snake.svg" />
    <img alt="Contribution snake" src="https://raw.githubusercontent.com/kaarlyz/kaarlyz/output/github-contribution-grid-snake.svg" width="800" />
  </picture>
</p>

<br/>

## 🤝 06 · Let's Build

<img src="assets/hdr-contact.svg" width="100%" alt="Let's Build" />

<div align="center">

Open to talking architecture, AI pipelines, or building something together. Drop an issue or reach out through GitHub.

<!-- Tambahin kontak lain di sini kalau mau: email / LinkedIn / Telegram -->
<a href="https://github.com/kaarlyz"><img src="https://img.shields.io/badge/GitHub-@kaarlyz-0b1220?style=for-the-badge&logo=github&logoColor=38bdf8" alt="GitHub" /></a>

<sub><i>"Tatakae. Keep moving forward until the artifact is built."</i></sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:090d16,50:0369a1,100:38bdf8&height=110&section=footer" width="100%" alt="" />

</div>
