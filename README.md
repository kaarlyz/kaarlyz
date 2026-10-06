<div align="center">

<img src="assets/banner.svg" width="100%" alt="Eka Restu Syahputra - Fullstack and Autonomous AI Systems" />

<a href="https://github.com/kaarlyz">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&pause=1200&color=38BDF8&center=true&vCenter=true&width=720&height=36&lines=Production-grade+software%2C+shipped+end+to+end;Autonomous+AI+pipelines+%26+fullstack+web;Local-first+architecture%2C+zero+fluff;Learn+%E2%86%92+Build+%E2%86%92+Ship+%E2%86%92+Own" alt="Typing animation" />
</a>

<p>
  <img src="https://img.shields.io/badge/STATUS-SHIPPING-38bdf8?style=for-the-badge&labelColor=0b1220" />
  <img src="https://img.shields.io/badge/FOCUS-AUTONOMOUS_AI-a78bfa?style=for-the-badge&labelColor=0b1220" />
  <img src="https://img.shields.io/badge/ARCH_LINUX-WAYLAND-1793d1?style=for-the-badge&logo=arch-linux&logoColor=white&labelColor=0b1220" />
  <img src="https://img.shields.io/badge/BASE-INDONESIA-10b981?style=for-the-badge&labelColor=0b1220" />
</p>

<table border="0" style="border: none; background: transparent; margin: 6px 0 12px 0;">
  <tr style="border: none; background: transparent;">
    <td align="center" width="125" valign="middle" style="border: none;">
      <img src="assets/avatar.jpg" width="110" height="110" style="border-radius: 50%; border: 2.5px solid #38bdf8; box-shadow: 0 0 20px rgba(56, 189, 248, 0.4), 0 0 40px rgba(56, 189, 248, 0.2); object-fit: cover;" alt="Avatar" />
    </td>
    <td valign="middle" align="left" style="border: none; padding-left: 16px;">
      <p style="margin: 0; color: #f8fafc; font-size: 15px; font-weight: 700; letter-spacing: -0.2px;">
        Eka Restu Syahputra 👋 <span style="color: #38bdf8; font-family: monospace; font-size: 13px; font-weight: 600;">@kaarlyz</span>
      </p>
      <p style="margin: 4px 0 0 0; color: #94a3b8; font-size: 13px; line-height: 1.5;">
        <i>"The cost of failing at 17 is Rp0. Eliminate speculative noise, master first principles, build proof of work, and let the code speak."</i>
      </p>
    </td>
  </tr>
</table>

<p>
  <a href="#work"><b>Work</b></a> &nbsp;/&nbsp;
  <a href="#tanka"><b>Tanka</b></a> &nbsp;/&nbsp;
  <a href="#stack"><b>Stack</b></a> &nbsp;/&nbsp;
  <a href="#principles"><b>Principles</b></a> &nbsp;/&nbsp;
  <a href="#telemetry"><b>Telemetry</b></a>
</p>

</div>

<br/>

<div align="center">
  <img src="assets/terminal.svg" width="90%" alt="Terminal: whoami, stack and current status" />
</div>

<br/>

> **I build systems that run in production, not demos.** Autonomous AI pipelines, local-first data layers, and fast interfaces. Every project below started as a real operational friction and ended as a working artifact.

<br/>

<a id="work"></a>
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
<summary><b>Interface previews</b></summary>
<br/>
<p align="center">
  <a href="https://github.com/kaarlyz/Tanka"><img src="assets/screenshot-tanka.png" width="32%" alt="Tanka UI" /></a>
  <a href="https://github.com/kaarlyz/myfxjournal"><img src="assets/screenshot-myfxjournal.png" width="32%" alt="KAFX Journal UI" /></a>
  <a href="https://github.com/kaarlyz/janka"><img src="assets/screenshot-janka.png" width="32%" alt="Janka UI" /></a>
</p>
</details>

**Experiments**

- **[MCP-TradingView](https://github.com/kaarlyz/MCP-TRADINGVIEW)**: Model Context Protocol server that lets AI coding agents inspect and control TradingView Desktop natively through Chrome DevTools Protocol. `TypeScript` `Node.js` `MCP` `CDP`
- **[RemiBot](https://github.com/kaarlyz/remibot)**: modular WhatsApp automation on the Baileys WebSocket library, built around structured workflows and broadcast queues. `JavaScript` `Baileys`
- **[MyCoffee](https://github.com/kaarlyz/mycoffee)**: coffee ordering storefront experiment. `Next.js` `TypeScript`

<br/>

<a id="tanka"></a>
<img src="assets/hdr-tanka.svg" width="100%" alt="Flagship: Tanka" />

**Tanka (短歌)** is an adaptive study platform that turns textbooks, handwritten notes, PDFs, and YouTube videos into a structured mastery system for Indonesian SMA/UTBK students. The core design rule: **generation must be grounded.** Facts are extracted and verified first, and only then synthesized into teaching material.

<p align="center">
  <img src="assets/tanka-pipeline.svg" width="100%" alt="Tanka pipeline: ingest, segment, ground, generate, retain" />
</p>

**Engineering problems solved**

| Problem | Approach |
|:--|:--|
| Model hallucination in study material | Two-Pass V3 pipeline: Pass 1 extracts canonical facts, Pass 2 does adaptive pedagogical synthesis. Concepts carry an origin tag (`source` or `ai_enrichment`) and are checked against the national curriculum (Ruangguru / Wikipedia) |
| OCR timeouts on large handwritten scans | Client-side HTML5 canvas compression with dynamic sizing, plus parallel multi-worker AI OCR to stay under HTTP / Cloudflare timeout limits |
| Complex math rendering | KaTeX typesetting with HTML tag isolation so expressions survive generation and sanitizing |
| Source diversity | Unified ingestion: `pdftotext`, Tesseract, PPTX/DOCX XML parsing, vision API for images, multilingual YouTube transcript extractor |
| Tutor context bleeding between documents | "Tanya Nara" with per-document session isolation and two-layer persistence (localStorage + SQLite) |
| Retention, not just reading | HOTS quizzes micro-batched up to 20 questions, hidden formula cards, Leitner spaced-repetition flashcards, mistakes bank, Feynman voice test (`MediaRecorder` to `faster-whisper`) |
| Token cost and rate limits | 9Router gateway with custom-header token-saver bypass, model cooldown handling, and per-domain adaptive temperature |
| Speed and offline resilience | PWA with service-worker caching, native Node.js HTTP server (no Express), in-process SQLite in WAL mode with cascading deletes |

**Adaptive domains.** Exact sciences get KaTeX equations and UTBK-style worked examples; practical topics get playbook-style output.

**Continuously audited.** Prompts, context truncation, tone consistency, mobile table/diagram rendering, and OCR typo correction are stress-tested on real study material rather than assumed to work.

<br/>

<a id="stack"></a>
<img src="assets/hdr-stack.svg" width="100%" alt="Tech Arsenal" />

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=ts,js,react,vite,tailwind,nodejs,express,python,sqlite,linux,arch,bash,neovim,git,github,figma&theme=dark&perline=8" alt="Tech icons" />
  </a>
</p>

**Frontend and UX systems** <br/>
![TypeScript](https://img.shields.io/badge/TypeScript-0f172a?style=flat-square&logo=typescript&logoColor=38bdf8)
![React](https://img.shields.io/badge/React_18/19-0f172a?style=flat-square&logo=react&logoColor=38bdf8)
![Vite](https://img.shields.io/badge/Vite-0f172a?style=flat-square&logo=vite&logoColor=a78bfa)
![Tailwind](https://img.shields.io/badge/Tailwind-0f172a?style=flat-square&logo=tailwindcss&logoColor=38bdf8)
![KaTeX](https://img.shields.io/badge/KaTeX-0f172a?style=flat-square)
![PWA](https://img.shields.io/badge/PWA_+_Service_Workers-0f172a?style=flat-square)
![Design](https://img.shields.io/badge/Editorial_anti--slop_UI-0f172a?style=flat-square)

**Backend and data layer** <br/>
![Node.js](https://img.shields.io/badge/Node.js_native_HTTP-0f172a?style=flat-square&logo=nodedotjs&logoColor=34d399)
![Express](https://img.shields.io/badge/Express-0f172a?style=flat-square&logo=express&logoColor=white)
![Python](https://img.shields.io/badge/Python_3.14_+_uv-0f172a?style=flat-square&logo=python&logoColor=fbbf24)
![SQLite](https://img.shields.io/badge/SQLite_WAL-0f172a?style=flat-square&logo=sqlite&logoColor=38bdf8)
![WebSockets](https://img.shields.io/badge/WebSockets-0f172a?style=flat-square)
![Protobuf](https://img.shields.io/badge/Protocol_Buffers-0f172a?style=flat-square)
![ExcelJS](https://img.shields.io/badge/ExcelJS-0f172a?style=flat-square)

**AI engineering** <br/>
![Pipelines](https://img.shields.io/badge/Multi--stage_grounded_pipelines-0f172a?style=flat-square)
![Vision](https://img.shields.io/badge/Vision_OCR_+_parallel_workers-0f172a?style=flat-square)
![MCP](https://img.shields.io/badge/MCP_+_CDP-0f172a?style=flat-square)
![9Router](https://img.shields.io/badge/9Router_gateway-0f172a?style=flat-square)
![Whisper](https://img.shields.io/badge/faster--whisper-0f172a?style=flat-square)
![MediaPipe](https://img.shields.io/badge/MediaPipe_Tasks-0f172a?style=flat-square)

**Quant, vision and systems** <br/>
![Quant](https://img.shields.io/badge/R:R,_drawdown,_Sharpe-0f172a?style=flat-square)
![MQL5](https://img.shields.io/badge/MQL5_Expert_Advisors-0f172a?style=flat-square)
![NumPy](https://img.shields.io/badge/NumPy_vectorized_physics-0f172a?style=flat-square)
![Arch](https://img.shields.io/badge/Arch_Linux-0f172a?style=flat-square&logo=archlinux&logoColor=1793d1)
![Bash](https://img.shields.io/badge/Bash_/_Zsh_/_D--Bus-0f172a?style=flat-square&logo=gnubash&logoColor=34d399)
![Git](https://img.shields.io/badge/Git-0f172a?style=flat-square&logo=git&logoColor=fb923c)
![Rclone](https://img.shields.io/badge/Rclone-0f172a?style=flat-square)

<br/>

<a id="principles"></a>
<img src="assets/hdr-principles.svg" width="100%" alt="How I Engineer" />

- **Proof of work over claims.** A working artifact beats a certificate or a slide.
- **Grounded over fluent.** AI output must trace back to a source or be labeled as enrichment.
- **Local-first, low-dependency.** Native HTTP and in-process SQLite: fewer moving parts, zero network latency to the data layer, easier to debug and ship.
- **Plan, then execute fast.** Define the concrete steps first, then move without ceremony.
- **Audit your own pipeline.** Prompts, context limits, tone drift, and OCR noise get tested, not assumed.
- **Design is engineering.** Clean editorial interfaces, no template slop, no visual clutter, instant interactions.

<br/>

<a id="telemetry"></a>
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

<a id="contact"></a>
<img src="assets/hdr-contact.svg" width="100%" alt="Let's Build" />

<div align="center">

Open to talking architecture, AI pipelines, or building something together. Reach out through GitHub.

<!-- Add other contact links here: email / LinkedIn / Telegram -->
<a href="https://github.com/kaarlyz"><img src="https://img.shields.io/badge/GitHub-@kaarlyz-0b1220?style=for-the-badge&logo=github&logoColor=38bdf8" alt="GitHub" /></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:090d16,50:0369a1,100:38bdf8&height=110&section=footer" width="100%" alt="" />

</div>