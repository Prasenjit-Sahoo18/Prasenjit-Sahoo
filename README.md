<div align="center">

<a href="https://vybeon.onrender.com/" title="Open Vybeon live">
  <img src="./dev-desk.svg" alt="Prasenjit coding Vybeon and VibeChat at his desk" width="100%"/>
</a>

<br/>

<img src="./images.dev.jpg" alt="Neon-lit illustration of Prasenjit at his developer desk" width="220"/>

<br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=19&duration=2600&pause=800&color=B8FF00&center=true&vCenter=true&width=820&lines=Hi%2C+I'm+Prasenjit+Sahoo+%E2%80%94+full-stack+developer;I+build+real-time+apps%2C+streaming+platforms+%26+AI+products;Next.js+%C2%B7+TypeScript+%C2%B7+Node+%C2%B7+Socket.IO+%C2%B7+Prisma+%C2%B7+PostgreSQL;B.Tech+CSE+%40+ITER%2C+SOA+University+%E2%80%94+always+shipping"/>

<br/>

<a href="https://vybeon.onrender.com/"><img src="https://img.shields.io/badge/LIVE-VYBEON-050505?style=for-the-badge&logo=spotify&logoColor=B8FF00"/></a>
<a href="https://www.linkedin.com/in/prasenjit-sahoo18/"><img src="https://img.shields.io/badge/LINKEDIN-050505?style=for-the-badge&logo=linkedin&logoColor=00F5FF"/></a>
<a href="mailto:mukeshsahoo902@gmail.com"><img src="https://img.shields.io/badge/EMAIL-050505?style=for-the-badge&logo=gmail&logoColor=7C3AED"/></a>
<img src="https://komarev.com/ghpvc/?username=Prasenjit-Sahoo18&style=for-the-badge&color=050505&label=VISITORS&labelColor=050505&abbreviated=true"/>

</div>

<br/>

```text
┌─────────────────────────── DEV.PROFILE ───────────────────────────┐
│  NAME       Prasenjit Sahoo                                        │
│  STUDYING   B.Tech CSE — ITER, SOA University, Bhubaneswar         │
│  LANGUAGES  Python · Java · C++ · TypeScript · JavaScript          │
│  SHIPPED    Vybeon · VibeChat · ShowPulse · CodeBuzz49 · foodiez   │
│  PRACTISING LeetCode · Competitive Programming · System Design     │
│  PRINCIPLE  A deployed product beats a perfect localhost.          │
└────────────────────────────────────────────────────────────────────┘
```

<br/>

<div align="center">

# ⚡ FLAGSHIP BUILDS

</div>

## 🎧 VYBEON &nbsp;·&nbsp; *Where every vibe comes alive*

> A futuristic music-streaming platform with a mood-driven **Vibe Engine**, an in-house **NeonMix AI** assistant, **Music DNA** analytics and a real-time **Web Audio visualizer** — wrapped in a Radium Neon design system.

<table>
<tr>
<td width="62%" valign="top">

```ts
stack: {
  app:      "Next.js 14 (App Router) · React 18 · TypeScript",
  ui:       "Tailwind CSS · Zustand · Recharts",
  auth:     "Auth.js v5 (JWT) · Zod validation",
  data:     "Prisma 5 · PostgreSQL 16",
  audio:    "HTML5 Audio + Web Audio Analyser",
  deploy:   "Render Blueprint (render.yaml)",
  quality:  "Vitest · strict TypeScript · /api/health",
}
```

</td>
<td width="38%" valign="top">

**What's inside**

🔮 Vibe Engine mood → playlist
🤖 NeonMix AI music assistant
📊 Music DNA listening analytics
📡 Neon Radio endless stations
🔊 Live spectrum visualizer
🏆 Achievement unlocks
⌨️ Full keyboard shortcuts

</td>
</tr>
</table>

[![Live](https://img.shields.io/badge/▶_Live_Demo-B8FF00?style=for-the-badge&logoColor=black)](https://vybeon.onrender.com/) [![Source](https://img.shields.io/badge/⌥_Source_Code-7C3AED?style=for-the-badge)](https://github.com/Prasenjit-Sahoo18/Vybeon)

<details>
<summary><b>🗺️ Vybeon architecture (click to expand)</b></summary>

```mermaid
graph TB
    subgraph Client
        UI[Next.js App Router] --> Store[Zustand Store]
        UI --> Audio[HTML5 Audio + Web Audio]
        Audio --> Viz[Canvas Visualizer]
    end
    subgraph Server
        API[REST API /api/*] --> Auth[Auth.js JWT]
        API --> Vibe[Vibe Engine]
        API --> Neon[NeonMix AI]
        API --> Prov[MusicProvider]
    end
    subgraph Data
        Prisma[Prisma ORM] --> PG[(PostgreSQL 16)]
    end
    UI --> API
    Prov --> Prisma
```

</details>

<br/>

## 💬 VIBECHAT &nbsp;·&nbsp; *Real-time social communication platform*

> Instant messaging with **voice & video calls (WebRTC)**, 24-hour **music status stories**, **in-chat payments** and an **AI copilot** — all running on a unified single-port Next.js + Socket.IO server.

<table>
<tr>
<td width="62%" valign="top">

```ts
stack: {
  app:       "Next.js 14 · React 18 · TypeScript · Tailwind",
  realtime:  "Node HTTP server + Socket.IO (single port)",
  calling:   "WebRTC MediaStream — voice & video",
  data:      "Prisma · PostgreSQL (SQLite locally, auto-switch)",
  auth:      "JWT in HTTP-only cookies · bcryptjs · Zod",
  payments:  "Razorpay / Stripe / sandbox abstraction",
  media:     "File API · Cloudinary adapter",
  deploy:    "Docker · Render blueprint · Fly.io config",
}
```

</td>
<td width="38%" valign="top">

**What's inside**

⚡ Typing, read receipts, reactions
📞 Voice & video calling
💸 Peer-to-peer wallet payments
🎵 Stories with music
🤖 AI copilot
📥 One-click media downloads
📷 Avatar upload from device

</td>
</tr>
</table>

[![Source](https://img.shields.io/badge/⌥_Source_Code-00F5FF?style=for-the-badge&logoColor=black)](https://github.com/Prasenjit-Sahoo18/Vibe_Chat)

<details>
<summary><b>🗺️ VibeChat request flow (click to expand)</b></summary>

```mermaid
flowchart LR
    A([Browser<br/>Next.js UI]) -->|HTTP| S[Custom Node Server]
    A <-->|Socket.IO events| S
    A <-.->|WebRTC peer media| B([Other client])
    S -->|signalling| A
    S --> R[Route Handlers<br/>JWT cookie auth]
    R --> P[(Prisma → PostgreSQL)]
    R --> Pay[Payment Service<br/>Razorpay / Stripe / Sandbox]
    R --> M[Media: Cloudinary / Data-URI]
```

</details>

<br/>

<div align="center">

# 🧩 MORE SHIPPED PROJECTS

</div>

<table>
<tr>
<td width="50%" valign="top">

### 🎬 ShowPulse
`Discover → Showtimes → Seat Lock → Checkout → QR Ticket`

10-minute temporary seat holds, coupon engine, JWT auth, QR tickets, admin analytics.

`React` `TypeScript` `Node` `Express` `Prisma` `PostgreSQL`

[▶ Live](https://cinepulse-7ajb.onrender.com) · [⌥ Code](https://github.com/Prasenjit-Sahoo18/ShowPulse)

</td>
<td width="50%" valign="top">

### 🧠 CodeBuzz49
`Practice → AI Hints → Execute → Proctor → Assess`

Gemini-powered hints, remote code execution, OpenCV + MediaPipe camera proctoring, premium plans.

`Django` `PostgreSQL` `Gemini API` `OpenCV`

[▶ Live](https://codebuzz-master.onrender.com/) · [⌥ Code](https://github.com/Prasenjit-Sahoo18/CodeBuzz49)

</td>
</tr>
</table>

<div align="center">

<a href="https://github.com/Prasenjit-Sahoo18/foodiez"><img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=Prasenjit-Sahoo18&repo=foodiez&hide_border=true&bg_color=050505&title_color=B8FF00&icon_color=00F5FF&text_color=F5F5F5"/></a>
<a href="https://github.com/Prasenjit-Sahoo18/Vybeon"><img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=Prasenjit-Sahoo18&repo=Vybeon&hide_border=true&bg_color=050505&title_color=B8FF00&icon_color=00F5FF&text_color=F5F5F5"/></a>

</div>

<br/>

<div align="center">

# 🛠️ TECH STACK

<img src="https://skillicons.dev/icons?i=python,java,cpp,c,typescript,javascript,html,css&theme=dark&perline=8"/>
<br/>
<img src="https://skillicons.dev/icons?i=nextjs,react,tailwind,vite,nodejs,express,django&theme=dark&perline=7"/>
<br/>
<img src="https://skillicons.dev/icons?i=postgres,prisma,mongodb,mysql,supabase&theme=dark&perline=5"/>
<br/>
<img src="https://skillicons.dev/icons?i=docker,aws,githubactions,vitest,linux,git,opencv&theme=dark&perline=7"/>

<br/>

![Socket.IO](https://img.shields.io/badge/Socket.IO-050505?style=flat-square&logo=socketdotio&logoColor=white)
![WebRTC](https://img.shields.io/badge/WebRTC-050505?style=flat-square&logo=webrtc&logoColor=00F5FF)
![Zustand](https://img.shields.io/badge/Zustand-050505?style=flat-square&logoColor=B8FF00)
![Auth.js](https://img.shields.io/badge/Auth.js-050505?style=flat-square&logo=authjs&logoColor=7C3AED)
![Zod](https://img.shields.io/badge/Zod-050505?style=flat-square&logo=zod&logoColor=3E67B1)
![Render](https://img.shields.io/badge/Render-050505?style=flat-square&logo=render&logoColor=B8FF00)
![Fly.io](https://img.shields.io/badge/Fly.io-050505?style=flat-square&logo=flydotio&logoColor=7C3AED)
![Gemini](https://img.shields.io/badge/Gemini_API-050505?style=flat-square&logo=googlegemini&logoColor=00F5FF)

</div>

<br/>

<div align="center">

# 🧭 LEVEL MAP

</div>

| 🟢 Daily driver | 🟡 Growing | 🟣 Next unlock |
|:--|:--|:--|
| Next.js · React · TypeScript · Node | Django · WebRTC · Socket.IO at scale | System Design (HLD / LLD) |
| Prisma · PostgreSQL · REST APIs | Docker · Render / Fly.io | AWS · CI/CD pipelines |
| Python · Java · C++ | AI API integration | AI Engineering · MLOps |
| Git · DSA on LeetCode | Competitive Programming | gRPC · Kafka · Redis |

<br/>

<div align="center">

# 📡 GITHUB SIGNAL

<img width="48%" src="https://github-readme-stats.vercel.app/api?username=Prasenjit-Sahoo18&show_icons=true&hide_border=true&bg_color=050505&title_color=B8FF00&icon_color=00F5FF&text_color=F5F5F5&include_all_commits=true&count_private=true&rank_icon=github"/>
<img width="40%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Prasenjit-Sahoo18&layout=compact&hide_border=true&bg_color=050505&title_color=B8FF00&text_color=F5F5F5&langs_count=8"/>

<img width="70%" src="https://streak-stats.demolab.com/?user=Prasenjit-Sahoo18&hide_border=true&background=050505&ring=B8FF00&fire=7C3AED&currStreakLabel=B8FF00&sideLabels=00F5FF&dates=8B8B9A&currStreakNum=F5F5F5&sideNums=F5F5F5&stroke=7C3AED"/>

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=Prasenjit-Sahoo18&bg_color=050505&color=B8FF00&line=7C3AED&point=00F5FF&area=true&hide_border=true&title=Contribution%20Activity"/>

<br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Prasenjit-Sahoo18/Prasenjit-Sahoo18/output/github-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Prasenjit-Sahoo18/Prasenjit-Sahoo18/output/github-snake.svg">
  <img alt="contribution snake" src="https://raw.githubusercontent.com/Prasenjit-Sahoo18/Prasenjit-Sahoo18/output/github-snake-dark.svg" width="98%">
</picture>

<br/><br/>

```
build → break → learn → ship → repeat
```

**Open to internships, collaborations and good conversations about code.**

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&section=footer&height=110&color=0:7C3AED,50:00F5FF,100:B8FF00"/>

</div>
