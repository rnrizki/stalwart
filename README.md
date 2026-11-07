# Stalwart Mail Server (RajaEmas)

All-in-one Mail & Collaboration server configured for the RajaEmas infrastructure on Dokploy with JMAP, IMAP, SMTP, CalDAV, and CardDAV support.

## Architecture & Configuration
- **Mail Server:** Stalwart Mail Server v0.16.21
- **Domain:** `https://mailserver.lmrei.id`
- **JMAP Endpoint:** `https://mailserver.lmrei.id/.well-known/jmap` -> `/jmap/session`
- **Database:** Internal Dokploy PostgreSQL (`database-postgresql-fy9a1w:5432/stalwart1`)
- **Web Admin & User Portal:** Port 8080 (Mapped locally to 8079 for Traefik SSL reverse proxy)

## Services & Ports
- **SMTP Submission:** 587, 465, 25
- **IMAP:** 143, 993
- **POP3:** 110, 995
- **ManageSieve:** 4190
- **HTTP / JMAP API:** 8080
