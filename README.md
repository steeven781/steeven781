<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:1e3a8a&height=200&section=header&text=Steeven%20Medina&fontSize=50&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Senior%20QA%20Engineer%20%7C%20Automation%20Architect&descAlignY=60&descSize=18&v=3" width="100%"/>
</p>

<p align="center">
  <a href="https://steevencodeqa.netlify.app"><img src="https://img.shields.io/badge/Portfolio-steevencodeqa.netlify.app-0f172a?style=for-the-badge&logo=netlify&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/steevenm7/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:stevenmedina781@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

<p align="center"><i>"I build tools for the people who verify software — and production systems for real businesses."</i></p>

---

### 🧭 What I Build

- **🧪 QA & testing tools** — I build products *for* the people who verify software: test case management platforms, agentic QA ecosystems, execution dashboards. A QA engineer who builds his own tooling.
- **🏢 Multi-tenant SaaS in production** — Real systems with real users: condominium administration, live-commerce with real-time raffles, AI analytics for SMEs — with production discipline: versioned migrations, RLS, RBAC, rate limiting, error tracking.
- **🤖 Infrastructure for AI agents** — MCP servers, publishable Claude Skills, and formally documented multi-agent development workflows. Not "I called an AI API" — building the infrastructure agents actually work on.

Across all three: unusually rigorous documentation — numbered ADRs, security models written *before* the code, disk-based kanbans, honest risk logs, and AI-assisted dev workflows (Claude implements / Codex reviews) codified as formal process.

### 🚀 Currently

Building **Numia** — a business intelligence SaaS for SMEs that connects to their existing databases and delivers AI-powered insights straight to WhatsApp.

### 🛠️ Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=py,fastapi,ts,react,nextjs,go,dotnet,supabase,docker&theme=dark" />
</p>
<p align="center">
  <img src="https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white" />
  <img src="https://img.shields.io/badge/MCP-000000?style=for-the-badge" />
</p>

---

### 🏗️ Systems I've Built

Products I designed, built, and shipped with full ownership — from problem definition to production.

<details>
<summary><b>Integrity</b> — Multi-tenant Condo Management SaaS &nbsp;·&nbsp; <i>Production · 2026</i></summary>
<br>

*An expanded, multi-tenant evolution of an earlier product (Nexus Admin) — grown from a single condominium's tracking site into a SaaS serving multiple independent communities.*

**Problem**
Residential communities managed payments, access control, maintenance reports, and resident data through spreadsheets and manual phone coordination — no audit trail, no self-service, and no way to onboard a new community without rebuilding the whole setup.

**Contribution**
Built a full multi-tenant SaaS with RLS-backed tenant isolation validated by a dedicated isolation test suite; a complete financial subsystem as pure, tested functions (prorated fee schedules, bulk charge publishing, payment application, late fees, statements, expense tracking); per-tenant feature-flagged modules (new modules ship off for everyone by default); OCR for national ID cards and payment receipts; QR-based visitor passes; three separate auth surfaces (public + reCAPTCHA, resident OTP, admin RBAC) plus a super-admin tenant-provisioning area.

**Impact**
1,589 commits and 150k+ lines of code in active production, with 62 numbered SQL migrations and 117 test files (~17k assertions across unit, e2e, and dedicated isolation suites) — running live across multiple independent communities.

`Next.js 16` `React 19` `TypeScript` `Supabase` `Cloudflare R2` `Upstash Redis` `Tesseract.js` `Vitest` `Playwright`

*Founder &amp; Solo Developer — end-to-end ownership*
</details>

<details>
<summary><b>raffle-pro</b> — Live-Raffle &amp; Commerce Platform &nbsp;·&nbsp; <i>Production v1.0.0 · 2026</i></summary>
<br>

**Problem**
A live-commerce business running raffles during Facebook Live streams tracked purchases and drew winners manually, with checkout coordinated ad hoc over WhatsApp DMs and no auditable link between what was purchased and who won.

**Contribution**
Built a production live-raffle and e-commerce platform solo: real-time purchase registration during live draws, purchase-weighted raffle selection, an animated 3D "treasure chest" reveal, a public storefront with WhatsApp checkout, and a full back-office (orders, products, customers, finance, users). Added versioned SQL migrations with up/down/verify tooling and a matching CLI, and documented a formal multi-agent AI development workflow (Claude implements from a ready-queue, Codex reviews) with CI enforcing migration and test gates on every PR.

**Impact**
Replaced ad hoc, error-prone raffle bookkeeping with an auditable platform running in production for a real e-commerce business, with real CI (migrations + build + tests on every PR) and an AI-assisted dev process that keeps the codebase moving fast without skipping review.

`Vite` `React 18` `React Router 7` `Turso (libSQL)` `Netlify Functions` `Cloudflare R2` `Upstash Redis` `Sentry` `React Three Fiber` `Vitest`

*Founder &amp; Solo Developer — end-to-end ownership*
</details>

<details>
<summary><b>TestMan</b> — QA Test Management Platform &nbsp;·&nbsp; <i>v1.0.0 Released · AI-Assisted · 2026</i></summary>
<br>

**Problem**
QA teams — including on my own projects — tracked test cases, test plans, and run results in spreadsheets: no reusable plans, no versioned run history per release, no pass/fail dashboard, and every failed test meant manually copying details into a Jira ticket.

**Contribution**
Built a multi-project test management platform solo, including migrating off a third-party auth provider to a self-owned auth system (scrypt hashing, opaque sessions with sliding 12h expiry, lockout, email 2FA) — with the security plan written *before* the code and validated with mutation testing that caught a real vulnerability pre-ship. Added a Gemini-powered test case drafting feature with structured-only output and a hard, server-enforced daily AI budget per user/project with real token/cost accounting; fail-closed project isolation; test runs that snapshot content at generation time (a retest is a new attempt, never an overwrite); and a Jira Cloud integration with AES-256-GCM-encrypted per-user tokens.

**Impact**
312/312 unit tests and 17/17 e2e tests gate every development phase; running in production across two live projects, with AI-assisted drafting cutting the time to write new test cases and the Jira integration removing the manual step of turning a failed test into a ticket.

`Next.js 16` `React 19` `TypeScript` `Turso (libSQL)` `Drizzle ORM` `Gemini API` `Jira Cloud API` `Playwright`

*Founder &amp; Solo Developer — end-to-end ownership*
</details>

<details>
<summary><b>Numia</b> — BI SaaS for SMEs &nbsp;·&nbsp; <i>Side Project · Active MVP · 2026</i></summary>
<br>

**Problem**
SMEs running old, un-upgradeable versions of the Aspel SAE ERP accumulate years of transactional data but have no real-time visibility into overdue collections, dead inventory, or margin leaks.

**Contribution**
Architected a clean separation between a SELECT-only database connector, a pure-function analysis engine (one function per business question — collections, dead inventory, price leaks, churn, profitability), and an AI/reporting layer whose test suite runs without a live database connection. Built a cross-platform installable agent with CI-driven builds for four targets (Windows, macOS, Linux x64/arm64) so it runs directly on a client's own server, with graceful degradation to a template-based summary when no AI key is configured.

**Impact**
212 Python tests and 102 TypeScript test files back the platform; recent commits show active security hardening (session revocation, anti-lockout, injection escaping) as it moves toward real customers, with a daily AI-written WhatsApp executive summary as the core subscription value.

`Python 3.12` `FastAPI` `pandas` `pymssql` `PyInstaller` `Anthropic SDK` `Next.js 16` `Turso (libSQL)` `Drizzle ORM`

*Founder &amp; Solo Developer — end-to-end ownership*
</details>

---

### ⚙️ Engineering Practices I Care About

- Versioned SQL migrations with `up` / `down` / `verify` tooling — not "run and hope"
- Security models and ADRs written **before** the code, not documented after the fact
- Mutation testing on authentication code — proof the tests catch real bugs, not just coverage
- Multi-tenant isolation treated as its own tested surface, not an assumption
- AI usage budgets enforced **server-side**, never left to client trust
- Multi-agent AI development workflows (implementation + independent review) formalized as process

---

### 💼 Professional &amp; Client Work

<details>
<summary><b>Contract-First API + UI Test Framework</b> &nbsp;·&nbsp; <i>Work Project · 2025</i></summary>
<br>

*Built for a client engagement — described here at the architecture level; product and client details withheld for confidentiality.*

Designed a Playwright test architecture where typed API clients and spec scaffolds are generated directly from the OpenAPI/Swagger contract, so a new endpoint is one regeneration away from coverage. Added a shared, cloud-stored authenticated session for UI tests, multi-environment configuration, and tagged smoke/regression suites wired into CI with Allure reporting.

`Playwright` `TypeScript` `OpenAPI/Swagger codegen` `AWS Secrets Manager` `Allure`

*Test Automation Architect*
</details>

<details>
<summary><b>Enterprise Warehouse &amp; ERP Systems</b> &nbsp;·&nbsp; <i>Work Project · .NET</i></summary>
<br>

Two internal systems built on .NET 8 + React: a warehouse logistics platform (picking → route assignment → QR-based decremental package scanning → delivery confirmation, with separate desktop/mobile interfaces), and an order-taking tool that reads and writes to a legacy ERP exclusively through parameterized stored procedures, with a data-driven permission system — adding a new page is a database insert, not a code deploy.

`.NET 8` `ASP.NET Core` `Entity Framework Core` `React` `SQL Server`

*Software Engineer*
</details>

<details>
<summary><b>Música y Audio Soluciones</b> — E-commerce landing &amp; catalog &nbsp;·&nbsp; <i>Guatemala</i></summary>
<br>

Landing page and product catalog for a music and pro-audio retailer. No backend — the catalog is fetched live from a Google Sheets API, with category/brand filtering, a deals carousel, and a WhatsApp-based purchase flow.

`Webpack 5` `Tailwind CSS v4` `Alpine.js` `ApexCharts`
</details>

<details>
<summary><b>FFCI Guatemala</b> — Marketing &amp; booking site &nbsp;·&nbsp; <i>Guatemala</i></summary>
<br>

Site for a leadership training and consulting foundation, with a course catalog and a free-consultation booking form that creates real Google Calendar events and sends confirmation emails.

`Next.js 14` `TypeScript` `Tailwind CSS` `Framer Motion` `Google Calendar API`
</details>

---

### 📌 Other projects

| Project | What it is |
|---|---|
| [**steeven781.github.io**](https://github.com/steeven781/steeven781.github.io) | My personal portfolio site |
| [**astro-cv-repo**](https://github.com/steeven781/astro-cv-repo) | Interactive CV/resume built with Astro |
| [**price-calculator**](https://github.com/steeven781/price-calculator) | Pricing & installment calculator for Guatemalan retail — USD→GTQ, margin presets, 12% VAT, bank-fee plans, PDF export, WhatsApp quote sharing |
| **OpenQase** | Open-source (MIT), self-hosted, multi-tenant test case management — an open alternative to spreadsheets for QA teams |
| **ux-sentinel** | A Claude Skill that audits and designs UX against named standards (ISO 9241-110, UXQB CPUX-F), with evidence-based, regression-aware findings |

### 📈 By the Numbers

<p align="center">

**20** projects &nbsp;·&nbsp; **4** in production with real users &nbsp;·&nbsp; **2,000+** combined commits &nbsp;·&nbsp; **700+** test files across core products

</p>

### 📊 GitHub Stats

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=steeven781&theme=tokyonight&hide_border=true&v=2" />
</p>

---

<p align="center"><i>📫 Reach me via my portfolio site above</i></p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a8a,100:0f172a&height=120&section=footer&v=2" width="100%"/>
