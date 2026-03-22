cat > /mnt/user-data/outputs/github-profile-readme.md << 'ENDOFREADME'
# Hi, I'm Kolt
I design and build software. Not one or the other — both.
Fractional CTO & Product Engineer based in NYC. I either build products solo end-to-end, or architect solutions and lead engineering teams through delivery.
## Recent Work
**[Kolt's Table](https://koltstable.com)** — A seasonal, plant-forward cooking platform designed and built solo. 1,450+ commits.
<br/>
[![Frontend CI/CD Pipeline](https://github.com/koltvictor/kolts-table/actions/workflows/frontend_ci_cd.yml/badge.svg)](https://github.com/koltvictor/kolts-table/actions/workflows/frontend_ci_cd.yml)
[![Backend CI/CD Pipeline](https://github.com/koltvictor/kolts-table/actions/workflows/backend_ci_cd.yml/badge.svg)](https://github.com/koltvictor/kolts-table/actions/workflows/backend_ci_cd.yml)

**AI — user-facing features (Anthropic Claude):**
- **The Pantry** — enter what's in your kitchen, Claude semantically normalizes and expands your ingredients, matches against the full recipe database, and returns ranked results with match percentage, match explanations, and a generated shopping list. Interactive homepage teaser drives traffic directly into the feature.
- **Natural language recipe search** — conversational queries ("something warming and quick for a weeknight") interpreted by Claude and translated into structured filters in real time
- **Ingredient-aware search with synonym expansion** — searches actual recipe ingredients, not just titles/descriptions. Synonym groups (spring onion = scallion = green onion, cilantro = coriander, + 10 more) ensure comprehensive results

**Seasonal Intelligence Engine:**
- Site-wide seasonal data config drives homepage, navigation, produce guides, and founder's note — all rotate automatically by month, zero manual updates
- "What's in Season" living reference page with interactive season tabs, clickable produce grid, and filtered recipe display
- Homepage redesign: seasonal hero, produce strip, curated recipes, editorial journal feature — 6 intentional sections, no redundancy

**AI — Platform Intelligence (20 autonomous jobs):**
- Auto-featuring algorithm driven by Engagement Quality Score — ratings, analytics, favorites, and seasonal context with governance rules and one-click revert
- Anonymous engagement analytics pipeline (zero PII) — time on page, scroll depth, view counts
- Claude-drafted newsletters with editorial review panel, weekly digests, and daily summaries
- Content analysis — recipe description polish, meta description optimization, internal linking suggestions
- Content and pantry gap analysis — identifies missing recipes based on seasonal produce and site data
- SEO audit — scans all content for title length, description quality, images, tags, duplicates
- Codebase health scanner — dependency audit, security vulnerabilities, code quality metrics, database health
- Trending detection, draft monitoring, and image generation via Google Gemini
- Cron scheduler with live sync — toggle any job from the admin dashboard, no restart needed

**AI — SEO Intelligence (three-stage pipeline):**
- Automated audit: title length, description quality, images, tags, duplicates
- Claude proposes editorial fixes matching brand voice
- Approval queue with side-by-side comparison, one-click apply to database

**Governance & Approval System:**
- Centralized review queue for all AI-proposed changes
- Side-by-side current vs proposed comparison
- Apply writes to database only after human approval, full audit trail
- Newsletter, SEO fixes, and description rewrites all flow through the same queue

**AI — Recipe Entry (two-stage):**
- Paste raw recipe text → Sonnet parses ingredients/instructions in ~2s → Opus classifies across 100+ filter categories
- Strict classification rules: only selects what's true as written, never speculative

**Platform:**
- 180KB production bundle (53% smaller than NYT Cooking)
- Sub-50ms recipe search via PostgreSQL GIN indexes
- 96/100 Lighthouse performance scores across all metrics
- 44 normalized PostgreSQL tables, zero technical debt
- User dashboard with engagement stats, searchable favorites, dietary preferences
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
![Google Gemini](https://img.shields.io/badge/Google%20Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)

## Get In Touch
- Portfolio: [koltadams.com](https://koltadams.com)
- Email: kolt@koltadams.com
- LinkedIn: [linkedin.com/in/koltadams](https://linkedin.com/in/koltadams)
ENDOFREADME
echo "✅ done"
