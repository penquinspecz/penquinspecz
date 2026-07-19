# **Howdy** 🤠

I lead technical customer success (Linux, Kubernetes, AI) at an enterprise vendor. Off the clock I build and run production systems on bare-metal Kubernetes I own end to end.

---

## Projects

<!-- PATTERN FOR NEW ENTRIES — keep this shape so the section stays scannable:
### <Name> — <one-line what-it-is>
<One sentence of scale or stakes, with concrete numbers if you have them.>
- **<Contrarian claim>.** <The receipt. Evidence second, never first.>
(3–5 bullets. Each bullet leads with a stance a stranger could repeat, then earns it.)
-->

### RoleGauge — deterministic hiring intelligence

Tracks 1,862 companies' (scaling to 20k) job boards across 30 sectors and 9 ATS platforms. A core principle is something rare today: *no LLM at runtime, EVER.* You wouldn't want the same career question subjectively answered two different ways - we breathe that.

- **Governed, not scraped.** Every provider is under change control. A resolver chain (Wikidata → DBpedia → EDGAR → GitHub → Common Crawl) keeps careers URLs and ATS slugs current, and a healing engine recovers boards that rot out from under it. The result is a board-migration history nobody else publishes.
- **Determinism enforced in Kubernetes, not in a test harness.** `PYTHONHASHSEED=0`, `TZ=UTC`, snapshot-mode scraping, and a replay-drift canary proving two runs of the same input agree.
- **Rule-based classification, not ML.** A versioned role taxonomy under change control: same title, same answer, every time. No silent model drift. ML augments the last mile only.
- **The archive is the product.** Scrape artifacts are an immutable temporal record, not a cache — the only reason "what changed, and when" is answerable at all. 496 versioned migrations and no rewrites; row-level security, least-privilege roles, and exactly one audited path that can delete anything.

---

## How I build

**AI is a tool, Determinism is a principle.** A green that cannot go red is not a gate... Tests are proven to fail before they're trusted to pass. Most of the hard bugs I find are caught by attacking the evidence, not the code; it's a beautiful world where smell now counts as much as code-vision.

Built by specialised AI agent lanes over a strict hub-and-spoke cross-harness bus, with an architect holding final call and an adverserial red-team code review framework, myself as operator and Chief Arch.

Cattle, not pets. 🦦
