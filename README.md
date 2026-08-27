# Kolt Adams

I treat trust as an engineering problem.

Fractional CTO and product engineer, Las Vegas / New York. I build products solo end-to-end, or architect them and lead the team that ships them. Full case studies at [koltadams.com](https://koltadams.com) — this page is the engineer's cut.

| System | State | Evidence |
|---|---|---|
| [koltstable.com](https://koltstable.com) | live | 180 KB bundle · 96 Lighthouse · search <50 ms |
| Toren | private beta | 100 interactions · 41 substances · clinician-gated |
| [inklingapp.org](https://inklingapp.org) | TestFlight | 46/46 eval profiles · 0 personal data |
| [lopudmanagement.com](https://lopudmanagement.com) | live | static · 0 runtime dependencies |

*As of Aug 2026.*

---

### Kolt's Table — [koltstable.com](https://koltstable.com)

Seasonal cooking platform. Solo, six months, 1,500+ commits.
[![Frontend CI/CD](https://github.com/koltvictor/kolts-table/actions/workflows/frontend_ci_cd.yml/badge.svg)](https://github.com/koltvictor/kolts-table/actions/workflows/frontend_ci_cd.yml)
[![Backend CI/CD](https://github.com/koltvictor/kolts-table/actions/workflows/backend_ci_cd.yml/badge.svg)](https://github.com/koltvictor/kolts-table/actions/workflows/backend_ci_cd.yml)

- **The site rotates itself.** A seasonal config drives homepage, navigation, produce guides, and editorial by month. No manual updates.
- **20-job intelligence network, not 20 crons.** Jobs trigger and inform each other through a dependency graph with tracked causal links (SEO audit → description polish; trending detection → auto-feature). Content lifecycle uses 7d/30d engagement moving averages and linear-regression decay to predict unfeature dates.
- **Every AI write is gated.** All proposals land in one review queue with side-by-side diff, Levenshtein-based change-magnitude confidence scoring, and a full audit trail. Apply writes to the database only after human approval.
- **Two-stage recipe entry.** Sonnet parses raw text in ~2 s; Opus classifies across 100+ filters under strict only-what's-written rules.
- **Search.** Ingredient-aware with synonym groups, plus Claude-interpreted natural-language queries compiled to structured filters. Sub-50 ms via PostgreSQL GIN indexes.
- **Platform.** 180 KB production bundle (NYT Cooking ships 380). 60+ normalized tables. Docker + GitHub Actions zero-downtime deploys. Redis, Elasticsearch, New Relic.

React 19 · TypeScript · Node · PostgreSQL · Redis · Docker · Claude · Gemini

---

### Toren

Native iOS supplement and longevity tracker. Private beta.

- **Content is AI-drafted, clinician-gated, schema-enforced.** A database-level constraint makes it structurally impossible to publish a high-severity interaction warning backed only by preliminary evidence. The invariant lives in the migration, not in reviewer discretion.
- **100 published interaction records across 41 substances**, each reviewed by a licensed physician. Seven of 107 were retracted and the systematic errors behind them fixed at the source. Pharmacist completeness review gates public launch.
- **Nightly biometric ingestion** from Oura and Apple HealthKit, with per-source retention honoring each provider's data terms.
- **Evidence-graded** — every claim carries its evidence level, and the UI shows it.

SwiftUI · HealthKit · Node · PostgreSQL · Cloudflare Access · Claude

---

### Inkling — [inklingapp.org](https://inklingapp.org)

Mental-health screening orientation. Helps someone decide whether what they're feeling is worth a professional conversation. Never a diagnosis.

- **Two model stages.** Free-text routing to a validated screener (GAD-7, PHQ-9, PCL-5, others) or straight to crisis support; then plain-language, non-diagnostic reflection of results.
- **Eval-driven.** 46-profile classification suite at 100%, with a crisis-detection floor that held through every prompt revision and 42 out-of-scope guards against misrouting. Prompts that didn't clear the floor didn't ship.
- **Accountless, on-device, zero PII.** Crisis support one tap from every screen.

React Native · Expo · TypeScript · Cloudflare Workers · Claude

---

### Lopud Management — [lopudmanagement.com](https://lopudmanagement.com)

Client work under a hard identity-guideline brief. No framework, no analytics, no cookie banner. Static files, a Makefile, and a Playwright screenshot-diff verifier so a stylesheet change can't regress a page nobody looked at.

---

### env-doctor — [npm](https://www.npmjs.com/package/@koltvictor/env-doctor)

[![npm](https://img.shields.io/npm/v/@koltvictor/env-doctor?color=cb3837&logo=npm)](https://www.npmjs.com/package/@koltvictor/env-doctor)

Zero-dependency CLI. Scans source for `process.env` usage, diffs against `.env.example`, reports missing, undocumented, and unused vars. Exits `1` on issues, so it drops into CI.

---

**kolt@koltadams.com** · [koltadams.com](https://koltadams.com) · [LinkedIn](https://linkedin.com/in/koltadams)
