<h1 align="center">Hi, I'm Steeven Medina 👋</h1>
<p align="center">Senior QA Engineer &amp; Automation Architect — building full-stack SaaS products on the side 🇬🇹</p>

<p align="center">
  <a href="https://steevencodeqa.netlify.app"><img src="https://img.shields.io/badge/Portfolio-steevencodeqa.netlify.app-black?style=flat-square&logo=netlify" /></a>
  <a href="https://www.linkedin.com/in/steevenm7/"><img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat-square&logo=linkedin" /></a>
</p>

---

### 🚀 Currently

Building **Numia** — a business intelligence SaaS for SMEs that connects to their existing databases and delivers AI-powered insights straight to WhatsApp. Handling product and architecture end to end, from data pipeline to the analysis layer.

### 🛠️ Tech I work with

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
</p>

---

### 🏗️ Systems I've Built

Products I designed, built, and shipped with full ownership — from problem definition to production.

<details>
<summary><b>Numia</b> — BI SaaS for SMEs &nbsp;·&nbsp; <i>Side Project · In Development · 2026</i></summary>
<br>

**Problem**
SMEs running their operations on Aspel SAE accumulate years of transactional data but have no real-time visibility into overdue collections, dead inventory, or margin leaks — the insight exists but nobody has time to query it.

**Contribution**
Architecting and building the platform solo: a SQL Server connector, a pandas-based analysis engine (prioritized collections, dead inventory detection, price leak identification), an AI layer on the Claude API for daily summaries and deep analysis, a FastAPI backend, and a React dashboard — plus the full go-to-market and pricing model.

**Impact**
Designed so a distribution partner can show a business owner their own live data value within one hour — the core of the sales motion — and automates a daily 7am executive WhatsApp summary in place of manual reporting.

`Python` `FastAPI` `pyodbc` `pandas` `SQL Server` `Claude API` `React`

*Founder &amp; Solo Developer — end-to-end ownership*
</details>

<details>
<summary><b>Integrity</b> — Multi-tenant Condo Management SaaS &nbsp;·&nbsp; <i>Production · 2026</i></summary>
<br>

*An expanded, multi-tenant evolution of an earlier product (Nexus Admin) — grown from a single condominium's tracking site into a SaaS serving multiple independent communities.*

**Problem**
Residential communities managed payments, access control, maintenance reports, and resident data through spreadsheets and manual phone coordination — no audit trail, no self-service, and no way to onboard a new community without rebuilding the whole setup.

**Contribution**
Designed and built a multi-tenant platform with modular, per-tenant feature flags (new modules ship off by default and are enabled per community); public intake forms for maintenance reports and service evaluations (reCAPTCHA-protected, no login required); a resident self-service portal (OTP login) for identity, vehicles, and pets; and a full admin panel with role-based access control and a tenant switcher. Backed by Supabase (Postgres/Auth/Storage), Cloudflare R2 for file storage with automated reference-checked cleanup, and Upstash Redis.

**Impact**
Replaced spreadsheet-based billing and phone-based coordination with a fully auditable system live across multiple independent communities, with a modular architecture that lets new features roll out to one tenant without touching the rest.

`Next.js` `TypeScript` `Supabase` `Cloudflare R2` `Upstash Redis` `Vitest`

*Full-Stack Architect &amp; Engineer — end-to-end ownership*
</details>

---

### 🧪 Testing &amp; Automation Architecture

<details>
<summary><b>Contract-First API + UI Test Framework</b> &nbsp;·&nbsp; <i>Work Project · 2025</i></summary>
<br>

*Built for a client engagement — described here at the architecture level; product and client details withheld for confidentiality.*

**Problem**
Manual regression testing across a fast-evolving REST API and its web front end was slow to run and consistently drifted out of sync with the real API contract as endpoints changed.

**Contribution**
Designed a Playwright test architecture where typed API clients and spec scaffolds are generated directly from the OpenAPI/Swagger contract, so a new endpoint is one regeneration away from coverage. Added a page-object layer for the UI suite with a shared, cloud-stored authenticated session (so tests never re-login), multi-environment configuration (dev/staging/prod), and tagged smoke/regression suites wired into CI with Allure reporting.

**Impact**
Kept the test suite automatically aligned with a changing API contract, cut manual regression effort, and gave the team a one-command smoke check plus a full regression pass — reducing the risk of untested endpoints slipping into production.

`Playwright` `TypeScript` `OpenAPI/Swagger codegen` `AWS Secrets Manager` `Allure`

*Test Automation Architect*
</details>

<details>
<summary><b>TestMan</b> &nbsp;·&nbsp; <i>[status] · [year]</i></summary>
<br>

**Problem**
_[Add: what was manual, broken, or missing before this existed]_

**Contribution**
_[Add: what you built and your role]_

**Impact**
_[Add: the measurable result]_

`[tech]` `[tech]` `[tech]`
</details>

---

### 💼 Client Work

<details>
<summary><b>Música y Audio Soluciones</b> — E-commerce landing &amp; catalog &nbsp;·&nbsp; <i>Guatemala</i></summary>
<br>

Landing page and product catalog for a music and pro-audio retailer. No backend — the catalog is fetched live from a Google Sheets API (Apps Script), with category/brand filtering, a deals carousel, and a WhatsApp-based purchase flow instead of a checkout.

`Webpack 5` `Tailwind CSS v4` `Alpine.js` `ApexCharts`
</details>

<details>
<summary><b>FFCI Guatemala</b> — Marketing &amp; booking site &nbsp;·&nbsp; <i>Guatemala</i></summary>
<br>

Site for a leadership training and consulting foundation, with a course catalog, purchase-request flow, and a free-consultation booking form that creates real Google Calendar events (service-account auth) and sends confirmation emails.

`Next.js 14` `TypeScript` `Tailwind CSS` `Framer Motion` `Google Calendar API`
</details>

---

### 📌 Other projects

| Project | What it is |
|---|---|
| [**steeven781.github.io**](https://github.com/steeven781/steeven781.github.io) | My personal portfolio site |
| [**astro-cv-repo**](https://github.com/steeven781/astro-cv-repo) | Interactive CV/resume built with Astro |
| [**price-calculator**](https://github.com/steeven781/price-calculator) | [Add a 1-line description: what does it calculate, who's it for] |
| [**fel**](https://github.com/steeven781/fel) | [Add a 1-line description of what this project does] |
| **Andares Activities Tracking** | Original single-condo activity tracker — evolved into Integrity |

### 📊 GitHub stats

<p>
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=steeven781&show_icons=true&theme=tokyonight&hide_border=true" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=steeven781&layout=compact&theme=tokyonight&hide_border=true" />
</p>
<p>
  <img src="https://streak-stats.demolab.com/?user=steeven781&theme=tokyonight&hide_border=true" />
</p>

---

<p align="center"><i>📫 Reach me via my portfolio site above</i></p>
