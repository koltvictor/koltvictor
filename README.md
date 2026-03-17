# Hi, I'm Kolt
I design and build software. Not one or the other — both.
Principal Software Consultant based in NYC. I either build products solo end-to-end, or architect solutions and lead engineering teams through delivery.
## Recent Work
**[Kolt's Table](https://koltstable.com)** — A seasonal, plant-forward cooking platform designed and built solo.
<br/>
[![Frontend CI/CD Pipeline](https://github.com/koltvictor/kolts-table/actions/workflows/frontend_ci_cd.yml/badge.svg)](https://github.com/koltvictor/kolts-table/actions/workflows/frontend_ci_cd.yml)
[![Backend CI/CD Pipeline](https://github.com/koltvictor/kolts-table/actions/workflows/backend_ci_cd.yml/badge.svg)](https://github.com/koltvictor/kolts-table/actions/workflows/backend_ci_cd.yml)

**AI features powered by Anthropic Claude:**
- **The Pantry** — enter what's in your kitchen, Claude semantically normalizes and expands your ingredients, matches against the full recipe database, and returns ranked results with match percentage, matched ingredients, missing ingredients, match explanation, and a generated shopping list
- **Natural language recipe search** — conversational queries ("something warming and quick for a weeknight") are interpreted by Claude and translated into structured filters in real time

**Platform:**
- 180KB production bundle (53% smaller than NYT Cooking)
- Sub-50ms recipe search via PostgreSQL GIN indexes
- 94/100 Lighthouse performance score
- 60+ normalized PostgreSQL tables, zero technical debt
- Full CI/CD pipeline — Docker, GitHub Actions, zero-downtime deploys
- New Relic APM, Redis caching, Elasticsearch, Kibana

**[env-doctor](https://www.npmjs.com/package/@koltvictor/env-doctor)** — Zero-dependency CLI that diagnoses environment variable issues in any Node.js project.
<br/>
[![npm](https://img.shields.io/npm/v/@koltvictor/env-doctor?color=cb3837&logo=npm)](https://www.npmjs.com/package/@koltvictor/env-doctor)
- Scans source code for `process.env` usage
- Compares against `.env.example` — surfaces missing, undocumented, and unused vars
- Exit code `1` on issues, making it CI-pipeline friendly

## Tech Stack
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![ElasticSearch](https://img.shields.io/badge/-ElasticSearch-005571?style=for-the-badge&logo=elasticsearch)
![Kibana](https://img.shields.io/badge/kibana-%23005571.svg?style=for-the-badge&logo=kibana&logoColor=white)
![New Relic](https://img.shields.io/badge/New%20Relic-1CE783?style=for-the-badge&logo=newrelic&logoColor=white)
![Anthropic](https://img.shields.io/badge/Anthropic%20Claude-D97706?style=for-the-badge&logo=anthropic&logoColor=white)

## Get In Touch
- Portfolio: [koltadams.com](https://koltadams.com)
- Email: kolt@koltadams.com
- LinkedIn: [linkedin.com/in/koltadams](https://linkedin.com/in/koltadams)
