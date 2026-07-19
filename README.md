# Howdy 🤠

Cloud-native Customer Success leader who builds production-grade systems in the gaps — CI discipline, determinism contracts, cattle > pets.

---

### What I'm building

**RoleGauge** — a deterministic hiring intelligence engine. Four architectural bets that diverge from the market:

**1. Determinism as infrastructure.** Same inputs, same outputs, every time. `PYTHONHASHSEED=0` and `TZ=UTC` enforced at the Kubernetes level rather than in a test harness, snapshot-mode scraping, and a replay drift canary that validates dual-run consistency in CI. Every output is auditable; every signal traces to a source artifact.

**2. Rule-based classification, not ML.** A versioned role taxonomy maps every job title to the same classification every time — explicitly, through rules under change control, not silently through model drift. ML augments at the last mile only.

**3. A governed fleet, not a crawl.** 1,862 providers across 30 sectors and 9 ATS platforms aren't scraped — they're *governed*. A resolver chain (Wikidata → DBpedia → EDGAR → GitHub → Common Crawl) keeps every careers URL and ATS slug current, maintaining a board-migration history nobody else publishes. A healing engine auto-recovers providers whose boards rot out from under them.

**4. The archive is the product.** Scrape artifacts are an immutable temporal record, not a cache — the thing that makes "what changed, and when" answerable at all. Deleting them destroys signal you cannot re-derive, so the invariant is enforced by pre-commit hooks, runtime guards, and a single audited deletion path. 496 versioned migrations, no rewrites.

---

### How it's built

**Verification over assertion.** The operating rule is that *a green which cannot go red is not a gate*. Tests are proven to fail before they're trusted to pass; a count is meaningless without the selection that produced it; a claim describes the artifact, never the intent. Most of the hard bugs found in this system were found by attacking the evidence, not the code.

**Multi-agent development.** The engine is built by specialized agent lanes — backend, infrastructure, CI, recall — coordinating through a strict hub-and-spoke message bus with a single architect holding final call. Every load-bearing change carries two independent reviews plus an adversarial pass, because an author is the worst reviewer of their own reasoning.

**On-prem first.** A bare-metal k3s fleet with a Postgres moat, row-level security, least-privilege workload roles, and archival to object storage. Cloud-agnostic by construction.

---

### What I care about

- Deterministic systems, not vibe coding — AI is **always** last mile
- Reproducible builds and CI discipline
- Clear state contracts and invariants
- On-prem + cloud-agnostic deployment posture
- CNCF principles applied outside pure engineering roles

---

### Professional background

Senior Manager, Technical Customer Success (Linux / Kubernetes / AI) — leading enterprise cloud-native portfolios, focused on system maturity, scale models, and ROI.

The engineering above isn't a side hobby from the day job; it's the same discipline pointed at a harder problem. Running production infrastructure is what makes the customer conversations honest.

---

<sub>🦦</sub>
