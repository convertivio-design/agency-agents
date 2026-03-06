# Examples

This directory contains example outputs demonstrating how the agency's agents can be orchestrated together to tackle real-world tasks.

## Why This Exists

The agency-agents repo defines dozens of specialized agents across engineering, design, marketing, product, support, spatial computing, and project management. But agent definitions alone don't show what happens when you **deploy them all at once** on a single mission.

These examples answer the question: *"What does it actually look like when the full agency collaborates?"*

## Contents

### [identity-trust-demo.md](./identity-trust-demo.md)

**What:** A non-technical walkthrough of agent identity and trust verification, designed for executives, product managers, and compliance officers.

**The scenario:** AI agents are executing stock trades, accessing patient records, and deploying software. The demo walks through *why* agents need cryptographic identity, *how* the verification process works step by step, and *what happens* when a compromised agent tries to act — all using real-world analogies (passports, credit scores, security cameras, power of attorney).

**Sections:**
| Section | What It Covers |
|---------|---------------|
| The One-Sentence Problem | Why this matters in plain language |
| The Four Building Blocks | Identity, Trust, Evidence, Delegation — with analogies |
| See It in Action | Step-by-step trade execution (pass) and compromised agent (blocked) |
| Real Business Scenarios | Finance, healthcare, deployment, B2B |
| The Numbers That Matter | Executive-level metrics |
| Common Questions | FAQ for stakeholders |

**Key takeaway:** The entire verification process takes 10-50 milliseconds. Agents don't notice. Users don't notice. But the audit trail is complete and tamper-proof.

### [identity-trust-demo.html](./identity-trust-demo.html)

**What:** An interactive web demo of agent identity verification — zero dependencies, just open the HTML file in a browser.

**How to run:** Download and double-click the file, or:
```bash
open examples/identity-trust-demo.html
# or serve it:
python3 -m http.server 8080 --directory examples
# then visit http://localhost:8080/identity-trust-demo.html
```

**Features:**
- Four clickable scenarios: authorized trade, compromised agent, expired delegation, scope escalation
- Animated step-by-step verification with per-check timing
- Live trust score meters and agent identity cards
- Visual delegation chain showing scope narrowing
- Tamper-evident evidence chain that builds record by record
- Running totals: actions verified, actions blocked, evidence records, verification latency

**Key takeaway:** Non-technical stakeholders can click "Run Verification" and watch the system prove identity, check authorization, and block unauthorized actions in real time — all in under 50ms.

### [marketing-campaign-demo.html](./marketing-campaign-demo.html)

**What:** A full-funnel marketing operations simulator showing the complete machinery behind a B2B campaign — from ad click to closed deal, with agent decision logs, lead scoring, automation workflows, and multi-touch attribution.

**How to run:**
```bash
open examples/marketing-campaign-demo.html
# or serve it:
python3 -m http.server 8080 --directory examples
# then visit http://localhost:8080/marketing-campaign-demo.html
```

**What this demonstrates (the full marketing automation stack, not just content):**
| Area | What You See |
|------|-------------|
| Integration nodes | 10 connected systems (HubSpot CRM, SendGrid, Google Ads, Meta Ads, Segment+Mixpanel, Stripe, Slack, Tracking Pixels, Clearbit, Calendly) with live sync status |
| Agent decision logs | 20+ timestamped log entries showing reasoning: audience segmentation, ad campaign configs with bid strategies, A/B test statistical significance, funnel leak detection, lead score calculations |
| Lead pipeline | 6 individual leads tracked from anonymous visitor to closed-won/lost with score progression, stage changes, and every touchpoint |
| Lead scoring | Full score breakdowns: source (+10), blog read (+10), whitepaper (+15), company size (+10), pricing visits (+7), email engagement (+5) with MQL threshold triggers |
| Nurture sequences | 7-step email sequence with per-step open/click rates, branching logic (opened + pricing visit → fast-track), A/B test winner promotion |
| SDR handoff | MQL → Clearbit enrichment → ICP scoring → SDR round-robin → 3-touch outreach → SQL qualification with SLA monitoring |
| Retargeting | Pixel events → intent segmentation → creative matching → frequency capping → real-time suppression → lookalike expansion |
| Attribution | Linear model by channel with pipeline value, CAC, and LTV:CAC per channel |
| Revenue events | Deal-by-deal revenue timeline including a lost deal routed to win-back nurture |
| Conversion paths | Full multi-touch journeys for 2 closed deals (every touchpoint from first ad click to contract signed) |
| Funnel | Live visualization: Visitors 48.2K → Leads 4.8K → MQL 342 → SQL 89 → Opp 34 → Won 12 |

**Key agent logs that show deep expertise:**
- Ads agent detects CTR drop → diagnoses cause → pauses underperformer → promotes winner → adds negative keywords → adjusts bid targeting
- Email agent runs A/B test → reports z-test confidence at 99.2% → promotes winner → applies pattern to future sequences
- Growth agent runs referral timing experiment (n=2,400) → 181% lift → ships to 100% → projects $30K/month ad spend savings
- CRM agent promotes MQL with full score breakdown → triggers Slack alert → assigns SDR with SLA → fast-tracks nurture → updates retargeting audience → pulls Clearbit enrichment
- Analytics agent performs signup-to-activation cohort analysis → identifies integration step as 35% drop-off → recommends product + marketing + growth actions
- Social strategist ranks channels by pipeline-per-dollar → recommends budget reallocation with specific dollar amounts

**Key takeaway:** This demonstrates the full marketing automation stack — not "a bot that writes tweets" but a system that tracks 48K visitors through a funnel, scores and nurtures leads, optimizes ad spend in real-time, hands off to sales with context, and attributes $847K in pipeline to specific channels with CAC and LTV ratios.

---

### [nexus-spatial-discovery.md](./nexus-spatial-discovery.md)

**What:** A complete product discovery exercise where 8 agents worked in parallel to evaluate a software opportunity and produce a unified plan.

**The scenario:** Web research identified an opportunity at the intersection of AI agent orchestration and spatial computing. The entire agency was then deployed simultaneously to produce:

- Market validation and competitive analysis
- Technical architecture (8-service system design with full SQL schema)
- Brand strategy and visual identity
- Go-to-market and growth plan
- Customer support operations blueprint
- UX research plan with personas and journey maps
- 35-week project execution plan with 65 sprint tickets
- Spatial interface architecture specification

**Agents used:**
| Agent | Role |
|-------|------|
| Product Trend Researcher | Market validation, competitive landscape |
| Backend Architect | System architecture, data model, API design |
| Brand Guardian | Positioning, visual identity, naming |
| Growth Hacker | GTM strategy, pricing, launch plan |
| Support Responder | Support tiers, onboarding, community |
| UX Researcher | Personas, journey maps, design principles |
| Project Shepherd | Phase plan, sprints, risk register |
| XR Interface Architect | Spatial UI specification |

**Key takeaway:** All 8 agents ran in parallel and produced coherent, cross-referencing plans without coordination overhead. The output demonstrates the agency's ability to go from "find an opportunity" to "here's the full blueprint" in a single session.

## Adding New Examples

If you run an interesting multi-agent exercise, consider adding it here. Good examples show:

- Multiple agents collaborating on a shared objective
- The breadth of the agency's capabilities
- Real-world applicability of the agent definitions
