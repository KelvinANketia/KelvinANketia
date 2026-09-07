<h1 align="center">Kelvin Amankwah Nketia</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=6A5ACD&center=true&vCenter=true&width=520&lines=Full+Stack+Engineer;Django+%2B+DRF+%7C+Node+%2B+Express;React+%2B+TypeScript;Security-minded+delivery" alt="Full Stack Engineer" />
</p>

<div align="center">
  <a href="mailto:kelvinkwabenanketia@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://github.com/KelvinANketia">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <!-- Add LinkedIn here — recruiters look for it first -->
</div>

<br/>

## About

Full stack engineer in Accra, Ghana. I build line-of-business systems end to end — Django/DRF and Node/Express services, React and TypeScript front ends, and the Docker, CI and test tooling that keeps them shippable.

Most of my work is in private client and employer repositories, so this page describes the systems rather than linking to source. Across the last two years that's **~3,000 commits over 33 repositories**: an inventory management system I built single-handed for a national research institute, and an enterprise HR platform where I'm the leading contributor on both the API and the front end.

I care about the parts that show up after launch — migrations that can be rolled back, audit trails that hold up, dependencies pinned for a reason, and tests that catch the regression before the client does.

<br/>

## Selected Work

### CSIR Stores — Inventory Management System
**Sole engineer · 613 commits · Express 5 · MongoDB · Redis**

An inventory and requisition platform for the Stores department of the CSIR, Ghana's Council for Scientific and Industrial Research. It covers requisitions and approvals, stock checkouts, goods-received notes, supplier and invoice handling, non-conformance reporting, and departmental reporting — served to two distinct portals over one API.

I designed and built all of it: 24 data models, 22 API route modules, and 23 services. Authentication runs on WebAuthn passkeys and TOTP two-factor over HttpOnly sessions with CSRF protection. Uploads are virus-scanned through ClamAV, requests are rate-limited in Redis, and every mutation writes to a tamper-evident audit chain. The front end is a vanilla-JS progressive web app with offline support and no build step, which keeps deployment trivial on constrained infrastructure.

Behind the API: idempotency middleware, request coalescing, tiered caching, query deduplication and profiling, and server-sent events for live updates. Schema changes ship as 16 numbered migrations, each with a dry-run and a rollback path. Quality is enforced by 31 test suites, Playwright end-to-end runs with axe accessibility checks, a coverage floor in CI, gitleaks secret scanning, and documented OWASP ZAP penetration scans.

### GSL Human Resource Management Platform
**Lead contributor, both repositories · 991 commits · Django 6 · DRF · React · TypeScript**

An enterprise HR platform for the Ghana School of Law's CLET programme, built by a team of eleven. I'm the top committer on both halves — 479 of the backend's commits and 512 of the front end's.

The API is Django 6 and Django REST Framework over PostgreSQL, with Celery and celery-beat for scheduled work and a Kafka producer driven by an outbox pattern for reliable event publishing. It spans 27 domain applications including payroll, recruitment and applicant tracking, interviews, attendance, leave, performance, learning, compliance and audit. Payslips, contracts and org-chart exports render through WeasyPrint and ReportLab; payroll and analytics export to XLSX via openpyxl.

The front end is a Turborepo and pnpm monorepo — two applications over nine shared internal packages for UI, auth, the API client, hooks and types. React and TypeScript on Vite, with TanStack Query for server state, Zustand for client state, react-hook-form and Zod for validation, and Tailwind for styling.

Both repositories run SonarQube and Trivy image scanning in CI, with Ruff and pytest on the API, Vitest, Testing Library and Playwright on the front end, and Husky, lint-staged and commitlint on the way in. Dependencies are pinned with the reasoning written inline — a Django floor that excludes a QuerySet SQL-injection advisory, a Pillow floor that excludes a decompression-bomb fix.

### IAM 3.0 and the CLET Service Estate
**Core contributor · 75 commits · Django · Celery**

The central identity and access management service for an estate of roughly 100 repositories, where I'm the third of twelve contributors. Alongside it I've worked across the surrounding services — communications, payments, API integration and the Kubernetes platform tooling — which is where I've learned how systems behave once they're distributed across teams rather than owned by one.

<br/>

## Tech Stack

**Languages**
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" />
</p>

**Backend**
<p>
  <img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/DRF-A30000?style=for-the-badge&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white" />
</p>

**Front end**
<p>
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwind-css&logoColor=white" />
  <img src="https://img.shields.io/badge/TanStack_Query-FF4154?style=for-the-badge&logo=reactquery&logoColor=white" />
  <img src="https://img.shields.io/badge/Zod-3E67B1?style=for-the-badge&logo=zod&logoColor=white" />
  <img src="https://img.shields.io/badge/Turborepo-EF4444?style=for-the-badge&logo=turborepo&logoColor=white" />
</p>

**Data & messaging**
<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white" />
</p>

**Infrastructure & quality**
<p>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/SonarQube-4E9BCD?style=for-the-badge&logo=sonarqube&logoColor=white" />
</p>

<br/>

## GitHub Stats

<div align="center">
  <img src="https://streak-stats.demolab.com?user=KelvinANketia&theme=radical&hide_border=true" alt="GitHub Streak" />
</div>

<br/>

## How I Work

```javascript
const kelvin = {
  backend:      ['Django', 'DRF', 'Express', 'Celery', 'Kafka'],
  frontend:     ['React', 'TypeScript', 'Vite', 'Tailwind', 'TanStack Query'],
  data:         ['PostgreSQL', 'MongoDB', 'Redis', 'S3'],
  platform:     ['Docker', 'Kubernetes', 'GitHub Actions', 'Nginx'],
  architecture: ['REST', 'event-driven via outbox', 'monorepo', 'RBAC'],
  currentFocus: 'Systems that stay maintainable after the launch sprint',
  funFact:      'I debug with console.log() and prayer — both equally effective'
};
```

- **Reversible changes.** Migrations ship with dry-run and rollback paths, so a bad deploy is an inconvenience rather than an incident.
- **Security as routine, not a phase.** Passkeys and 2FA, secret scanning in pre-commit, image scanning in CI, and dependency pins that cite the advisory they exclude.
- **Tests that earn their keep.** Unit and integration coverage behind a CI floor, plus end-to-end runs with accessibility assertions.
- **Accessible and fast by default.** Axe checks in the pipeline, and offline-capable front ends for users on unreliable connections.

<br/>

<details>
  <summary><b>✝️ Faith Corner</b></summary>
  <br/>
  <blockquote>
    "For I know the plans I have for you," declares the LORD, "plans to prosper you and not to harm you, plans to give you hope and a future." — Jeremiah 29:11
  </blockquote>
  <p>Alongside engineering I teach the Bible, and I care about sharing what I learn — in both directions.</p>
</details>

<br/>

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=KelvinANketia&label=Profile%20views&color=6A5ACD&style=flat" alt="Profile Views" />
</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer&fontSize=90" alt="" />
</div>
