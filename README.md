<div align="center">

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&pause=1000&color=6E56CF&center=true&vCenter=true&width=600&lines=Full-stack+engineer;Backend+%2B+Frontend+%2B+Mobile+%2B+AI;I+fix+the+pattern%2C+not+just+the+bug" alt="Typing SVG" />
</a>

</div>

# Hi, I'm Kiwaalabye Ggayi Germaine 👋

Software Engineer, entrepreneur & Product Architect engineer who works across backend architecture, frontend, mobile, and applied AI. Particular focus on systems that touch money, identity, and state transitions correctly the first time.

<br>

## What I Work On

I build full-stack platforms end-to-end: relational data models, API layers, frontend clients, native mobile apps, and the domain logic that ties them together. Think multi-tenant systems, multi-currency transactions, ticketing/inventory-style state machines, and role-based access.

## Languages & Runtimes

<div align="left">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
<img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" />
<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" />
</div>

- **TypeScript / JavaScript**: primary language for backend and frontend work
- **Kotlin**: native Android development
- **Java**: backend domain/finance logic
- **Python**: microservices, tooling, automation
- **SQL**: relational schema design and query optimization

## Backend

<div align="left">
<img src="https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white" />
<img src="https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white" />
<img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
</div>

- **NestJS**: modular service architecture, dependency injection, guards/interceptors
- **Prisma**: schema modeling, migrations, type-safe data access
- **PostgreSQL**: relational design, indexing, transactional integrity
- **GraphQL & REST**: API design across both paradigms, including schema tradeoffs
- **Flyway**: versioned database migrations
- **BullMQ / Redis**: background job processing, caching, queues

## Frontend

<div align="left">
<img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
<img src="https://img.shields.io/badge/Zustand-433E38?style=for-the-badge&logo=react&logoColor=white" />
<img src="https://img.shields.io/badge/Zod-3E67B1?style=for-the-badge&logo=zod&logoColor=white" />
</div>

- **React**: component architecture, state modeling
- **Zustand**: lightweight global state management
- **SWR**: data fetching, caching, revalidation
- **Zod**: runtime schema validation
- Discriminated-union patterns for representing async/loading/error state cleanly rather than relying on ad hoc booleans

## Mobile

<div align="left">
<img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" />
<img src="https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white" />
<img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" />
</div>

- **Kotlin + Jetpack Compose**: native Android UI
- **Mavericks**: MVI-style state management for Android

## AI / LLM Integration

<div align="left">
<img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" />
</div>

- Local LLM serving via **Ollama** running quantized models (GGUF, CPU-only inference)
- Designing gateway-style services that centralize LLM access behind a single point rather than scattering calls across a codebase
- Role-scoped retrieval design, making sure different consumers of an AI layer only see what they're authorized to see.

<br>

## Finance-Adjacent Systems

- Java-based domain logic for financial calculations
- Payment state machine design: separating UX-layer pre-checks from authoritative backend enforcement
- Planning integrations with real payment providers rather than relying on dev-phase shortcuts

<br>

## Systems Thinking & Engineering Principles

I care a lot about *how* systems fail, not just whether they work in the demo. Some principles I actively design around:

- **Never trust unverified identifiers across boundaries.** Headers, guessed IDs, and fallback values don't count as identity. Always resolve from an authoritative source.
- **One resolution point per shared resource.** When multiple parts of a system need the same data (roles, media, location, pricing), they should all go through a single normalization function. No component should reimplement its own guess at the shape.
- **UI implying a rule ≠ the rule being enforced.** I actively look for state transitions that *look* gated in the interface but have no backend enforcement behind them.
- **Confidence-tagging over silent guessing.** When data quality varies (estimated vs. verified vs. missing), I prefer explicit confidence levels over quietly treating everything as equally reliable.
- **Instrumentation before feature flags.** Metrics get wired for real, and an observation window has to actually pass, before I'll ship a flag-flip or removal.
- **Evidence over assertion.** A plan or summary describing what code does isn't the same as having read the code. I don't sign off on either without actual file contents, diffs, or grep output.
- **Premature abstraction is a cost, not a virtue.** I don't generalize a pattern until there's a second real call site that needs it.

<br>

## How I Work

- I write things down before I build them: architecture plans with real file/line references, not just prose intentions.
- I track known gaps and dev-phase shortcuts explicitly rather than letting them blend into "done."
- I prefer staged rollouts with real observation windows over single-pass, all-at-once changes.
- I actively watch for the same *class* of bug reappearing in new places (e.g., a boundary-resolution problem showing up in role handling, then media, then geocoding) and fix the pattern, not just the instance.

---

<div align="center">
<sub>This README reflects tools and practices I use day to day, always evolving as the work does.</sub>
</div>
