### Hi, I'm Igor 👋

**Senior full-stack engineer and tech lead.** I build serverless systems on AWS, from the data model to the offline-first frontend. I have been shipping production software since 2017.

Most of my work lives in private organization repos, so this page sums it up.

---

#### 🛠️ What I work with

**Backend**
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Quarkus](https://img.shields.io/badge/Quarkus-4695EB?style=flat-square&logo=quarkus&logoColor=white)
![GraalVM](https://img.shields.io/badge/GraalVM_native-F29111?style=flat-square&logo=oracle&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)

**AWS & data**
![Lambda](https://img.shields.io/badge/Lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white)
![AppSync](https://img.shields.io/badge/AppSync-FF4F8B?style=flat-square&logo=amazonaws&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=flat-square&logo=amazondynamodb&logoColor=white)
![Aurora](https://img.shields.io/badge/Aurora_PostgreSQL-527FFF?style=flat-square&logo=amazonrds&logoColor=white)
![Athena](https://img.shields.io/badge/Athena-8C4FFF?style=flat-square&logo=amazonaws&logoColor=white)
![Iceberg](https://img.shields.io/badge/Apache_Iceberg-4E8EE9?style=flat-square&logo=apache&logoColor=white)
![Step Functions](https://img.shields.io/badge/Step_Functions-E7157B?style=flat-square&logo=amazonaws&logoColor=white)
![CloudFormation](https://img.shields.io/badge/CloudFormation_/_SAM-FF4F8B?style=flat-square&logo=amazonaws&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)

**Frontend**
![Vue](https://img.shields.io/badge/Vue_3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![Quasar](https://img.shields.io/badge/Quasar-1976D2?style=flat-square&logo=quasar&logoColor=white)
![Vuetify](https://img.shields.io/badge/Vuetify-1867C0?style=flat-square&logo=vuetify&logoColor=white)
![PWA](https://img.shields.io/badge/PWA_offline--first-5A0FC8?style=flat-square&logo=pwa&logoColor=white)
![Pinia](https://img.shields.io/badge/Pinia-FFD859?style=flat-square&logo=pinia&logoColor=black)

**Quality & AI tooling**
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![MCP](https://img.shields.io/badge/MCP_servers-000000?style=flat-square&logo=anthropic&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code_plugins-D97757?style=flat-square&logo=claude&logoColor=white)

---

#### 🚀 Things I've built

- **A GraphQL API with about 470 operations** on AppSync and Kotlin/Quarkus Lambdas. It uses single-table DynamoDB plus Aurora PostgreSQL, and its infrastructure is split into 14 per-domain CloudFormation nested stacks. I wrote about 77% of its commits.
- **A greenfield backend compiled to a GraalVM native image** on Lambda. It has AppSync with dual Cognito + IAM auth, real-time subscriptions pushed through SigV4, and a DynamoDB Streams → S3 → Athena analytics pipeline. I was its backend architect and wrote most of its commits.
- **An S3 cost fix based on measurement.** I traced the bill to Athena polling over tens of thousands of small JSON files, replaced it with a GSI change feed, and moved the stream data to Apache Iceberg via Firehose. Weekday S3 GET requests dropped by about 55%.
- **The offline-first layer of a field PWA.** It has an outbox queue with a poison guard, durable incremental sync and IndexedDB storage. In a Playwright test with the network cut, it rendered about 1,000 tasks.
- **A Python jobs and ETL worker.** Step Functions and EventBridge orchestrate a job-router Lambda that writes PDF and Excel reports and runs Athena queries.
- **Algorithms.** Banded Levenshtein with a q-gram index for fuzzy catalog matching, and a calibrated TF-IDF + SVM text classifier.

#### 🧭 How I work

- **I measure before I optimize.** Cost and performance changes start from data, not guesses.
- **I write the spec before the code.** Design docs, ADRs and runbooks for migrations and cutovers.
- **I test what matters.** Playwright with the network off, golden tests for reports, unit tests on the core logic.
- **I migrate without downtime.** Census of the data, then dual-write or backfill, then verification, with a rollback plan ready.

---

<details>
<summary>🇧🇷 Em português</summary>

**Desenvolvedor full-stack sênior e tech lead.** Construo sistemas serverless na AWS, do modelo de dados ao frontend offline-first, e coloco software em produção desde 2017.

- API GraphQL com cerca de 470 operações (AppSync + Kotlin/Quarkus em Lambda) e infraestrutura em 14 nested stacks CloudFormation.
- Backend compilado como GraalVM native image, do qual fui o arquiteto e escrevi a maior parte dos commits.
- Correção do custo de S3: troquei polling por change-feed e migrei para Apache Iceberg. Os GETs em dias úteis caíram cerca de 55%.
- Camada offline-first de PWA com outbox, sync incremental e IndexedDB.

</details>

📫 **igordoico@gmail.com** · Porto Alegre, Brazil
