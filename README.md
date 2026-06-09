# Solo Founder Startup Ideas — Deep Research Report

**Date:** June 9, 2026
**Method:** Five parallel research streams (solo-founder revenue evidence, AI's reshaping of the landscape, vertical/B2B niches, 2026 trend signals, and solo-SaaS economics benchmarks), each drawing on dozens of primary sources, then cross-verified and synthesized against an evidence-based evaluation framework. Revenue claims are flagged where self-reported.

---

## TL;DR — The ideas I'd sponsor, ranked

| # | Idea | Buyer | Price point | Confidence |
|---|------|-------|-------------|------------|
| 1 | EU e-invoicing (Peppol) tooling for SMBs, sold through accountants | EU SMBs / accounting firms | €29–99/mo | High — narrowed wedge (see deep dive) |
| 2 | Security + maintenance subscription for vibe-coded apps | Non-technical app creators | $49–199/mo | High — repositioned to maintenance retainer (see deep dive) |
| 3 | AI-agent readiness for SMB e-commerce ("is your store visible to ChatGPT?") | Shopify/Woo merchants | $29–149/mo | High |
| 4 | Vertical AI receptionist for one offline trade | Home-service SMBs | $99–299/mo | Downgraded — product play closed (see deep dive) |
| 5 | Client-document chasing tool for bookkeeping firms | Bookkeeping/accounting firms | $49–149/mo | Medium-high |
| 6 | B2B-commerce apps on Shopify (quotes, net terms, buyer accounts) | Shopify B2B merchants | $79–299/mo | Medium-high |
| 7 | Deep two-app connector / niche dataset API | SMB ops teams / devs | $29–500+/mo | Medium |
| 8 | MCP / agent-infrastructure micro-tooling | Dev teams adopting agents | $20–99/seat | Medium (technical founders only) |

---

## The evaluation framework (what the evidence says to screen for)

Before the ideas, the screens they had to pass. These come from 2024–2026 benchmark data, not vibes:

1. **Business/professional buyer, never consumer.** Sub-$25 prosumer products churn at ~6.1%/mo median (ChartMogul); mobile consumer subscriptions churn at 13–14%/mo (RevenueCat, ~30k apps). At $500+ ARPA churn drops to 2.2%/mo. A solo founder cannot staff the replacement treadmill of consumer churn. Target ≤3.5%/mo with annual-plan push.
2. **Price ≥$29/mo, sweet spot $79–149.** $10K MRR = ~100 customers at $99 vs. ~345 at $29. Cheap customers generate churn; expensive ones generate feedback. Avoid lifetime deals post-validation (AppSumo takes ~70%; LTD cohorts are high-support, high-refund).
3. **Narrow, bounded use case = survivable support load.** AI support now deflects 50–67% of tier-1 (Intercom Fin: ~67% resolution at ~$0.99/resolution) — but only with clean docs and a narrow product. Vertical beats horizontal for a solo operator.
4. **Moat = distribution + workflow depth + data, never features.** AI-assisted cloning compresses feature parity to 12–18 months. What survives: being embedded in a workflow (scheduling + invoicing + dispatch = painful switching), accumulated proprietary data, owned distribution, trust/community.
5. **No single-platform dependency for both channel AND function.** Twitter's 2023 API repricing killed an entire app ecosystem in 7 days. Shopify apps trade at a 20–30% valuation discount for this reason. One platform for *either* distribution *or* function is acceptable; both is disqualifying.
6. **Realistic expectations:** ~40% of micro-SaaS never pass $1K MRR; median time to $10K MRR for those who get there is 12–18 months. Exit math: ~3.9x trailing-twelve-month profit (Acquire.com, Jan 2026 — median across 2024 and 2025). A $10K-MRR product at 80% margin is a ~$350–450K asset. Run small bets until one shows retention signal, then concentrate.
7. **"Why now" must be structural** — a regulation with a date, a platform shift with adoption data, or a cost trend with an index. Not a listicle.

---

## The ideas

### 1. EU e-invoicing (Peppol) tooling for SMBs — sold through accountants

**What:** A dead-simple bridge for small businesses to comply with EU e-invoicing mandates: PDF/ERP → EN 16931-compliant e-invoice, a cheap Peppol access point, inbound-invoice receiving inbox, and a compliance dashboard an accountant can manage for 50 clients at once.

**Target customer:** EU SMBs below the threshold where Sage/SAP-tier tooling makes sense — reached **through accountants and bookkeepers**, who are the trusted channel and feel the compliance pain across their whole client book.

**Monetization:** €29–99/mo per business, or accountant-firm plans (€199–499/mo for a client portfolio). Annual plans default.

**Why now (the strongest "why now" of any idea on this list):** This is *forced* adoption with statutory dates. Germany: all businesses must receive e-invoices since Jan 2025; sending mandatory for >€800K turnover Jan 2027, everyone Jan 2028. Belgium: B2B Peppol mandate **already live** (Jan 1, 2026) — PDF-by-email is now non-compliant. France: phased Sept 2026–2028. ViDA (adopted March 2025) makes intra-EU B2B e-invoicing mandatory by July 2030. Billentis projects ~28%/yr market growth to €22–24B by 2028. Millions of SMBs must do this whether they want to or not.

**Why a solo founder wins:** The enterprise players (Pagero, Basware, Sovos) are priced and built for mid-market+. The long tail needs something that costs less than a phone bill and requires zero learning. Compliance products have intrinsically low churn — you can't churn off a legal requirement. The accountant channel means one sale = many seats, without an enterprise sales motion.

**Key risks:** (a) Accounting-software incumbents bundle "good enough" e-invoicing — mitigate by serving businesses on spreadsheets/legacy ERPs and by being the *multi-country* normalizer; (b) per-country certification/access-point requirements add bureaucratic setup — this is actually a feature (it's a moat against drive-by competitors); (c) country-by-country fragmentation means picking a beachhead — Belgium (live now) or France (Sept 2026 deadline panic) are the obvious ones.

**First 90 days:** Pick Belgium or France. Build PDF→Peppol converter + receiving inbox. Get 10 accounting firms piloting via bookkeeper communities and accounting-association directories. Charge from day one.

---

### 2. Security + maintenance subscription for vibe-coded apps

**What:** "The mechanic for your AI-built app." One-click security audit (auth, RLS/data exposure, API keys, payment flows) for apps built on Lovable/Bolt/v0/Replit, with auto-fix where safe, a plain-English report where not, and an ongoing monitoring + maintenance retainer.

**Target customer:** The ~63% of vibe-coding users who are non-developers (converging data from Lovable's own numbers, Taskade, and community analyses) who shipped an app that handles real user data and have no idea whether it's safe.

**Monetization:** $99–299 one-time audit as the wedge → $49–199/mo monitoring/maintenance subscription. The audit is lead-gen; the retainer is the business.

**Why now:** The security debt is documented, not hypothetical. CVE-2025-48757: 10.3% of 1,645 scanned Lovable showcase apps had critical row-level-security failures exposing PII. A separate pen test found 69 vulnerabilities (6 critical) across 15 vibe-coded apps; ~45% of AI-generated code carries vulnerabilities. Sources consistently describe a "month-3 wall" where codebases outgrow their creators' prompting ability. The creator population is growing by millions per year and nothing downstream of "generate the app" is solved.

**Why a solo founder wins:** Buyers are non-technical, so they buy *outcomes and reassurance*, not features — which means premium pricing and low feature-competition. AI does most of the audit work; the founder's leverage is trust and packaging. The early entrants (cottage scanners) validate demand without saturating it; nobody owns the *brand* for "vibe-code safety" yet.

**Key risks:** (a) Platforms build security in — mitigate by being cross-platform (the platforms compete with each other, not with you) and by owning the maintenance/rescue layer, which platforms structurally won't do; (b) liability framing — sell "audit and hardening," not "guarantee"; (c) the customer base has a hobbyist tail with high churn — qualify for apps with real users/revenue.

**First 90 days:** Build scanner for the top 3 platforms covering the documented vulnerability classes (RLS, exposed keys, auth bypass). Post teardowns of (anonymized) vulnerable app patterns in vibe-coding communities — the content markets itself through fear that is, in this case, justified. Convert audits to retainers.

---

### 3. AI-agent readiness for SMB e-commerce

**What:** Monitoring + remediation that makes small online stores visible and transactable to AI shopping agents: structured-data/feed fixes, agent-readability audits, and a recurring "how AI assistants see your store" report across ChatGPT, Perplexity, Gemini, and agentic-checkout surfaces.

**Target customer:** Long-tail Shopify/WooCommerce/BigCommerce merchants ($100K–$5M GMV) — below the enterprise tier that Profound-class tools ($495+/mo) serve.

**Monetization:** $29–149/mo, tiered by catalog size; agency plans for the freelancers who manage many stores.

**Why now:** Adobe Analytics: AI-referred traffic to US retailers **+393% YoY in Q1 2026** (+693% during holiday 2025), and AI-referred traffic now **converts 42% better** than human traffic — a reversal from a year earlier. Morgan Stanley projects agentic commerce at $190–385B by 2030. Adobe's same report notes most retail sites are *not machine-readable to agents*. Merchants can see the channel shift in their own analytics, which makes the sale self-evident.

**Why a solo founder wins:** The enterprise players ignore the long tail; the SMB tier needs a $49/mo product, not a $6K/yr contract. It's a classic "new channel = new tooling" land grab, like early SEO tools in 2005 — and those were largely built by tiny teams.

**Key risks:** (a) Standards are moving fast (agentic checkout protocols, schema evolution) — solo speed is actually the advantage here, but expect rework; (b) Shopify ships native agent-readiness — mitigate by being cross-platform and by owning the *monitoring/reporting* layer (platforms fix their own surface, they don't report on competitors' engines); (c) the adjacent AEO/GEO category is crowding — differentiate by being commerce-specific (feeds, inventory, checkout) rather than content-visibility-generic.

**First 90 days:** Build the free "agent visibility scan" as the viral wedge (every merchant wants their score). Charge for continuous monitoring + fixes. Distribute via e-commerce communities and the Shopify app store (channel only — function works everywhere, passing the platform-risk screen).

---

### 4. Vertical AI receptionist for one offline trade

**What:** A packaged AI phone receptionist for **one** trade vertical (e.g., plumbing/HVAC or salons) — answers every call, books jobs into the calendar, captures lead details, quotes standard services from the business's price sheet, and texts the owner a summary. Built on Vapi/Retell-class infrastructure; the product is the *vertical workflow*, not the voice tech.

**Target customer:** 1–10-person service businesses where a missed call is a lost $300–3,000 job. ~62% of inbound SMB calls go unanswered at peak.

**Monetization:** $99–299/mo. The ROI math is attributable ("it booked 11 jobs last month"), which is the single best churn defense that exists.

**Why now:** Voice AI crossed the quality threshold in 2024–25; Beside (AI receptionist) hit $4M ARR and 20,000+ paying customers, validating category willingness-to-pay, while indie developers are already profitably reselling packaged agents. The customer is offline — they will never build this themselves and the labs will never sell to them directly.

**Why a solo founder wins:** Horizontal players must be everything to everyone; a solo founder can win one trade with deep defaults (the plumber's call script, the salon's booking rules, integration with the one or two calendars/FSM tools that trade actually uses). Vertical depth + operational embedding = the highest-NRR pattern in SMB software.

**Key risks:** (a) Crowding — the category is hot, so the vertical wedge and local distribution (trade Facebook groups, supplier networks, one good affiliate in the niche) matter more than the tech; (b) infra dependency on Vapi/Retell — acceptable: function-layer dependency with multiple substitutable vendors; (c) support expectations from non-technical owners — bounded by doing one trade with one workflow; (d) telephony edge cases eat time — budget for it.

**First 90 days:** Pick the trade. Onboard 10 local businesses personally (white-glove). Nail the booking-rate metric. Then productize onboarding and buy distribution via trade-niche affiliates (the HeadshotPro affiliate playbook, applied to a vertical).

---

### 5. Client-document chasing for bookkeeping firms

**What:** A point tool that automates the most-hated workflow in every bookkeeping/accounting firm: chasing clients for documents (bank statements, receipts, signatures) with automated sequences, a no-login client portal, and status across the whole client book. Bolt-on, not platform — works alongside QBO/Xero/Karbon.

**Target customer:** Solo bookkeepers and 2–20-person accounting firms. They complain publicly that Karbon is "too complicated" and Canopy's modular pricing balloons; low-end entrants (Financial Cents at $19/user, Cone at $5/user) prove the budget tier is viable and still underserved.

**Monetization:** $49–149/firm/mo. Annual default — firms budget annually.

**Why now:** Steady-state pain rather than a structural wave — but accountants are the single best solo-founder customer profile in the dataset: they pay reliably, churn little (ChartMogul's low-churn band), congregate in findable communities (r/Accounting, Bookkeeping Side Hustle, accounting Facebook groups), and refer each other constantly. And there's **portfolio synergy with idea #1**: same buyer, same channel — e-invoicing compliance and document-chasing can share a distribution engine.

**Why a solo founder wins:** Incumbents keep moving upmarket into all-in-one practice management; the focused "does one thing perfectly, costs less than lunch" bolt-on is structurally unattractive to them and perfect for one person. Support load is bounded: one workflow, professional users.

**Key risks:** (a) Practice-management suites bundle a "good enough" version — mitigate by being best-in-class at the *client experience* side (the part suites neglect); (b) it's a feature-sized product — true, and that's fine: feature-sized products at $99/mo with near-zero churn are exactly what the Acquire.com data says sells at the best multiples; (c) crowded adjacent space (proposal tools, engagement letters) — stay on the chasing/portal wedge.

**First 90 days:** Build the chase-sequence + portal MVP. Get 20 firms from bookkeeping communities. Obsess over time-to-first-chase < 10 minutes from signup.

---

### 6. B2B-commerce apps on Shopify

**What:** Apps for Shopify merchants selling wholesale/B2B: quote management, net-terms/credit workflows, multi-user buyer accounts, tiered/contract pricing. Possibly several small apps rather than one suite.

**Target customer:** The fast-growing cohort of Shopify merchants doing B2B — Shopify's B2B GMV grew ~101% YoY, while the app store remains saturated in B2C categories (email, reviews, upsells) and comparatively thin here.

**Monetization:** $79–299/mo via the app store. Shopify takes 0% of the first $1M (since Jan 2025), which materially improves solo economics.

**Why now:** B2B is Shopify's strategic growth vector, and buyer intent inside the app store is real purchase intent — merchants search the store with a problem and a credit card. Meanwhile the ecosystem data shows the spoils are power-law (median dev ~$725/mo; top quartile ~$167K/yr) — meaning category selection, not effort, is the variable. B2B is the underweighted category.

**Why a solo founder wins:** Documented precedent — solo founders run Shopify app portfolios past $100K/mo (e.g., Erikas Mališauskas, self-reported via Indie Hackers AMA). The app-store channel replaces marketing for the first $10–30K MRR.

**Key risks:** This is the one idea on the list that deliberately accepts platform risk — Shopify regularly sherlocks app categories, and Shopify apps trade at a 20–30% valuation discount. Mitigations: B2B workflows are deep and idiosyncratic (less sherlockable than reviews/email), build 2–3 apps rather than one, and treat it as a cash-flow business, not a legacy asset.

**First 90 days:** Mine app-store reviews of existing B2B apps for unmet needs (1-star reviews of competitors are a free roadmap). Ship the narrowest viable app (e.g., quote-to-order). Iterate on app-store SEO.

---

### 7. Deep two-app connector or niche dataset API

**What:** Either (a) a best-in-class deep sync between two specific high-value systems (e.g., QuickBooks/Xero ↔ a vertical ops tool, or accounting ↔ e-commerce at the line-item level), or (b) a niche data API serving one hungry use case (the ScrapeCreators pattern — solo founder, $10K MRR in ~12 months on social-data endpoints).

**Target customer:** SMB ops teams (connectors) or developers/growth teams (APIs).

**Monetization:** Connectors: $29–99/mo flat. Data APIs: usage-based, $500–2,000/mo for serious clients.

**Why now:** Evergreen rather than wave-driven — but the evidence shows the pattern reliably sustains multiple small profitable players even in Zapier's shadow (G-Accon, Coupler.io, solo-run Retriever in just the QBO↔Sheets niche). Deep two-app sync beats shallow many-app automation because edge cases (the actual product) compound into switching costs.

**Why a solo founder wins:** Bounded scope, technical buyers who self-serve, integration lock-in, near-zero marketing if you pick a pair with existing search demand ("[App A] to [App B] sync" queries).

**Key risks:** (a) Modest ceiling — most of these plateau at $5–30K MRR (acceptable: that's a $250–450K asset at current multiples, or a great cash-flow base for a portfolio); (b) API platform risk on both ends — pick stable, boring platforms (accounting software APIs are the most stable in SaaS); (c) for data APIs, ToS/legal exposure — pick data sources accordingly.

**First 90 days:** Validate via search volume + community complaints for the chosen pair. Ship sync for the 5 most-demanded objects. Charge immediately.

---

### 8. MCP / agent-infrastructure micro-tooling *(for technical founders)*

**What:** Small, sharp tools in the AI-agent infrastructure layer: MCP server gateways/auth, agent-behavior observability for small teams, eval harnesses for specific agent use cases. Not a Langfuse competitor — the gaps *underneath* and *beside* the funded players.

**Target customer:** Development teams deploying agents/MCP in production — a population growing extremely fast since MCP went to the Linux Foundation (Dec 2025) with OpenAI/Google adoption.

**Monetization:** $20–99/seat/mo or flat team pricing; open-core works here.

**Why now:** Category validation is strong — ClickHouse acquired Langfuse (Jan 2026; 2,000+ paying customers), and practitioners consistently report debugging/inspection tooling remains underbuilt. Greenfield categories reward speed, which is the solo founder's only structural advantage.

**Key risks:** This is the highest-beta idea on the list: (a) the labs or funded players may absorb any given niche within 12–18 months — pick wedges that are *operationally* annoying rather than technically glamorous (auth, billing for agent usage, compliance logging); (b) developer price sensitivity and build-it-myself churn; (c) requires genuine technical depth — this idea is only for a founder who is already living in this stack. Sponsored with the explicit caveat: ship fast, charge early, be willing to sell or fold the bet within 18 months.

---

## Post-publication deep dives (June 9, 2026)

Second-round research on ideas #1, #2, and #4 — focused on saturation, sherlock risk, and structural barriers. These revise the original assessments.

### Idea #4 (AI receptionist): downgraded — the product window has closed

- **Top end:** Avoca raised $125M+ at a **$1B valuation (April 2026)**, eight-figure ARR, partnered with ServiceTitan/Nexstar — it owns mid-market trades.
- **Bottom end:** Rosie ($49/mo), Sameday (~$3.5M ARR), NextPhone ($199/mo) own the low end; salons collide with Zenoti's native AI receptionist; restaurants with Slang.ai ($36M Series B); auto with Numa.
- **Sherlocked already:** ServiceTitan Contact Center Pro voice agents (Nov 2024), **Jobber AI Receptionist GA Aug 2025** ($99/mo add-on), Housecall Pro CSR AI. The standalone product's only durable edge — deep FSM integration — is now native to the FSMs.
- **Reseller channel is industrialized:** white-label wholesale at ~$55/agent resold at $250–500/mo, 1,000+ agencies on a single white-label dashboard; every plumber is cold-emailed about AI receptionists weekly.
- **Retention is ugly at the low end:** median gross revenue retention ~40%, ~23% for sub-$50/mo products; 31% of consumers hang up on AI immediately.
- **What remains:** after-hours/overflow-only hybrid positioning (the evidence-backed retention pattern), emergency dispatch triage with on-call rotation logic, Spanish-bilingual metros, and forgotten trades (septic, well drilling, chimney, appliance repair) — viable as a high-touch local productized service (~$300–500/mo, dozens of clients), not as a SaaS product company.

### Idea #2 (vibe-code security): confirmed demand, but reposition away from scanning

- **Scanning is saturated and being sherlocked:** 8+ self-serve scanners at $5–29/mo (Vibe App Scanner closest to category leader, with an SEO moat); Lovable shipped Security Checker 2.0 (Aug 2025); **Replit's Security Agent + Auto-Protect is literally "ongoing security monitoring" as a platform feature**. Pure scanning has a ~2-year half-life.
- **Audits/rescue are crowded but fragmented:** $500–3,000 audits (Sherlock Forensics, Beesoul — which reports "is my Lovable app safe?" as its #1 inbound request), £999+ rescue services, 10+ dev shops pivoted to "vibe-code cleanup" ($2K–20K projects), Fiverr bottom at $5–50.
- **The open slot nobody owns:** a **recurring maintenance + security + compliance subscription** ($200–500/mo) for revenue-generating apps whose creators hit the documented "month-3 wall." Supply is project-based; demand signals are strong; no public MRR leader exists. Durability drivers beyond scanning: Apple began rejecting vibe-coded apps (May 2026), EU AI Act + GDPR liability stacking, cyber-insurance compliance demands.
- **Market size:** Lovable ~8M users/$500M+ ARR/~1M new projects per week; Replit $525M annualized. Funnel cliff to apps-with-real-user-data is steep (1–3%), so the buyer pool is tens of thousands, not millions — right-sized for a solo business, not venture scale.
- **Caution flag:** no public MRR reports from anyone in the niche yet — validate the retainer conversion rate early.

### Idea #1 (EU e-invoicing): still high confidence, but the wedge is narrower than first written

- **Not structurally excluded:** solo founders can ride existing access-point APIs (Recommand, e-invoice.be at €0.18–0.25/invoice, getpeppr at €49–399/mo built on Storecove, Qvalia €39/mo) instead of pursuing Peppol certification. Proof of indie viability: Recommand reached **2,500 customers in ~1 year** riding the Belgian mandate.
- **But horizontal SMB invoicing is gone:** Belgium's floor is €0–10/mo (Billit €7.50, Accountable free Peppol, Dexxter €180/yr); Germany is incumbent-dominated with no Peppol mandate.
- **France PA status is out of reach** (ISO 27001, ~€100K all-in), but the officially sanctioned OD/"Solution Compatible" role on top of one of the ~108 registered platforms is low-burden.
- **The real wedges:** (a) embedded Peppol APIs/SDKs for vertical SaaS that must add compliant sending, (b) PDF-to-Peppol conversion for the long tail (43% of Belgian zero-employee businesses still had no Peppol ID as of Jan 2026; Hermes, the free state platform, was decommissioned Dec 2025; Belgium's 120% tax deduction subsidizes paid tools), and (c) the **French SME issuing wave of Sept 2027** — the one mandate window still genuinely ahead.

## Watchlist (close, but didn't make the sponsored list)

- **Vertical AEO/GEO for local SMBs** (dentists, law firms): explosive category growth (2,000%+ on G2 since March 2025) but high platform risk — engines consolidate, Google publishes its own guidance, and tool durability is unproven. The commerce-specific version (idea #3) has better grounding.
- **Managed self-hosting for SMBs** ("we run your Nextcloud/Zulip for $99/mo"): demand is real (SaaS inflation 12–14.5%/yr, Vertice; Nextcloud interest tripled in early 2025) but it puts a solo founder on pager duty — the one ops burden that genuinely doesn't scale to a team of one. Viable as a productized service with strict scope; not as open-ended infra ops.
- **Digital legacy / credential-first estate tooling**: strong demographic tailwind (56% of Americans have no estate plan; LastPass's "digital will" feature lifted premium DAUs) but consumer churn dynamics; would need a B2B2C channel (financial advisors, estate attorneys) to pass the screens.
- **Caregiver coordination**: large and growing (~16% CAGR) and genuinely underserved, but B2C, emotionally heavy support, and fragmented willingness-to-pay. Better suited to a mission-driven funded team.

## Anti-portfolio (what I would not fund in 2026, with reasons)

- **Thin AI wrappers** (writing assistants, chat-with-PDF, generic image UIs, prompt marketplaces): the labs absorbed each of these within ~18 months of shipping the capability; survivors commoditized to lifestyle scale (ChatPDF ~$440K/yr) or imploded (Jasper's trajectory, Tome's pivot).
- **AI companion apps**: winner-take-most (top 10% of apps capture ~89% of revenue), moderation and regulatory tail risk, and a documented privacy disaster (43M leaked intimate messages, Oct 2025).
- **Boilerplates/starter kits**: ShipFast's decay from ~$100K/mo (2024) to ~$20K/mo (2025) is the category telling you AI codegen ate it.
- **Anything dependent on one platform for both channel and function** — the Twitter API massacre (7 days' notice, ecosystem dead) is the permanent cautionary tale.
- **Restaurant tech, generic chatbot builders, consumer subscription apps, CSRD/ESG reporting for SMBs** (the EU Omnibus gutted the SMB mandate and the Commission ships a free tool), and **vibe-coding app builders themselves** (138+ tools competing against Lovable/Bolt/Cursor at $200M–2B ARR — closed to new solo entrants).

## Cross-cutting playbook (what the evidence says about execution)

- **Distribution realities, mid-2026:** Product Hunt is dead for indies (worst-converting channel; ~89% wouldn't relaunch). X build-in-public is a *trust amplifier, not a traffic channel* — no app in the studied dataset passed $1M ARR on it alone. What works: affiliate programs (HeadshotPro pays out ~$50K/mo to ~5,000 affiliates), niche communities, data-moat SEO (thin programmatic SEO is dead; proprietary-data SEO survives AI Overviews), and for ideas #1/#5, channel partners (accountants).
- **Pricing:** flat and simple, ≥$29/mo, annual default. Hybrid (flat + usage cap) only where costs are variable (voice minutes, API calls).
- **Sequencing:** small bets until retention signal, then concentrate — the data favors Vassallo-style exploration but SaaS compounding punishes permanently divided attention. Ideas #1+#5 are designed to share a channel precisely so exploration isn't divided attention.
- **Expectations:** 12–18 months to $10K MRR is the *successful* case. ~40% of launches never pass $1K MRR. The exit market pays ~3.9x profit for clean, low-founder-dependency businesses — build with that scoreboard in mind from day one.

---

## Appendix: research stream summaries

1. **Solo-founder revenue evidence (2025–26):** Verified acquisition-market data (Acquire.com median 3.9x TTM profit; Flippa 2.5–4.5x) against self-reported MRR claims (Tony Dinh/TypingMind ~$130–160K/mo; Marc Lou $1.03M across 2025, diversified; HeadshotPro ~$300K/mo peak; cautionary inflation in levels.io's "$1M ARR in 17 days"). Recurring profitable categories: niche B2B utilities, platform-ecosystem apps, vertical AI tools, directories/job boards.
2. **AI's reshaping of the landscape:** The wrapper graveyard is real but killed margins more than companies; durable AI products own workflows, data, or offline customers. Verified solo high-water mark: Base44, solo-built, sold to Wix for $80M cash six months post-launch. New solo-serveable categories: voice AI for SMBs, AEO/GEO, agent observability, MCP tooling, AI-content compliance.
3. **Vertical/B2B niches:** Best solo-fit verticals: accounting/bookkeeping firms, single trades, small law point-tools, "boring" verticals (funeral homes ~45% without centralized software). Strongest compliance wave: EU e-invoicing (Belgium live, France Sept 2026, Germany 2027–28, ViDA 2030). Platform data: Shopify median dev ~$725/mo but 0% rev-share to $1M and a B2B gap; WordPress still the most proven indie marketplace; Stripe Apps thin but uncrowded.
4. **2026 trend signals:** Vibe-code security aftermarket (CVE-2025-48757; 63% of creators non-developers), agentic commerce (+393% YoY AI retail traffic, converts 42% better), SaaS price revolt (12–14.5% SaaS inflation driving unbundling/self-hosting), YC RFS 2026 themes, agetech/digital-legacy demographics.
5. **Solo-SaaS economics:** Churn by segment (consumer 6–14%/mo vs. SMB 2–4%), pricing data ($29–149 sweet spot), support benchmarks (AI deflects 50–67% of tier-1 in 2026), failure base rates (~40% never pass $1K MRR), defensibility evidence (distribution/data/workflow, not features), platform-risk case studies, exit multiples.

*Primary sources are cited inline throughout the underlying research streams; headline claims above were cross-checked across at least two independent sources where possible, and flagged as self-reported where not.*
