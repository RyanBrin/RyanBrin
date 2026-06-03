### Hey, I'm Ryan 👋

I build personal systems that actually run — autonomous trading bots, mobile apps, and workflow automation. Everything I ship is production-deployed and actively used.

---

#### 🤖 What I'm building right now

**[Nexus](https://github.com/RyanBrin/nexus)** — a personal command-center ecosystem:

| Project | Description | Status |
|---------|-------------|--------|
| [**hermes-trading**](https://github.com/RyanBrin/hermes-trading) | Autonomous BTC + stock trading bot — Elliott Wave/Fibonacci strategy, AI reflection, risk firewall, real-time dashboard | [![live](https://img.shields.io/badge/-live-22c55e?style=flat-square)](https://hermes-trading-production-c312.up.railway.app) |
| [**dashboard-api**](https://github.com/RyanBrin/dashboard-api) | Personal banking API — Plaid integration, live balances, transaction history, Fidelity holdings | [![live](https://img.shields.io/badge/-live-22c55e?style=flat-square)](https://dashboard-api-production-ebee.up.railway.app) |
| [**dashboard-app**](https://github.com/RyanBrin/dashboard-app) | Android command-center — calendar, budget, trading, banking, work shifts, push notifications | ![android](https://img.shields.io/badge/-Android-3b82f6?style=flat-square) |
| [**work-schedule-sync**](https://github.com/RyanBrin/work-schedule-sync) | Google Apps Script — Claude Haiku OCR reads schedule screenshots and syncs shifts to Google Calendar automatically | ![apps script](https://img.shields.io/badge/-Apps%20Script-34a853?style=flat-square) |

---

#### ⚡ Hermes Trading Bot

The main thing I'm working on — an autonomous paper trading system that:

- Scans **30 stocks** using Elliott Wave + Fibonacci retracement analysis
- Tracks **setup types** (retracement entry, breakout continuation) with confidence scoring
- Has a **hardcoded risk firewall** that AI cannot modify — enforces stop sizes, R/R minimums, position limits
- Uses **Claude Haiku** for per-scan natural language analysis and **Claude Sonnet** for batch strategy reflection
- Logs every trade idea with full rejection reasoning, stored in Supabase
- Must prove **positive expectancy over 100+ paper trades** before advancing to live capital

Live dashboard → [hermes-trading-production-c312.up.railway.app](https://hermes-trading-production-c312.up.railway.app)

---

#### 🛠 Tech I use

![Python](https://img.shields.io/badge/Python-3b82f6?style=flat-square&logo=python&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7c3aed?style=flat-square&logo=kotlin&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-22c55e?style=flat-square&logo=fastapi&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-3b82f6?style=flat-square&logo=android&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-22c55e?style=flat-square&logo=supabase&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-6366f1?style=flat-square)
![Anthropic](https://img.shields.io/badge/Claude%20AI-f59e0b?style=flat-square)
