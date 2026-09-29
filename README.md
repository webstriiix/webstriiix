# 👋 Hi, I'm Surya Wiguna

Rust backend engineer — Denpasar, Bali, Indonesia.

I build high-performance backend systems, terminal applications, and smart contracts in Rust. Currently open to remote backend and Web3 roles.

## 🧑‍💻 About Me

I'm a backend engineer focused on Rust: high-performance APIs, CLI/TUI tooling, and systems programming. Since 2023 I've delivered end-to-end client projects — a pharmacy POS desktop app, a patient records backend with role-based access control and audit logging, and a multi-tenant CMS with third-party CRM integration.

In 2025 I worked two contracts: I migrated a legacy PHP monolith to Java Spring Boot microservices, cutting API response time from over 1,000 ms to under 100 ms, and I designed and deployed four production smart contracts for a token ecosystem on Ethereum-compatible chains, validated with Foundry and Hardhat test suites.

Right now I'm building a cross-platform D&D character sheet manager in Rust (TUI + API backend), shipping small CLI tools for cloud infrastructure workflows, and exploring how to run LLM inference on a decentralized, blockchain-coordinated compute network. <!-- VERIFY: kalimat terakhir adalah ide Decentralized AI L1 kamu — belum ada di CV; keep, reword, or delete -->

I'm open to remote full-time or contract work in Rust backend, systems programming, or Web3. <!-- VERIFY: CV tidak menyatakan ini eksplisit; sesuaikan kalau preferensimu beda -->

## 🛠️ Selected Projects

### [D&D Character Sheet Manager](https://github.com/webstriiix/cli_adventure_sheet)
**Problem:** Running a D&D 5e campaign means constantly juggling character stats, spells, slots, conditions, and inventory across sessions — usually on paper or in a spreadsheet.
**Solution:** A terminal-based character sheet manager with a full creation wizard, built in Rust with Ratatui and backed by a REST API.

- Step-by-step character creation wizard: race, class, ability scores, background, equipment, spells
- Combat tracking: death saves, spell slots, hit dice, conditions, and concentration
- Compendium browser for classes, races, spells, items, monsters, backgrounds, and feats
- Level-up with XP tracking, ASI, and feat selection; multiclass support
- JWT-based account system for syncing characters across devices

**Result:** Phase 1 (CLI MVP) complete and in public beta; actively gathering feedback from the D&D community.
`Rust` `Ratatui` `Axum` `SQLx` `PostgreSQL` `Tokio` `JWT + Argon2`

<!-- TODO: add a screenshot or GIF of the TUI (wizard + sheet tabs) -->
<!-- Backend lives in its own repo: https://github.com/webstriiix/backend_adventure_sheet -->

### [Omniroute Model Importer](https://github.com/webstriiix/omniroute-model-importer)
**Problem:** Registering cloud models on the OmniRoute dashboard was manual, one-by-one entry for 30+ models.
**Solution:** A Rust CLI that bulk-registers models from a JSON configuration file.

- Idempotent diffing: detects what changed before applying, preventing duplicate registrations
- Dry-run flag previews operations without side effects
- Modular architecture: config parser, API client, diff engine, and reporting subsystems

**Result:** Replaces manual dashboard entry for 30+ models with a single, repeatable command.
`Rust` `Tokio` `Reqwest` `Clap` `Serde`

<!-- TODO: repo ini belum punya README; tambah README + demo singkat (config in, diff out) -->

### [Aksara Auth API](https://github.com/The-Aksara/aksara-backend)
**Problem:** A web dApp needed a clean identity layer that connects email login with on-chain wallet bindings.
**Solution:** An Actix Web API with Google OAuth 2.0 login, user identity in PostgreSQL, and Solana (Phantom) wallet binding.

- Google OAuth 2.0 callback flow
- Phantom wallet association per user
- Diesel ORM + PostgreSQL with migrations
- Hosted on Shuttle

**Result:** Auth service for the Aksara dApp. <!-- VERIFY: repo bilang "hosted on Shuttle"; konfirmasi apakah sudah live production -->
`Rust` `Actix Web` `Diesel` `PostgreSQL` `Google OAuth 2.0` `Solana`

### [News API](https://github.com/webstriiix/news-api-rust)
**Problem:** A small content platform still needs secure auth, role-based access, and clean CRUD endpoints.
**Solution:** A REST API for users, categories, and news articles with JWT authentication and role-based access control.

- Secure login with bcrypt password hashing and JWT sessions
- Admin-only routes guarded by role-based access control
- Diesel migrations and a well-organized route structure

`Rust` `Actix Web` `Diesel` `PostgreSQL` `JWT`

## 💼 Selected Work

- **Freelance Backend Developer (Feb 2023 – present):** Delivered four end-to-end client projects — a pharmacy POS desktop app (Tauri + React + TypeScript), a patient records backend with role-based access control and audit logging, a multi-tenant CMS with CRM integration and automated tenant provisioning, and corporate profile websites.
- **Backend Developer, contract (Jun 2025 – Oct 2025):** Reduced API response time from over 1,000 ms to under 100 ms (10x+) by migrating a legacy PHP monolith to Java Spring Boot microservices; optimized MongoDB query patterns and indexing, reducing resource usage by ~40%.
- **Blockchain Developer, contract (Sep 2025 – Jan 2026):** Designed and deployed four production smart contracts for a token ecosystem — an ERC-20 with EIP-2612 permit, a multi-token presale accepting 7 assets with voucher-based KYC, an EIP-712 authorization contract with anti-replay protection, and a treasury contract for fee distribution and vesting — all validated with Foundry and Hardhat test suites.

## 🧰 Skills

| Area | What I use it for | Tools |
|------|-------------------|-------|
| Backend & systems programming | High-performance APIs, CLI/TUI apps, async services | Rust (Axum, Actix Web, Tokio, Ratatui, Serenity), Java (Spring Boot) |
| Blockchain | Smart contracts for token ecosystems; wallet and identity integrations | Solidity (ERC-20, EIP-712, EIP-2612), Foundry, Hardhat, ICP (dfx), XION, Solana |
| Databases | Schema design, query and index optimization | PostgreSQL, MongoDB, MySQL |
| Frontend & desktop | Desktop apps and web UIs | TypeScript, JavaScript, React, Tauri |
| Architecture | System design across client projects | Microservices, REST APIs, RBAC, multi-tenancy, BaaS vs self-host trade-offs |
| Infrastructure | Containerized deploys, CI, daily OS | Docker, GitHub Actions, Linux (Arch) |
| Also worked in | Prototypes and legacy code | C, Lua, PHP |

## 📬 Contact

- **Email:** suryawiguna0269@gmail.com
- **Phone:** +62 878-4007-9957
- **LinkedIn:** [linkedin.com/in/surya-wiguna](https://linkedin.com/in/surya-wiguna)
- **GitHub:** [github.com/webstriiix](https://github.com/webstriiix)
- **Instagram:** [instagram.com/webstriix](https://instagram.com/webstriix)
