# Ryan Brin

Security-minded software developer building practical automation, data systems, and local-first tools.

I learn in public, but I design for privacy: keep secrets out of source control, minimize exposed infrastructure, make safety constraints visible, and prefer deterministic behavior where mistakes would be expensive.

## Signature work

### Hermes Trading

A paper-trading research platform built around explainable decisions and defensive risk controls. The project separates market interpretation from deterministic execution rules and provides a dashboard for reviewing signals, rejections, and system state.

**Python · FastAPI · PostgreSQL · market-data integrations · safety-first automation**

[View project](https://github.com/RyanBrin/hermes-trading)

### Agent LAN Monitor

A local-first network inventory and reporting tool for authorized environments. It emphasizes conservative scanning, deterministic change detection, read-only reporting surfaces, and optional local-model interpretation.

**Python · local JSON API · inventory diffing · security tooling**

[View project](https://github.com/lucidshift/Agent-LAN-Monitor)

### Nexus

A Kotlin/Jetpack Compose Android dashboard backed by a small FastAPI service. It brings schedule, finance, and trading summaries into one interface while keeping credentials and sensitive provider access on the appropriate side of the client/server boundary.

**Kotlin · Jetpack Compose · FastAPI · Room · Retrofit**

[Android app](https://github.com/RyanBrin/dashboard-app) · [API](https://github.com/RyanBrin/dashboard-api)

### Work Schedule Sync

A deterministic scheduling workflow that turns differently formatted shift inputs into normalized calendar events. It focuses on idempotent updates, conflict reporting, and avoiding destructive calendar automation.

**Google Apps Script · calendar automation · parsing · notifications**

[View project](https://github.com/RyanBrin/work-schedule-sync)

## How I build

- Put safety checks around automation that can affect money, devices, or personal data.
- Keep AI assistance advisory; deterministic code owns validation and state changes.
- Favor observable systems with clear logs, status surfaces, and failure modes.
- Treat privacy cleanup and documentation as part of shipping—not an afterthought.

## Current direction

I am continuing to deepen my work in cybersecurity, backend systems, Android development, and dependable automation. My older language repositories remain available as a record of the fundamentals that led to these larger systems.

The safest way to reach me is through my public GitHub profile.
