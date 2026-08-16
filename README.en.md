# Eson Wong 汪毅盛

13 years of software engineering experience, long-time technical and team lead, focused in recent years on **enterprise AI adoption**. Currently at Guangzhou Danxiao Information Technology Co., Ltd. as **Head of the Enterprise AI Agent Platform** and **Head of AI Technology Application**, also leading the 20-person front-end team. Led the architecture and build-out of the company-wide AI Agent platform from 0 to 1, taking AI from pilot projects to everyday tooling across all business functions (marketing, product, QA, HR, legal, data, etc.); reshaped the engineering process with an "AI-generated code + CI gates + automated review" pipeline, and drove company-wide AI capability building. Skilled at combining technical architecture, engineering-process transformation, and organizational rollout so that AI actually gets used across the enterprise.

[中文版](./README.md)

## Personal Information

- Basic information: Male / 1990
- Mobile: 13265678623
- WeChat: EsonWong_
- Email: esonzero@gmail.com
- Expected job: Enterprise AI Application / AI Agent Platform Lead, AI Application Architect, AI Engineering Lead
- Work experience: 13 years
- Education: College / Hubei Vocational College / Computer Software Major

## Links

- Blog: <https://blog.esonwong.com>
- Twitter: [@eson000](https://twitter.com/eson000)
- Github: <https://github.com/esonwong>

## Project Experience

### Enterprise AI Agent Platform

🗓️ 2026/04 - Present

🏢 Guangzhou Danxiao Information Technology Co., Ltd.

A company-wide enterprise AI Agent platform whose goal is to **let everyone in the company solve their own job's problems with AI**. Built from 0 within half a year as platform lead and principal developer.

At its core is the **sub-app open platform**: business staff no longer wait on engineering — they self-apply, get a repo and credentials provisioned automatically, build an AI app for their own role with agents, and ship it; 8 business domains (marketing, product, QA, HR, legal, data, etc.) build on it. The platform exposes an **Agent API to every sub-app**, so each one is agent-capable by default, and business data flows back through these apps — making the platform the **convergence point for enterprise data and AI capability**. A **Skill Marketplace** captures reusable skills and installs them into Claude Code / Codex in one click so good practices travel between teams; **AI colleagues and scheduled tasks** keep agents resident in business roles, working on a schedule.

Foundation: **LangGraph / DeepAgents** orchestration, **RAG** enterprise knowledge base, **MCP** tool system (Streamable HTTP MCP server + PAT); SSO / OAuth, RBAC, multi-tenant isolation and skill review keep "anyone can build" manageable and auditable.

Impact and key results:

- **154 business sub-apps** launched company-wide, **97% built self-service by business teams**, with **43** business co-builders across 8 domains; **130 installable skills** accumulated in the Skill Marketplace.
- Established an "AI-generated code + CI gates + automated review" engineering pipeline, automating code review, merging, and production-alert handling with agents: team code merge wait time **dropped from about a day to under an hour** while engineering output doubled.
- Led company-wide AI adoption: founded and led a 17-person AI pioneer team, delivered three large tech-sharing sessions reaching 133 attendees; provided a one-command-install AI toolkit for non-engineering roles.

I am responsible for the overall technical architecture, technology selection, and core feature development of the platform, and lead the company's AI engineering process standards and adoption.

### Vibemate Mobile

🗓️ 2025/02 - 2026/04

🏢 Guangzhou Danxiao Information Technology Co., Ltd.

The mobile product of Vibemate, extending the desktop client's optimized live-streaming viewing experience to mobile. As the project's **technical lead**, I was responsible for mobile architecture and team leadership, and led the **adoption of AI features in the product**.

### Vibemate PC

🗓️ 2023/06 - 2025/02

🏢 Guangzhou Danxiao Information Technology Co., Ltd.

A desktop browser product that optimizes the live-streaming viewing experience, providing users with a smoother, more immersive live-streaming experience. Built as a cross-platform desktop application with **Electron**.

As the project's **technical lead**, I was responsible for the desktop technical architecture, technology selection, team leadership, and core feature development.

### Fanberry

🗓️ 2022/4 - 2023/7

🏢 Guangzhou Danxiao Information Technology Co., Ltd.

🔗 <https://fanberry.com>

Personal IP operation, fan operation, and charging tools. Supports multiple complex interactions, and uses CSS animation to achieve smooth drag and edit interaction effects.

This project uses **Vue3** and **Typescript** as the development framework and language. Use **Nuxt.js** to develop the **server-side rendering SSR** framework to meet the project's **SEO** requirements. The **adaptive layout** solution realizes friendly experience for mobile and desktop and different resolutions.

I am responsible for the front-end architecture and business development of the Fanberry project.

### Cam Extension

🗓️ 2020/08 - 2023/06

🏢 Guangzhou Danxiao Information Technology Co., Ltd.

Chrome and FirFox browser plug-in products, serving users who live broadcast in the browser. This project combines the company's hardware products to realize the interaction and interaction between the audience and the live broadcaster, and provides safe and easy-to-use APIs and **Developer documentation** for live broadcast platforms and other developers.

This project is developed using Java, MySql, **Vue**, and **Browser Extension API**.

I am responsible for project architecture development, business function development, project progress management, and support for integration of third-party developers.

## Side Projects

### Personal AI Agent Remote Control & Approval System

🗓️ 2026/07 - Present

Uses Claude Code sessions on multiple machines as the AI engine; dispatch tasks, follow progress, **approve tool permissions remotely**, switch models and restart sessions from iPhone / Apple Watch / Widget / Siri / Live Activity and Feishu. Cloudflare Worker + Durable Object backend, APNs push, WebSocket wake-up of per-machine bridges; built TDD. A personal proving ground for the AI-colleague and permission-governance ideas used at work.

### Eva · Self-built Home Voice AI Assistant

🗓️ 2026/07 - Present

A voice agent built end to end, from wake word to home control. Raspberry Pi as the voice terminal: always-on local keyword spotting, PortAudio full-duplex + AEC enabling barge-in while speaking; Mac mini as the brain: a Python asyncio session state machine with energy VAD segmentation → offline ASR (audio.cpp / Qwen3-ASR) → streaming LLM → sentence-level streaming TTS, ~2 s end-to-end first response; a Xiaomi touch speaker reflashed as the display terminal (Compose app: eye expressions / clock / notification glance); a self-hosted Matter fabric controlling curtains, light strips and temperature/humidity sensors. On top, **Pi Agent** runs sandboxed in Docker as the household agent: tasks recognized mid-conversation are delegated to it to manage lists / to-dos / schedules and appliance state, with `/workspace` as its long-term memory; plus scheduled tasks, daily memory consolidation ("dreaming", can draw to the e-ink screen), and a per-turn JSONL ledger with wake-word evidence for observability and training-sample collection.

### Somatic Corridor

🗓️ 2026/06

🔗 <https://running.esonwong.com>

A first-person endless corridor game driven by the webcam: jump / crouch / sidestep / punch recognized in real time. Pure front-end pose estimation + WebGL; taken from idea to launch in half a day with AI assistance.

### E-ink Todo List

🗓️ 2024/02 - Present

🔗 <https://einktodo.com> · [GitHub ★42](https://github.com/esonwong/e-ink-todo-list)

An e-ink to-do list built end to end: ESP32 firmware and custom PCB, Next.js web app, iOS app (Sign in with Apple / GitHub), CI/CD and E2E tests. Ships an **MCP server and a Claude Skill** so AI agents can push schedules, summaries and images straight to the physical screen — turning a device into a tool agents can call.

### Network-RC

🗓️ 2020/4 - 2023/8

🏢 Personal project

🔗 [GitHub ★274](https://github.com/esonwong/network-rc)

4G/5G remote network remote control car/robot system. Based on Raspberry Pi and RC remote control car hardware, using computer or mobile phone browser interaction control, realized with multi-camera low-latency network image transmission and voice intercom. The controlled end uses **NodeJS** to control the hardware, using **WebRTC** point-to-point communication technology and self-implemented frame-by-frame encoding video stream to achieve low-latency transmission of video images and bidirectional audio streams. The control end uses **React** to build interactive UI. Experimented with TTS, gravity sensing control, GamePad control, intranet penetration, gimbal control, **AI driving**, and other features. Personal experimental entrepreneurial project.

In this project, I achieved the **lowest video latency** of network remote control cars on the market.

### Also

- **esp-matter-window**: battery-powered Matter-over-Thread window opener (XIAO ESP32-C6 / ESP-IDF) working with Apple Home
- **I'm Listening**: web app generating personalized listening material with LLM + TTS

## Earlier Projects

### Garden Help

🗓️ 2019/2 - 2020/3

🏢 Beijing Garden Artery Network Technology Co., Ltd. / Remote

This project is an industry management software that serves the vertical field of garden construction and construction industry, including construction worker attendance management, construction project tracking management, enterprise data file management, enterprise process and organizational structure management, etc.

This project is mainly developed using Laravel, **Vue**, **Cordova**, and **Electron**.

I am responsible for the architecture and development of the web client on the desktop and mobile, the architecture and development of the Android and iOS App clients, and the development of the Windows and Mac client programs in the project.

### Fakeshion Mall

🗓️ 2018/7 - 2019/2

🏢 Dianzhan Technology / Remote

This project is a mall system based on WeChat applets.

It includes a small program client and a web background management system. The background management includes functions such as product management, order management, after-sales management, and sales data charts, developed using **React** framework, **Antd UI library**, **BizCharts chart library**, and other technologies.

I developed the front-end part of the remote background management system in this project.

### Shuibei Smart Cloud

🗓️ 2018/4 - 2018/8

🏢 Yanoxin Group

This project is a 2B system that provides data collection and analysis of customer traffic information, customer operation promotion integration for offline chain stores.

Using face recognition, wifi probes and other technologies to collect offline customer flow data, analyze store customer flow attributes, and provide accurate data for store operations. The front-end part of the project uses **React** + **Redux** + **Webpack** + **Babel** + **ES7** technology stack development. Use **Antd UI library**, BizCharts chart library.

I am responsible for the planning and management of the project, team building, and the architecture and business development of the project front-end refactoring.

### Cunjin Niu

🗓️ 2017/3 - 2018/3

🏢 Shenzhen Donghuang Network Technology Co., Ltd.

This project is an O2O Internet model financial investment and wealth management service software system.

It includes clients, management background, income calculation system, and gold store client, including PC, mobile, and Android and IOS App. I led a front-end team of 3 people to continuously integrate and develop the client and gold store parts of this project. The mobile and PC sides of the client use **React** + Redux + Webpack + Babel + ES6 architecture development, and the Android and IOS sides use **Cordova hybrid App** technology development. The gold store client uses **Vue** + Webpack + Babel + ES6 architecture development. Implemented many functions such as customer purchase of financial products and related process functions, operation and promotion requirements, real-time gold prices, gold price trends, etc.

Responsible for the architecture of the front-end project, technical selection, front-end development and architecture of Android and IOS **hybrid App** clients, and project progress management for part of the project cycle.

### Agent Operation

🗓️ 2016/3 - 2017/3

🏢 Shenzhen Duoyoumi Network Technology Co., Ltd.

Enterprise operation and taxation e-commerce projects, which are services for financial and taxation enterprises to bring more traffic and sales to financial and taxation enterprises.

This project includes a complete e-commerce system, as well as a promotion Q&A system and CMS system. This project includes JAVA-developed APIs. Developed using **NodeJS** + **React** web site, including mobile and PC. **Front-end and back-end are the same**, ensuring development efficiency and experience. Supports server-side direct output and has good **SEO** support.

In the project, I am responsible for the development environment construction of the front-end, technical architecture, project construction, API specification customization, and web development of the PC side.

### Yidai Network

🗓️ 2013/10 - 2015/10

🏢 Yidai Group

Travel accommodation OTA platform.

Using **NodeJS** and **Gulp** to build the project's front-end development environment, using front-end frameworks and libraries such as Jquery and **React** in conjunction with .Net backend development. Using agile development mode, updated every two weeks.

Fully participated in the project. In the early stage, I was responsible for the front-end development and architecture of the project. Planned the project development cycle and led the team to develop the project.

### Yousikemei Official Website

🗓️ 2012/12-2013/10

🏢 Yousikemei

An official website for an education and training institution aimed at overseas exams for middle and young people.

I am responsible for the interaction development and **SEO optimization** of the project.

## Skills

- JavaScript, HTML5, CSS3
- React, Vue2, Vue3
- Nodejs
- Webpack, Babel
- Cordova hybrid App
- Electron desktop program
- AI application architecture: LLM application design, RAG enterprise knowledge bases, agent orchestration (LangGraph / DeepAgents), MCP tool systems, multi-tenant AI platforms, permission and credential governance
- AI coding / agent tools: Claude Code (primary), Codex, Pi Agent, OpenClaw, GitHub Copilot (agent-driven day-to-day development; team-scale adoption and skill / workflow distribution)
- AI engineering: CI gates and automated review for AI-generated code, agent-run operations, skill capture and distribution
- Git

## Acknowledgments

Thank you for taking the time to read my resume and look forward to the opportunity to work with you.
