**Howdy** 🤠

I lead technical customer success (Linux, Kubernetes, AI) at an enterprise vendor. Off the clock I build and run **RoleGauge**, a deterministic hiring-intelligence engine tracking 1,862 companies' job boards (scaling to 20k) across 30 sectors and 9 ATS platforms, on bare-metal Kubernetes I own end to end.

- **Governed, not scraped.** Every provider is under change control. A resolver chain (Wikidata → DBpedia → EDGAR → GitHub → Common Crawl) keeps careers URLs and ATS slugs current, and a healing engine recovers boards that rot out from under it. The result is a board-migration history nobody else publishes.
- **Determinism enforced in Kubernetes, not in a test harness.** `PYTHONHASHSEED=0`, `TZ=UTC`, snapshot-mode scraping, and a replay-drift canary proving two runs of the same input agree.
- **Rule-based classification, not ML.** A versioned role taxonomy under change control: same title, same answer, every time. No silent model drift. ML augments the last mile only.
- **The archive is the product.** Scrape artifacts are an immutable temporal record, not a cache — the only reason "what changed, and when" is answerable at all. 496 versioned migrations and no rewrites; row-level security, least-privilege roles, and exactly one audited path that can delete anything.
- **A green that cannot go red is not a gate.** Tests are proven to fail before they're trusted to pass. A count means nothing without its selection. A report describes the artifact, never the intent. Most of the hard bugs here were caught by attacking the evidence, not the code.

Built by specialised AI agent lanes over a strict hub-and-spoke bus, with one architect holding final call and an adversary on anything load-bearing, because an author is the worst reviewer of their own reasoning. Cattle, not pets. 🦦
