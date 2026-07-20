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

Tracks 1,862 companies' (scaling to 20k, global companies but only focused on North America hirings right now) job boards across 30 sectors and 9 ATS platforms. A core principle is something rare today: *no LLM at runtime, EVER.* You wouldn't want the same career question subjectively answered two different ways - we breathe that.

- **Governed, not scraped.** Every provider is under change control. A resolver chain (Wikidata → DBpedia → EDGAR → GitHub → Common Crawl) keeps careers URLs and ATS slugs current, and a healing engine recovers boards that rot out from under it. The result is a board-migration history nobody else publishes.
- **Determinism enforced in Kubernetes, not in a test harness.** `PYTHONHASHSEED=0`, `TZ=UTC`, snapshot-mode scraping, and a replay-drift canary proving two runs of the same input agree.
- **Rule-based classification, not ML.** A versioned role taxonomy under change control: same title, same answer, every time. No silent model drift. ML augments the last mile only.
- **The archive is the product.** Scrape artifacts are an immutable temporal record, not a cache — the only reason "what changed, and when" is answerable at all. 496 versioned migrations and no rewrites; row-level security, least-privilege roles, and exactly one audited path that can delete anything.

### Puddle — the honest instrument for your AI agent fleet (macOS)

A menu-bar city that meters every AI coding agent on your machine — usage, cost, context pressure, and the water it all theoretically drinks — while staying leaner than the tools it watches. 2,100+ tests, six providers, one deadpan municipal government. Public launch imminent; the CLI is [@puddlectl](https://twitter.com/puddlectl).

- **Every number carries a receipt.** MEASURED / DERIVED / ESTIMATE stamps on every numeral in the app, enforced by a CI gate that fails the build if any surface renders a number outside the stamp system. Honesty as a compiler error, not a copy choice.
- **Zero telemetry is a build artifact, not a promise.** The release audit scans the binaries for network symbols and names every authorized exception in a public ledger; the only calls it ever makes are ones you enabled, to your own accounts, each visible in a live log. The category leader shipped crash telemetry under a "no telemetry" banner — we ship the audit script.
- **It refuses to know things.** Unknown liveness renders *idle*, never *zombie*; unmeasurable spend renders absent, never $0.00; every absence states its reason. An instrument that can't return the other answer isn't one.
- **Performance is the product.** Whole-fleet observability budgeted at <1% idle CPU against a published per-phase performance covenant, re-measured on a 16 GB real corpus at every gate — including the incident report that created the covenant. Popular incumbents idle at 10× the memory.
- **kubectl energy, municipal soul.** `puddlectl top sessions` for your agent fleet, approve agent actions without leaving flow, jump to the exact terminal pane that asked — one instrument from notch to CLI, with a cross-harness agent bus on the roadmap. Also: the water your tokens drink is cited to primary sources, and the almond is real.

---

## How I build

**AI is a tool, Determinism is a principle.** A green that cannot go red is not a gate... Tests are proven to fail before they're trusted to pass. Most of the hard bugs I find are caught by attacking the evidence, not the code; it's a beautiful world where smell now counts as much as code-vision.

Built by specialised AI agent lanes over a strict hub-and-spoke cross-harness bus, with an architect holding final call and an adverserial red-team code review framework, myself as operator and Chief Arch.

Cattle, not pets. 🦦
