<div align="center">

<h1>Ryan Brinkman</h1>

<b>Cybersecurity &middot; Backend &amp; Systems &middot; North Dakota</b>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=15&pause=1000&color=0AAAFF&center=true&vCenter=true&width=640&lines=Cybersecurity+%26+Computer+Networks+student;I+ship+real+systems+to+learn+by+building;Python+%7C+Kotlin+%7C+Java+%7C+C%2B%2B;FastAPI+%7C+Postgres+%7C+Linux+%7C+AI+agents+%7C+Automation)](https://github.com/RyanBrin)

<p>
  <a href="https://discord.com/users/852979622709690438"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white"/></a>
  <a href="https://linkedin.com/in/ryan-brinkman"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://twitter.com/_ryanbrin"><img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white"/></a>
  <a href="mailto:ryanjbrinkman@outlook.com"><img src="https://img.shields.io/badge/Email-0078D4?style=for-the-badge&logo=microsoft-outlook&logoColor=white"/></a>
</p>

<img src="https://komarev.com/ghpvc/?username=ryanbrin&label=Profile+Views&color=0AAAFF&style=flat-square"/>

</div>

---

## About me

I'm a **Cybersecurity & Computer Networks** student at Bismarck State College who
learns by shipping systems that actually run in production — with real users, real
deploys, and real consequences when something is wrong. The hard parts (auth,
persistence, safety rails, honest failure states, deployment) are the curriculum.

```python
ryan = {
    "location":   "Bismarck, North Dakota",
    "education":  "Cybersecurity & Computer Networks — Bismarck State College",
    "focus":      ["Security", "Networking", "Backend", "Linux", "AI agent orchestration"],
    "building":   "Nexus — a personal operations platform: manual-first trading, "
                  "network visibility, and a voice assistant, run by a fleet of AI agents",
    "principle":  "If it doesn't run in production, I haven't really learned it yet",
}
```

> Most of my source is private by design. The **`*-demo` repos below are public
> overviews** — architecture and engineering decisions, no secrets and no real data.

---

## Flagship — the Nexus platform

### 🛰️ [Nexus](https://github.com/RyanBrin/nexus-demo)
A **multi-user personal operations platform** (FastAPI + vanilla JS, deployed on
Railway) built around three pillars:

- **Manual-first trading OS** — plan → confirm → journal workflow over stocks and
  crypto, with a reconciled portfolio view and a paper ledger. **Paper-only by
  hard rule**: nothing simulated ever touches real money, and the platform never
  places an order.
- **OMNISENSE visibility** — a device-identity layer that fuses LAN and RF
  observations into one durable device database, with alerting, incident
  storm-capping, and a dark-launched notification outbox (deny-by-default
  delivery gates, idempotent, replay-safe).
- **Operator console** — an owner-gated control plane separated from the user
  product, with signed sessions, opt-in 2FA, strict-nonce CSP, and honest
  failure states (a failed health check never renders as "all clear").

Engineered like a real product: HMAC-signed sessions, Postgres durability,
server-sent events for real-time UI, an in-repo engineering registry with
one-command visual/interaction audit harnesses, and deploy verification that
diffs production against the working tree byte-for-byte.

`Python` · `FastAPI` · `Postgres` · `SSE` · `Railway` · `vanilla JS` · `Playwright audits`

### 📈 [Hermes](https://github.com/RyanBrin/hermes-trading-demo) · *the trading core*
The trading core inside Nexus — **manual-first and paper-only**. An earlier
autonomous paper-research engine (Elliott Wave / Fibonacci over BTC·ETH·SOL plus a
stock scanner) was retired non-destructively into a legacy archive with boundary
tests that keep it retired; today's core is deliberately human-in-the-loop, with
hardcoded risk floors and a safety-invariant file that CI and every AI agent must
obey.

`Python` · `risk gating` · `paper-only` · `archive-boundary tests`

### 📡 [LAN Monitor](https://github.com/RyanBrin/lan-monitor-demo) · *feeds OMNISENSE*
An always-on **Raspberry Pi appliance** that passively inventories the home
network (neighbor-cache only — no probing), pushes sensor data to Nexus over a
token-scoped API, and serves a loopback-only local dashboard. Privacy-first:
inventory, never surveillance.

`Python` · `Linux` · `systemd` · `push-model sensors`

### 🎙️ Voice assistant · *private*
A wake-word voice layer over the same ecosystem — an always-on local assistant
with a TV HUD, singleton/supervisor reliability, and a permission-guard that
hard-blocks publish/deploy actions even when its AI agent runs unattended. Built
AI-first: the assistant delegates real work to CLI agents and reports honestly
when a delegated run fails.

`Python` · `STT/TTS` · `agent delegation` · `fail-closed guards`

### 📅 [Work Schedule Sync](https://github.com/RyanBrin/work-schedule-sync-demo)
A Google Apps Script that turns pasted work-schedule text into calendar events —
a deterministic parser, no OCR, no AI required. Feeds both Google and Outlook
calendars via iCal subscription.

`Google Apps Script` · `Calendar API`

### 📱 [Personal Dashboard App](https://github.com/RyanBrin/dashboard-demo)
An Android command-center experiment (Kotlin / Jetpack Compose) — the prototype
that taught me what Nexus needed to be. Superseded, kept for history.

`Kotlin` · `Jetpack Compose`

---

## How I build

- **AI-agent engineering, done carefully.** I run coordinated fleets of AI coding
  agents with explicit lane ownership, adversarially-verified multi-agent code
  review, and hard human gates on anything that ships — pushes, auth changes, and
  money-adjacent code always require my word.
- **Audits over assumptions.** The platform carries its own audit tooling:
  Playwright interaction crawls that click every control, visual regression
  receipts, failure-injection tests that catch a UI lying about errors, and
  deploy verification that never trusts a green build message.
- **Safety invariants as code.** Paper-only trading, deny-by-default delivery
  gates, fail-closed authorization — written down, tested, and enforced against
  both humans and AI agents.

---

## Skills & tools

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![HTML/CSS](https://img.shields.io/badge/HTML%2FCSS-E34F26?style=flat-square&logo=html5&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Backend & platform**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![Android Studio](https://img.shields.io/badge/Android%20Studio-3DDC84?style=flat-square&logo=androidstudio&logoColor=white)

---

## What I'm learning

| Area | Working on |
|---|---|
| Security | Auth design, fail-closed authorization, secure configuration, threat detection |
| Networking | Subnetting, routing protocols, packet analysis, passive device identity |
| AI engineering | Multi-agent orchestration, adversarial review, permission-guarded autonomy |
| Linux | System administration, systemd services, shell scripting |
| Cloud | Operating production services — deploys, verification, cost containment |

---

## GitHub stats

<div align="center">

[![Followers](https://img.shields.io/github/followers/RyanBrin?style=for-the-badge&logo=github&logoColor=white&label=Followers&color=0AAAFF&labelColor=0d1117)](https://github.com/RyanBrin?tab=followers)
[![Nexus stars](https://img.shields.io/github/stars/RyanBrin/nexus-demo?style=for-the-badge&logo=github&logoColor=white&label=Nexus%20stars&color=0AAAFF&labelColor=0d1117)](https://github.com/RyanBrin/nexus-demo)
[![Nexus updated](https://img.shields.io/github/last-commit/RyanBrin/nexus-demo?style=for-the-badge&logo=git&logoColor=white&label=Nexus%20updated&color=0AAAFF&labelColor=0d1117)](https://github.com/RyanBrin/nexus-demo)

<sub>Most of my work lives in private repos &mdash; the <code>*-demo</code> repos above are public windows into it.</sub>

</div>

---

<div align="center">
<sub>Built in North Dakota &middot; Paper-first, safety-first &middot; Always learning by shipping</sub>
</div>
