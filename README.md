<h1 align="center">Apofis391</h1>

<p align="center">
  <b>Computer Science Engineer · Full Stack Developer</b><br>
  <sub>Universidad UTE · Pichincha, Ecuador</sub>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com/?font=Inter&weight=500&size=18&duration=2800&pause=1200&color=86868B&center=true&vCenter=true&width=560&lines=Business+systems%2C+end+to+end.;Java+%C2%B7+Python+%C2%B7+PHP+%C2%B7+TypeScript;Servers%2C+deployment+and+self-hosted+AI.;Automating+the+boring+parts." alt="Business systems, end to end. Java, Python, PHP, TypeScript. Servers, deployment and self-hosted AI.">
</p>

<table align="center">
  <tr>
    <td align="center" width="140"><h3>6</h3><sub>systems built</sub></td>
    <td align="center" width="140"><h3>6</h3><sub>languages</sub></td>
    <td align="center" width="140"><h3>4</h3><sub>database engines</sub></td>
    <td align="center" width="140"><h3>102</h3><sub>automated tests<br>in one project</sub></td>
  </tr>
</table>

<br>

### About

Computer Science Engineer graduated from Universidad UTE, working as a full stack developer.
I design and deliver complete systems for real organizations — finance, education, human resources, retail and hospitality — covering the database, backend, frontend, server and deployment.
I also run my own infrastructure: Windows Server 2022 on Hetzner and a self‑hosted AI service published through Cloudflare.

**What I bring to a project**

| | |
|:--|:--|
| **Full stack delivery** | From the database schema to the screen the user clicks |
| **Data integrity** | Transactions, audit trails and double‑entry accounting where money is involved |
| **Security by default** | Role‑based access, encrypted fields, strict security headers, no secrets in code |
| **Quality** | Automated tests against the real database, static analysis and CI on every push |
| **Operations** | Servers, reverse proxies, tunnels, Docker and production checklists |

<br>

### Stack

| | |
|:--|:--|
| **Languages** | <picture><source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=java,python,php,js,ts,cs&theme=dark"><img src="https://skillicons.dev/icons?i=java,python,php,js,ts,cs&theme=light" height="36" alt="Java, Python, PHP, JavaScript, TypeScript, C#"></picture> |
| **Backend** | <picture><source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=spring,django,laravel,nodejs&theme=dark"><img src="https://skillicons.dev/icons?i=spring,django,laravel,nodejs&theme=light" height="36" alt="Spring Boot, Django, Laravel, Node.js"></picture> |
| **Frontend** | <picture><source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=angular,react,vue,vite,tailwind,html,css&theme=dark"><img src="https://skillicons.dev/icons?i=angular,react,vue,vite,tailwind,html,css&theme=light" height="36" alt="Angular, React, Vue, Vite, Tailwind CSS, HTML, CSS"></picture> |
| **Databases** | <picture><source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=mysql,postgres,sqlite,redis&theme=dark"><img src="https://skillicons.dev/icons?i=mysql,postgres,sqlite,redis&theme=light" height="36" alt="MySQL, PostgreSQL, SQLite, Redis"></picture> &nbsp;+ SQL Server (T‑SQL) |
| **Infrastructure** | <picture><source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=windows,linux,docker,nginx,cloudflare&theme=dark"><img src="https://skillicons.dev/icons?i=windows,linux,docker,nginx,cloudflare&theme=light" height="36" alt="Windows Server, Linux, Docker, Nginx, Cloudflare"></picture> &nbsp;+ Hetzner · Windows Server 2022 |
| **AI** | Ollama · DeepSeek (self‑hosted LLM) |
| **Tools** | <picture><source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=git,github,githubactions,powershell,vscode,idea&theme=dark"><img src="https://skillicons.dev/icons?i=git,github,githubactions,powershell,vscode,idea&theme=light" height="36" alt="Git, GitHub, GitHub Actions, PowerShell, VS Code, IntelliJ IDEA"></picture> |

<br>

### Featured Projects

<sub>Click <b>Architecture</b> under each project to see how it is built.</sub>

---

#### FINTEC — Credit union core system
Manages members, savings, contributions, loans, transactions, accounting, audit and reports.

![Java](https://img.shields.io/badge/Java_25-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3.4-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![Angular](https://img.shields.io/badge/Angular_21-DD0031?style=flat-square&logo=angular&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white)

- **Money is never edited directly.** Every movement creates a transaction, a journal entry (debit = credit) and an audit record. Errors are fixed with reversals, never deletes.
- **Exact amounts.** No floating‑point numbers in financial calculations.
- **Loans** with German amortization, guarantor rules, PDF application and an approval workflow.
- **12 backend modules · 18 database schemas**, versioned migrations, BCrypt passwords, bulk user import from Excel and automatic logout after 15 minutes of inactivity.

<details>
<summary><b>Architecture</b></summary>
<br>

```mermaid
flowchart LR
  U([Member · Staff]) --> A[Angular 21]
  A -->|REST API| B[Spring Boot 3.4]
  B --> T{{Financial transaction}}
  T --> M[Movement]
  T --> J[Journal entry<br/>debit = credit]
  T --> L[Audit log]
  B --> D[(SQL Server<br/>18 schemas)]
```

</details>

---

#### mi_rrhh — Human resources platform
Employee records, self‑service, vacations and absences, processes, hiring and a control dashboard for an educational institute.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django_5.2-092E20?style=flat-square&logo=django&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Bulma](https://img.shields.io/badge/Bulma-00D1B2?style=flat-square&logo=bulma&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chartdotjs&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

- **11 modules:** accounts, credentials, employees, vacations, attendance, tasks, hiring, notifications, audit, dashboard and TIC teachers.
- **Security:** AES‑256‑GCM field encryption, strict Content Security Policy, protected file downloads, brute‑force protection and 8 roles with per‑object permissions.
- **Quality:** 102 automated tests against real SQL Server, CI with static analysis, coverage and dependency audit, and load tests with Locust.
- **Real time:** WebSocket notifications, web push and institutional email through Microsoft Graph.

<details>
<summary><b>Architecture</b></summary>
<br>

```mermaid
flowchart LR
  U([Employees · HR · Managers]) --> N[Nginx]
  N --> W[Waitress<br/>HTTP]
  N --> S[Daphne<br/>WebSocket]
  W --> DJ[Django 5.2<br/>11 apps]
  S --> DJ
  DJ --> H[(HR database<br/>SQL Server)]
  DJ -.read only.-> AT[(Attendance DB)]
  DJ -.read only.-> AC[(Academic DB)]
  DJ --> R[(Redis)]
  DJ --> G[Microsoft Graph<br/>email]
```

</details>

---

#### Intec Academic Platform
Role‑based academic system for an institute: separate dashboards for admin, students, teachers and sales; enrollment templates; teacher contracts.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django_5.2-092E20?style=flat-square&logo=django&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

- **Legacy integration:** logs users in against an existing SQL Server database without touching its tables.
- **Documents:** generates Excel enrollment templates and teacher contracts (DOCX → PDF).
- **Communication:** email with OAuth2 (Google, Microsoft, Yahoo) and web push notifications.
- **Data migration** scripts from SQL Server to PostgreSQL, and a Docker setup for development.

<details>
<summary><b>Architecture</b></summary>
<br>

```mermaid
flowchart LR
  U([Admin · Student · Teacher · Sales]) --> R[React + Vite]
  R --> DJ[Django]
  DJ -->|login by role| L[(Legacy SQL Server)]
  DJ --> S[(SQLite<br/>sessions)]
  DJ --> X[Excel templates]
  P[PHP module] --> C[Contracts<br/>DOCX → PDF]
  P --> E[Email OAuth2<br/>Web Push]
```

</details>

---

#### Self‑hosted AI service
Private, self‑hosted LLM API running DeepSeek with Ollama, published to the internet through Cloudflare.

![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![DeepSeek](https://img.shields.io/badge/DeepSeek-4D6BFE?style=flat-square&logo=deepseek&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare_Tunnel-F38020?style=flat-square&logo=cloudflare&logoColor=white)

<details>
<summary><b>Architecture</b></summary>
<br>

```mermaid
flowchart LR
  C([Client app]) -->|HTTPS| CF[Cloudflare Tunnel]
  CF --> O[Ollama API]
  O --> D[DeepSeek model]
```

</details>

---

#### HuecoUIO — Sales and inventory management
Business dashboard for products, inventory, clients, orders, sales, invoices with VAT and reports. Team project at Universidad UTE.

![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![Vue](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![Inertia](https://img.shields.io/badge/Inertia.js-9553E9?style=flat-square&logo=inertia&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![shadcn](https://img.shields.io/badge/shadcn%2Fui-000000?style=flat-square&logo=shadcnui&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

<details>
<summary><b>Business flow</b></summary>
<br>

```mermaid
flowchart LR
  P[Products] --> I[Inventory]
  I --> O[Orders]
  C[Clients] --> O
  O --> S[Sales]
  S --> F[Invoice + VAT]
  F --> R[Reports]
```

</details>

[View repository →](https://github.com/ElHuecoUTE/huecoUIO_LaravelApp)

---

#### Hotel Oasis — Hotel website and back office
Public site with services, promotions, reservations and contact, plus a staff area for reservations, rooms, income and expenses, inventory, cleaning, staff and marketing.

![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Composer](https://img.shields.io/badge/Composer-885630?style=flat-square&logo=composer&logoColor=white)

Built on a custom MVC structure: own router, controllers, views and reusable partials.

---

#### Open source

| Repository | What it does | Built with |
|:--|:--|:--|
| [automatizacion-whassap](https://github.com/Apofis391/automatizacion-whassap) | Sends a task checklist as a WhatsApp poll and keeps reminding until every task is checked | Node.js · whatsapp‑web.js |
| [Certificados](https://github.com/Apofis391/Certificados) | Splits bulk PDFs into one file per certificate, reads them with OCR and flags missing ones | Python |
| [Java-MDNE](https://github.com/Apofis391/Java-MDNE) | Data structures and algorithms: AVL and binary search trees, queues, hash tables, Prim, knapsack | Java |

#### In design

| Project | Goal | Planned stack |
|:--|:--|:--|
| Cybersecurity Lab | Practice security in safe, simulated labs with levels, progress tracking and automatic reports | Angular · Java · SQL · Docker |
| Security & Network Quotes | Build professional quotes for cameras and network equipment from a product catalog | Angular · TypeScript · Java · SQL |
| Tech Store | Online catalog and store for cameras, networking gear and electronic components | Angular · TypeScript · SQL |
| Smart City 3D | Interactive 3D city to visualize traffic, lighting, IoT devices and network infrastructure | JavaScript · 3D web |

#### Side project
Tank combat game for Fortnite Creative, scripted in Verse (UEFN).

<br>

### GitHub Activity

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./profile-summary-card-output/github_dark/3-stats.svg">
    <img src="./profile-summary-card-output/github/3-stats.svg" width="49%" alt="GitHub statistics">
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./profile-summary-card-output/github_dark/2-most-commit-language.svg">
    <img src="./profile-summary-card-output/github/2-most-commit-language.svg" width="49%" alt="Most used languages by commit">
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com/?user=Apofis391&hide_border=true&background=00000000&ring=2997FF&fire=2997FF&currStreakNum=F5F5F7&sideNums=F5F5F7&currStreakLabel=F5F5F7&sideLabels=86868B&dates=86868B&stroke=3A3A3C">
    <img src="https://streak-stats.demolab.com/?user=Apofis391&hide_border=true&background=00000000&ring=0071E3&fire=0071E3&currStreakNum=1D1D1F&sideNums=1D1D1F&currStreakLabel=1D1D1F&sideLabels=86868B&dates=86868B&stroke=D2D2D7" width="495" alt="GitHub contribution streak">
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Apofis391/Apofis391/output/github-snake-dark.svg">
    <img src="https://raw.githubusercontent.com/Apofis391/Apofis391/output/github-snake.svg" width="100%" alt="Contribution snake">
  </picture>
</p>

<br>

### Currently Learning

<p>
  <img src="https://img.shields.io/badge/Windows_Server_2022-0071E3?style=flat-square" alt="Windows Server 2022">
  <img src="https://img.shields.io/badge/Cloud_Servers-0071E3?style=flat-square&logo=hetzner&logoColor=white" alt="Cloud servers on Hetzner">
  <img src="https://img.shields.io/badge/Local_LLMs-0071E3?style=flat-square&logo=ollama&logoColor=white" alt="Local LLMs with Ollama">
  <img src="https://img.shields.io/badge/CI%2FCD-0071E3?style=flat-square&logo=githubactions&logoColor=white" alt="CI/CD">
  <img src="https://img.shields.io/badge/Cybersecurity-0071E3?style=flat-square&logo=letsencrypt&logoColor=white" alt="Cybersecurity">
</p>

<br>

### Learning Philosophy

> **Build to understand. Understand to solve.**
>
> I don't learn a technology by reading about it — I learn it by building something real with it.
> If I haven't built it, I can't truly solve it.

```mermaid
flowchart LR
  B[Build] --> T[Test] --> U[Understand] --> S[Solve] --> B
```

<br>

### Open Source & Collaboration

Open to collaborating on business systems, automation, self‑hosted AI and server infrastructure.
Issues, ideas and pull requests on my repositories are welcome.

[github.com/Apofis391](https://github.com/Apofis391)
