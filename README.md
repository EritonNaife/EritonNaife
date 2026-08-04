## Eriton Naife

**Software Engineer — Backend & Full-Stack.** Porto, Portugal.

I build and ship production backends in **Go** and **Python/Django** — REST APIs, PostgreSQL data models, authentication, payments — with the Docker and CI/CD plumbing around them. Front-ends in SvelteKit/TypeScript and React Native (Expo) when a product needs one.

Currently in the Common Core at **42 Porto**, deepening systems fundamentals in C.

### What I work on

**An API-first modular monolith (Go).** One binary of independently owned modules — identity, organizations, access control, payments, finance, ledger, audit, locations, mail, notifications, files — each owning its own PostgreSQL schema, its own migrations and its own route prefix. Dependency direction is enforced by consumer-defined interfaces, so providers never import their consumers. The money path is deliberately split across three modules — PSP-agnostic collection, an immutable double-entry ledger, and a single ledger writer — so no module owns two bounded contexts.

**A business operating system for nightlife event organizers.** Built as a product on that platform, consuming its identity, payments and notification modules rather than carrying its own. Three clients on shared REST contracts: an attendee web app, an organizer web app, and a staff door-scanner on Tauri v2 (SvelteKit webview, Rust core).

**An installment-based fintech (Python/Django).** Client project. Django/DRF modular monolith: phone + OTP + PIN authentication, idempotent payment recording, a rules-based trust score, disputes and notifications — with a React Native (Expo) customer app and a SvelteKit PWA for merchants.

These repositories are private — pre-launch and client work. Happy to walk through the architecture or give a demo on request.

### Stack

| | |
|---|---|
| **Backend** | Go (chi, golang-migrate) · Python/Django + DRF · REST API design |
| **Data** | PostgreSQL (schema-per-module) · SQL · double-entry ledgers |
| **Auth** | WebAuthn · JWT · OTP · rotating refresh tokens |
| **Front-end** | SvelteKit 5 · TypeScript · React Native (Expo) · Tauri v2 |
| **Infrastructure** | Docker · CI/CD (GitLab CI, GitHub Actions) · OpenTofu · Ansible · Proxmox/LXC · Traefik · Linux |
| **At 42 Porto** | C — systems, memory management, computing fundamentals |

### Elsewhere

[LinkedIn](https://www.linkedin.com/in/eritonnaife) · naifeeriton@gmail.com

Open to backend, full-stack, and platform-leaning roles — remote or Porto-based.
