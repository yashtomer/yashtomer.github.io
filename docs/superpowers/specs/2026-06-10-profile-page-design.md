# Yashdeep Tomer — Profile/Lead-Generation Page — Design Spec

**Date:** 2026-06-10
**Goal:** A single-page, SEO-optimized personal profile site that converts visitors into client leads for freelance/contract work.

## Client facts (confirmed by user + resume `Yash_Tomar_Resume_Premium.pdf`)

- **Name (branding):** Yashdeep Tomer (user's explicit choice; resume uses "Yash Tomar" — one find-replace to flip)
- **Experience:** 15+ years; currently Sr. Manager – Technology at Aeologic Technologies; ex-IndiaMart, Monster India
- **Positioning (from resume):** AI Technical Architect — Agentic AI, Voice AI, RAG/LLM orchestration + Full-Stack + DevOps. Voice/Agentic AI is the differentiator and primary SEO niche.
- **Proof points:** missed-call rate 33% → <5%; sub-2s voice AI turn-taking; zero per-token cost via local LLMs; sub-2-min speed-to-lead; projects for SpiceJet (Kargo360), a Saudi Arabian bank, an Australian finance brokerage, RatePerSqft
- **Stack highlights:** LangChain/LangGraph/LlamaIndex/CrewAI/AutoGen/MCP · OpenAI/Claude/Gemini · LiveKit/Whisper/ElevenLabs/Deepgram/Twilio · Pinecone/ChromaDB/pgvector · Node.js/NestJS/Python/FastAPI · React/Next.js/Angular · AWS/GCP/Docker/K8s/Terraform
- **Education/certs:** MCA; LangChain for LLM App Development (DeepLearning.AI); Generative AI with LLMs (Coursera)
- **Target market:** Global (US/EU/remote startups and businesses)
- **Contact channels:** Email `yashdeep.tomer@gmail.com`, WhatsApp `+91 98999 86773`, LinkedIn `https://www.linkedin.com/in/yashtomar-tech/`, GitHub `https://github.com/yashtomer`
- **Location:** Ghaziabad, India (remote, global)
- **Domain:** not purchased yet — use `https://yashdeeptomer.com/` as a clearly-marked placeholder for canonical/OG URLs.

**Hero positioning:** "AI Technical Architect & Full-Stack Developer" — lead with
Agentic/Voice AI expertise (high-value, low-competition keywords: "hire voice AI
developer", "agentic AI consultant", "RAG developer for hire"), with full-stack +
DevOps as breadth. Services cards become: AI & Agentic Systems, Voice AI Agents,
Full-Stack Web & Mobile, DevOps & Cloud. Add a "Selected work" section with the
four strongest resume projects and their measurable outcomes.

## Approach

Single-page static site. No build step, no JS framework. Deployable as-is to
Netlify / Vercel / GitHub Pages. Rationale: fastest possible load (Core Web
Vitals = SEO ranking factor), zero maintenance, ideal for a personal brand
lead-capture page.

## Files

| File | Purpose |
|---|---|
| `index.html` | Full page markup, semantic HTML5, JSON-LD, meta tags |
| `styles.css` | All styling (single stylesheet, mobile-first) |
| `robots.txt` | Allow all crawlers, point to sitemap |
| `sitemap.xml` | Single-URL sitemap |

## Page sections

1. **Header/nav** — name wordmark, anchor links (Services, Skills, FAQ), "Hire Me" CTA button.
2. **Hero** — H1: "Senior Full-Stack & AI Developer for Hire"; subhead with 6+ years / global remote pitch; primary CTA "Get a Free Project Quote" (→ #contact), secondary CTA WhatsApp deep link.
3. **Services** — 4 cards (Web Development, Mobile Apps, AI & ML Solutions, DevOps & Cloud), each H3 + keyword-rich 2-3 sentence copy targeting "hire freelance X developer" search intent.
4. **Why hire me** — trust signals: 6+ years experience, end-to-end ownership, overlap with US/EU time zones, clear communication. (No fabricated testimonials or fake client logos.)
5. **Skills** — grouped tech chips: Frontend (React, Next.js, TypeScript), Backend (Node.js, Python), Mobile (React Native, Flutter), AI/ML (LLM integrations, OpenAI/Claude APIs, RAG), DevOps (AWS, Docker, Kubernetes, CI/CD). *(Generic senior full-stack list — user can edit; marked with HTML comment.)*
6. **Process** — 4 steps: Discovery call → Proposal & estimate → Build with weekly demos → Launch & support.
7. **FAQ** — 5-6 long-tail questions (cost, timezone, engagement models, NDA, maintenance) marked up for FAQ rich results.
8. **Contact** — email button (mailto), WhatsApp button (`https://wa.me/919899986773` with pre-filled message), LinkedIn button. Footer with copyright.

## SEO requirements

- `<title>` ≈ "Yashdeep Tomer — Senior Full-Stack & AI Developer for Hire | Web, Mobile, DevOps"
- Meta description ~155 chars with hiring intent keywords.
- Canonical link, Open Graph tags, Twitter card tags (placeholder domain).
- JSON-LD: `Person` (+ sameAs LinkedIn), `ProfessionalService`, `FAQPage`.
- Semantic landmarks (`header`, `main`, `section`, `footer`), single H1, logical H2/H3 hierarchy.
- Descriptive anchor text, `lang="en"`, accessible contrast and focus states.
- No render-blocking JS; CSS in one small file; system/self-hosted-free font strategy for instant text paint.

## Visual direction

Distinctive, senior, trustworthy — not a generic template. Dark or off-white
refined palette with one confident accent color, strong typographic hierarchy,
generous whitespace. Must look excellent on mobile (most LinkedIn-referred
traffic is mobile).

## Out of scope (YAGNI)

- Blog, CMS, analytics wiring (user can add Google Analytics/Search Console later — leave an HTML comment marking where).
- Contact form backend (email/WhatsApp/LinkedIn buttons only, per user's channel choices).
- Multi-language support.

## Acceptance criteria

- Page renders correctly at 375px and 1440px widths.
- Valid HTML (no unclosed/misnested tags); JSON-LD parses as valid JSON.
- All three contact links work (mailto:, wa.me with correct number, LinkedIn URL).
- robots.txt and sitemap.xml present and consistent with placeholder domain.
