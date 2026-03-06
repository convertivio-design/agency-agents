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

**What:** An interactive campaign simulator showing all 8 marketing agents collaborating on a real campaign — from strategy to content to measurable results.

**How to run:**
```bash
open examples/marketing-campaign-demo.html
# or serve it:
python3 -m http.server 8080 --directory examples
# then visit http://localhost:8080/marketing-campaign-demo.html
```

**Four campaign scenarios:**
| Scenario | What It Demonstrates |
|----------|---------------------|
| Product Launch | 6-week SaaS launch across all channels — blog, threads, TikTok, Reddit, referral loops |
| Viral Growth | Maximum reach in minimum time — trend-jacking, meme strategy, conversion funnels |
| Community Trust | 6-month authentic Reddit presence — from silent observation to 24K karma and AMA |
| App Store Launch | ASO, screenshot A/B testing, coordinated launch day, ratings strategy |

**Features:**
- Live agent roster showing which agents activate during each campaign phase
- Animated campaign timeline tracking progress through strategy → content → launch → optimize
- Content preview cards showing actual platform-specific outputs (tweets, TikTok scripts, Reddit posts, Instagram carousels, blog articles)
- Real-time metrics dashboard with animated counters (impressions, engagement rate, sign-ups, CAC, viral K-factor)
- Platform-specific styling (Twitter blue, Reddit orange, TikTok, Instagram, LinkedIn, App Store)

**Agents featured:** Growth Hacker, Content Creator, Twitter Engager, TikTok Strategist, Instagram Curator, Reddit Community Builder, App Store Optimizer, Social Media Strategist

**Key takeaway:** Non-technical stakeholders can watch 8 specialized agents collaborate on a campaign in real time — seeing the actual content each produces, which platforms it targets, and the measurable business results.

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
